FileReader类是将文件按字符流的方式读取char数组或者String.

FileInputStream则按字节流的方式读取文件byte数组。

- 1.首先获得一个文件句柄。 File fille= new File();file即为文件句柄。两人之间连
  通电话网络了。接下来可以开始打电话了
- 2.通过这条线路读取甲方的信息: new FileInputStream(fe)目前这个信息已经
读进来内存当中了。接下来需要解读成乙方可以理解的东西
- 3.既然你使用了 FileInputStream()。那么对应的需要使用 InputStreamReader()
这个方法进行解读刚才装进来内存当中的数据
- 4.解读完成后要输出呀。那当然要转换成IO可以识别的数据呀。那就需要调用字节
码读取的方法 Bufferedreader()。同时使用 bufferedReader()的 readline()方
法读取txt文件中的每一行数据哈。

