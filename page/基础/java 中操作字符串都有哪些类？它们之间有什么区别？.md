```
String、StringBuffer、StringBuilder

String : final修饰，String类的方法都是返回new String。即对String对象的任何改变都不影响到原对象，对字符串的修改操作都会生成新的对象。
StringBuffer : 对字符串的操作的方法都加了synchronized，保证线程安全。
StringBuilder : 不保证线程安全，在方法体内需要进行字符串的修改操作，可以new StringBuilder对象，调用StringBuilder对象的append、replace、delete等方法修改字符串。


String str="i"与 String str=new String("i")一样吗？
不一样， 第一种是直接虚拟机分配到常量池中，第二种事分配到堆内存中，即使内容一样也会创建新的对象。
反转字符串
StringBuffer、StringBuilder 成员方法中resverse() 方法
```

```
String 常用的方法：
	indexOf() 		返回指定字符得索引
	charAt() 		返回指定索引处得字符
	repalce() 		字符串替换
	trim() 			去除字符串两端的空白
    split() 		分割字符串 返回分割后的字符串数组
	getBytes()  	返回字符串的byte类型数组
	length() 		返回字符串的长度
	toLowerCase()	字符串转小写
	toUpperCase() 	字符串转大写
	substring() 	截取字符串
    equals() 		字符串比较
   ```