
https://www.cnblogs.com/zrtqsk/p/3735273.html

准确的了解Spring Bean的生命周期是非常必要的。我们通常使用ApplicationContext作为Spring容器。这里，我们讲的也是 ApplicationContext中Bean的生命周期。而实际上BeanFactory也是差不多的，只不过处理器需要手动注册


Bean的完整生命周期经历了各种方法调用，这些方法可以划分为以下几类：

1、Bean自身的方法　　：　　这个包括了Bean本身调用的方法和通过配置文件中<bean>的init-method和destroy-method指定的方法

2、Bean级生命周期接口方法　　：　　这个包括了BeanNameAware、BeanFactoryAware、InitializingBean和DiposableBean这些接口的方法

3、容器级生命周期接口方法　　：　　这个包括了InstantiationAwareBeanPostProcessor 和 BeanPostProcessor 这两个接口实现，一般称它们的实现类为“后处理器”。

4、工厂后处理器接口方法　　：　　这个包括了AspectJWeavingEnabler, ConfigurationClassPostProcessor, CustomAutowireConfigurer等等非常有用的工厂后处理器　　接口的方法。工厂后处理器也是容器级的。在应用上下文装配配置文件之后立即调用。

--- 
Spring 实战 P105


## 了解了Bean的生命周期之后有什么用？


---

这部分网上有很多文章都讲到了，下面的内容整理自：yemengying.com/2016/07/14/… ，除了这篇文章，再推荐一篇很不错的文章 ：www.cnblogs.com/zrtqsk/p/37… 。
https://juejin.im/post/5cf7ca6d6fb9a07ef71062d7



