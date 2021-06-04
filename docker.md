![image-20210419175406201](docker.assets/image-20210419175406201.png)



**exit 退出镜像**

![image-20210419175615926](docker.assets/image-20210419175615926.png)



**容器的退出**

![image-20210422144155712](docker.assets/image-20210422144155712.png)







**docker安装mysql: **                     （映射时主机不存在对应目录或文件不要紧，docker会自动创建。）

![image-20210425095658778](docker.assets/image-20210425095658778.png)

`````cmd
docker run -p 3306:3306 --name mysql -v /home/lww/docker/mysql/conf:/etc/mysql/conf.d  
-v /home/lww/docker/mysql/logs:/logs 
-v /home/lww/docker/mysql/data:/var/lib/mysql 
-e MYSQL_ROOT_PASSWORD=123456 
-d mysql:5.7
`````

![image-20210425101341238](docker.assets/image-20210425101341238.png)





**docker里面的mysql，数据库导出为sql文件  放到主机目录:**

![image-20210425101851216](docker.assets/image-20210425101851216.png)

`````cmd
docker exec 78194affc22f sh -c ' exec mysqldump -- all-databases -uroot -p"123456" '  >  /home/lww/all-databases.sql
`````



