# CommonJS规范：
## 规范的作用：弥补当前javascript没有标准的缺陷，目的是达到像Python、Ruby、Java等具备开发大型应用的基础能力；
## 规范的好处：导出和引入机制使得用户完全不用考虑变量污染

---

## CommonJS规范包括：模块、二进制、Buffer、字符集、I/O流、进程环境、文件系统、套接字、单元测试、web服务器网关接口、包管理等

## Node借鉴CommonJS的Modules规范实现了一套非常易用的模块系统。

##CommonJS的模块规范（模块引用、模块定义、模块标识）：
- 模块引用：var http = require('http');
- 模块定义：
    - 上下文提供exports对象用于导出当前模块的属性或者方法
    - 模块中有个module对象，代表模块本身，exports是module的属性
    - node中，一个文件即是一个模块
```
exports.fun = function () {
    var a = 'test';
    return a;
}
```
- 模块标识：就是传递给require()方法的参数

## 参考
- [CMD 模块定义规范](https://github.com/seajs/seajs/issues/242)