

![](images/springmvc原理.png)


客户端（浏览器）发送请求，直接请求到 DispatcherServlet。
DispatcherServlet 根据请求信息调用 HandlerMapping，解析请求对应的 Handler。
解析到对应的 Handler（也就是我们平常说的 Controller 控制器）后，开始由 HandlerAdapter 适配器处理。
HandlerAdapter 会根据 Handler来调用真正的处理器开处理请求，并处理相应的业务逻辑。
处理器处理完业务后，会返回一个 ModelAndView 对象，Model 是返回的数据对象，View 是个逻辑上的 View。
ViewResolver 会根据逻辑 View 查找实际的 View。
DispaterServlet 把返回的 Model 传给 View（视图渲染）。
把 View 返回给请求者（浏览器）

作者：Guide哥
链接：https://juejin.im/post/5cf7ca6d6fb9a07ef71062d7
来源：掘金
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

