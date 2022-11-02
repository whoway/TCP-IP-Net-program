# 理解网络编程和套接字

```c
#include <sys/socket.h>
int socket( int domain, int type, int protocol ) ;
```
- 成功时返回文件描述符，失败时返回-1

```cpp
#include <sys/socket.h>
int bind( int sockfd, struct sockaddr *myaddr, socklen_t addrlen);
//成功时返回0，失败返回-1
```

```c
#include <sys/socket.h>
int listen(int sockfd, int backlog)
//成功时返回0，失败return -1
```

```c
#include <sys/socket.h>
int accept(int sockfd, struct sockaddr * addr, socklen_t * addrlen);
- 成功时返回文件描述符，失败时返回-1
```

