# Offer-Oriented Notebook
这是本人面向2022年和2023年的实习找工笔记。
### 03 数组中重复的数字
1. 排序然后判断，排序时间O(nlogn)
2. 哈希表unordered_map查找重复元素
 O(1)查找该元素是否已经在哈希表中，不在就添加进去；若存在，则返回该元素
时间O(n)，空间O(n)
```C++
class Solution {
public:
    int findRepeatNumber(vector<int>& nums) {
        unordered_map<int, bool> hash;
        for(int num:nums)
        {
            if(hash[num])   return num;
            hash[num]=true;
        }
        return -1;
    }
};
```
3. 利用条件“长度为n的数组里所有元素都在0-n-1范围内
如果该数组中没有重复元素，则nums[i]=i；
这样可以将空间缩小为O(1)，同时虽然有两重循环，但每个元素最多经过两次交换就能确定位置，因此时间为O(n)
```C++
class Solution {
public:
    int findRepeatNumber(vector<int>& nums) {
        int i=0;
        while(i<nums.size())
        {
            if(nums[i]==i)
            {
                i++;
                continue;
            }
            if(nums[nums[i]]==nums[i])  return nums[i];
            swap(nums[i], nums[nums[i]]);
        }
        return -1;
    }
};
```
### 04 二维数组中的查找
利用该矩阵的特性，每次选取左下角或者右上角的数字，时间O(行数+列数)，空间O(1)；如果选择右下角或者左上角，无法剔除该元素所在的行或者列
```C++
//利用该矩阵提供的的特性
class Solution {
public:
    bool findNumberIn2DArray(vector<vector<int>>& matrix, int target) {
        int i=matrix.size()-1, j=0;
        if(matrix.size()==0||matrix[0].size()==0)       return false;
        while(i>=0&&j<=matrix[0].size()-1)
        {
            if(matrix[i][j]>target) i--;
            else if(matrix[i][j]<target)    j++;
            else return true;
        }
        return false;
    }
};
```

