https://blog.csdn.net/woshizisezise/article/details/79374460
```
public static <T> void show1(List<T> list){
 for (Object object : list) {
        System.out.println(object.toString());
    }
}

public static void show2(List<?> list) {
    for (Object object : list) {
        System.out.println(object);
    }
}
public static void test(){
   List<Student> list1 = new ArrayList<>();
   list1.add(new Student("zhangsan",18,0));
   list1.add(new Student("lisi",28,0));
   list1.add(new Student("wangwu",24,1));
   //这里如果add(new Teacher(...));就会报错，因为我们已经给List指定了数据类型为Student
   show1(list1);

   System.out.println("************分割线**************");

   //这里我们并没有给List指定具体的数据类型，可以存放多种类型数据
   List list2 = new ArrayList<>();
   list2.add(new Student("zhaoliu",22,1));
   list2.add(new Teacher("sunba",30,0));
   show2(list2);
}
```
