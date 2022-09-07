# problem01
一个有问题的代码源码

关于maven使用<plugin>导入tomcat插件问题


单独使用
![image](https://github.com/shzy2022/problem01/blob/main/readme_photo/plugin_tomcat.png)
配置可以生效
tomcat可以运行

但是在依赖加上tomcat后
![image](https://github.com/shzy2022/problem01/blob/main/readme_photo/dependency_tomcat.png)
会发生错误
![image](https://github.com/shzy2022/problem01/blob/main/readme_photo/error.png)

不知道原因是什么
有人说
@WebServlet里urlPattern的路径时没有在前面加“/“
![image](https://github.com/shzy2022/problem01/blob/main/readme_photo/reslove01.png)
#没试过，找机会试试

有人说
是servlet-mapper配置的问题
要加上<scope>provided</scope>
![image](https://github.com/shzy2022/problem01/blob/main/readme_photo/reslove02.png)
#没试过，找机会试试

也有说
https://developer.aliyun.com/article/342754

总结：学会看日志，才能更好的解决问题
