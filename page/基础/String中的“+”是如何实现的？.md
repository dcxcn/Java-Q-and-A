https://www.cnblogs.com/xiaoxi/p/6036701.html
```
String c = "xx" + "yy " + a + "zz" + "mm" + b; 实质上的实现过程是： String c = new StringBuilder("xxyy ").append(a).append("zz").append("mm").append(b).toString();
底层通过 StringBuilder实现
```

