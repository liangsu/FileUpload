# FileUpload
这是一个个人测试文件断点续传的例子

* * * *




## 一、遇到的问题总结：
	1.在servelt-api-2.4.jar中，在jsp中写下载程序，下载后的excel打开后始终是乱码，经过多次尝试，发现要在jsp代码块的开头加上:
```
out.clear();
out = pageContext.pushBody();
```
