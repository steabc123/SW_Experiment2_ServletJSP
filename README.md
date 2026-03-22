利用JSP+Servlet开发一个基于Web的计算器

项目说明：
本项目实现了一个简单的Web计算器，通过JSP页面收集用户输入，使用Servlet处理业务逻辑，并调用Calculator类完成具体运算。

项目结构：
src/main/java/com/demo/servlet/
  - Servlet.java：处理HTTP请求，接收前端参数并调用计算器
  - Calculator.java：计算器核心逻辑，实现四则运算功能

src/main/webapp/
  - calcu_servlet.jsp：计算器前端界面，包含输入表单
  - index.jsp：默认首页
  - WEB-INF/web.xml：Servlet配置文件

功能特点：
1. 支持加、减、乘、除四则运算
2. 前端使用JSP技术实现用户界面
3. 后端使用Servlet处理请求
4. 包含除零异常处理，避免程序崩溃
5. 使用Maven进行项目构建管理

使用方法：
1. 部署项目到支持Servlet的Web服务器（如Tomcat）
2. 访问calcu_servlet.jsp页面
3. 输入两个数字并选择运算符
4. 点击计算按钮查看结果

技术栈：
- Java 22
- Jakarta EE Servlet API 5.0
- JSP
- Maven 3.8.4
- Tomcat 10.1.19

配置信息：
pom.xml中已配置必要的Servlet依赖，项目打包方式为WAR包。
web.xml中配置了Servlet映射路径为/calculServlet。
