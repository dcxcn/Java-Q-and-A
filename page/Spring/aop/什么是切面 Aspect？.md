aspect 由 pointcount 和 advice 组成，切面是通知和切点的结合。 它既包含了横切逻辑的定义, 也包括了连接点的定义. Spring AOP 就是负责实施切面的框架, 它将切面所定义的横切逻辑编织到切面所指定的连接点中. AOP 的工作重心在于如何将增强编织目标对象的连接点上, 这里包含两个工作:

（1）如何通过 pointcut 和 advice 定位到特定的 joinpoint 上

（2）如何在 advice 中编写切面代码.

可以简单地认为, 使用 @Aspect 注解的类就是切面.

