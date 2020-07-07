![](http://ww1.sinaimg.cn/large/007s8HJUly1g5w4sq64ymj30xf0bvtfd.jpg)

在存储散列集合时〔如Set类),如果原对象equals新对象,但没有对 hashCode重写,即两个对象拥有不同的hashCode,则在集合中将会存储两个值相同的对象,从而导致混看。因此在重写 equals方法时,必须重写 hashCode


