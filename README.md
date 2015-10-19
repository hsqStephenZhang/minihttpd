minihttpd
========

基于c++11和socket API实现的web服务器

## 使用方法
```c++
#include "../include/EventLoop/EventLoop.h"
#include "../include/Http/Http.h"

int main()
{
    EventLoop<Http> httpServer(8080);
    httpServer.loop();
    return 0;
}
```