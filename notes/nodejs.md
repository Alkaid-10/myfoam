- 事件
  - Node.js 使用事件驱动模型，当web server接收到请求，就把它关闭然后进行处理，然后去服务下一个web请求。

当这个请求完成，它被放回处理队列，当到达队列开头，这个结果被返回给用户。
- EventEmitter 类
  - EventEmitter 的核心就是事件触发与事件监听器功能的封装。
    - 注册event（使用on函数）: event.on('some_event', function() { 
    //代码 
}); 
  - 创建对象：// 引入 events 模块
var events = require('events');
// 创建 eventEmitter 对象
var eventEmitter = new events.EventEmitter();
  - 触发事件：emit 