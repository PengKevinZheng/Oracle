# Oracle

##实例
    用Oracle官方描述：实例是访问Oracle数据库所需的一部分计算机内存和辅助处理后台进程，是由进程和这些进程所使用的内存(SGA)所构成一个集合。
    
    其实就是用来访问和使用数据库的一块进程，它只存在于内存中。就像Java中new出来的实例对象一样。 
    
    我们访问Oracle都是访问一个实例，但这个实例如果关联了数据库文件，就是可以访问的，如果没有，就会得到实例不可用的错误。  
##监听  
    当用户登录数据库时，用户进程发送请求，服务器端的监听程序监听到用户进程的请求，使用listener.ora核对用户连接信息，如果正确，则启动一个服务器进程，  
    
    然后把用户进程直接或者间接交付给服务器进程。
