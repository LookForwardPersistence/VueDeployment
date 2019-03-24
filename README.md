# VueDeployment
Vue前端框架部署问题


#### 一、history模式路由时vue前端部署到tomcat，刷新404问题
##### 1、必须部署到tomcat的root下
##### 2、后台支持，WEB-INFA/web.xml 添加404时重定向到根目录，
###### <error-page>
    <error-code>404</error-code>
    <location>/</location>
  </error-page>

##### 3、访问地址不允许有路径（根目录访问）
