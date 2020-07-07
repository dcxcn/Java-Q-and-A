通过Jackson框架就可以把Java里面的对象直接转化成Js可以识别的Json对象。具体步骤如下 ：



（1）加入Jackson.jar



（2）在配置文件中配置json的映射



（3）在接受Ajax方法里面可以直接返回Object,List等,但方法前面要加上@ResponseBody注解

