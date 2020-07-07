回答的时候我个人觉得把每个模块的大致作用说一下更好：

（1）spring core：提供了框架的基本组成部分，包括控制反转（Inversion of Control，IOC）和依赖注入（Dependency Injection，DI）功能。

（2）spring beans：提供了BeanFactory，是工厂模式的一个经典实现，Spring将管理对象称为Bean。

（3）spring context：构建于 core 封装包基础上的 context 封装包，提供了一种框架式的对象访问方法。

（4）spring jdbc：提供了一个JDBC的抽象层，消除了烦琐的JDBC编码和数据库厂商特有的错误代码解析， 用于简化JDBC。

（5）spring aop：提供了面向切面的编程实现，让你可以自定义拦截器、切点等。

（6）spring Web：提供了针对 Web 开发的集成特性，例如文件上传，利用 servlet listeners 进行 ioc 容器初始化和针对 Web 的 ApplicationContext。

（7）spring test：主要为测试提供支持的，支持使用JUnit或TestNG对Spring组件进行单元测试和集成测试。


