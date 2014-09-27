hello-maven-jetty
=================

Sample test project for maven jetty web app

Starting Jetty
==============
```
mvn jetty:run
```
launch http://localhost:9000/helloworld

war packaging
=============
```
mvn package
```
go to target folder and grab .war file and you can deploy to tomcat/webapps folder directly
or better write build.xml and have the ant target to deploy it to tomcat/webapps

copying to tomcat
=================
```
mvn dependency:copy
```
You have define two parameters:
```
<package.name>hello-maven-jetty.war</package.name>
<webapps.path>/opt/apache-tomcat-8.0.12/webapps</webapps.path>
```
