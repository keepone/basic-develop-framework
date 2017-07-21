# basic-develop-framework
这是我在做彩票项目时搭建的基础框架，基于spring mvc+spring+mybatis,其他项目可以基于这个框架快速开发项目.
目录结构： bh-model：数据模型，与数据库表字段对应的实体类 bh-core：核心业务项目。主要是Service处理业务逻辑 bh-dao：数据持久层，操作低层数据库。 bh-api：用来对外服务的接口。 bh-web :这个就是整个项目的web层了，页面的显示以及控制层
基础功能：包含基础的增删改查功能，已经实现增加，查询代码
开发工具： eclipse luna
数据库： mysql 
运行环境： 
java:java version "1.8.0" Java(TM) SE Runtime Environment (build 1.8.0-b132) Java HotSpot(TM) 64-Bit Server VM (build 25.0-b70, mixed mode)
tomcat:tomcat7.0

注意事项： 
1.maven引用包的升级引起各种冲突

2常见bug
2.1-通过eclipse导入时，可能会报错：
Description	Resource	Path	Location	Type
Archive for required library: '/Users/Allen/.m2/repository/org/mybatis/mybatis/3.2.4/mybatis-3.2.4.jar' in project 'basic-core' cannot be read or is not a valid ZIP file	basic-core		Build path	Build Path Problem

修改eclipse的maven配置，将user setting配置成指定的地址，例如：/Users/Allen/develop/maven/maven-3.5.0/conf/settings.xml

2.2-
Description	Resource	Path	Location	Type
JavaServer Faces 2.2 can not be installed : One or more constraints have not been satisfied.	basic-web		line 1	Maven Java EE Configuration Problem

直接删除忽视即可。

--allen 2017-7.21
