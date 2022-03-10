# 02-引入错误提示和读写操作
## perror
为了方便和可读性，可以封装一个错误处理函数
```C++
void errif(bool condition, const char *errmsg){
    if(condition){
        perror(errmsg);
        exit(EXIT_FAILURE);
    }
}
//perror: 打印出errno的实际意义，还会打印我们传入的字符串
//exit: 程序退出，返回预定义常量
```
## 建立Socket连接后的数据读写

对于TCP，可以使用<unistd.h>头文件中的read和write；

对于UDP，可以使用sendto和recvfrom。
