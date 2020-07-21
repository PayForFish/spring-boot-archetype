# spring-boot-archetype  
spring-boot-archetype used to build spring-boot project efficiently  
## 操作指南  
1. 创建自己的项目文件夹，进入然后执行shell:  
~~~shell script
git clone https://github.com/PayForFish/spring-boot-archetype.git
~~~  
2. cd到项目根目录，然后：  
~~~shell script
cd spring-boot-web-backend-archetype
mvn clean install
~~~  
3. 用maven的archetype插件创建脚手架工程，使用IDEA的建议使用集成环境提供的可视化工具：  
   ![](https://picabstract-preview-ftn.weiyun.com/ftn_pic_abs_v3/f37c9023b39a8d2d084bf9a12223a8e67b3c663881cdcf5485008bcb5a36e5fae7afec5b065c1a99bd8a94f6ef6d6c02?pictype=scale&from=30013&version=3.3.3.3&uin=1084856844&fname=WX20200721-140341%402x.png&size=750)  
   
4. 输入项目的相关属性参数：    
   ![](https://picabstract-preview-ftn.weiyun.com/ftn_pic_abs_v3/334e6bd57d298d9b56ebc457eec08db4b311bca8ec11421d8bb0826fa1dc9af4e737295cdb29e88cd99356e5c1ee3f8b?pictype=scale&from=30013&version=3.3.3.3&uin=1084856844&fname=WX20200721-141004%402x.png&size=750)  
   
5. 点击next->创建多模块项目脚手架工程，可自行修改父pom中依赖的版本:)  
## 一些建议  
#### 若项目按服务划分，自行配置RPC相关后service module作为服务化单独启动    
#### 若为单体服务，service module自行删除配置再作为一个依赖在web端引入  
#### module下的package随意命名，请根据自身业务规划，分层  
#### 注意version, 目前最新version为2.0.0, 生成脚手架时注意不是图中1.0.0
