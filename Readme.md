Tagging : v(version),lw - lightweight tagging
----
git tag v 0.0.01-lw - 

Changes : This is a sample microservice. The first version of this microservice will be tagged in git. This microservice serves couple of end points which just returns some hardcoded response.

The two endpoints are

http://localhost:8101/employee/all
http://localhost:8101/employee/id/1

----
git tag v 0.0.02-lw
Changes : Additional class for Swagger configuration has been added
URL for accessing Swagger UI - http://localhost:8101/swagger-ui.html

---
git tag v 0.0.03-lw

Changes : liquibase introduced to connect to db and execute sql scripts contained withing 
resources/db/changelog/changes folder.
db.changelog-master.yaml is the master file which controls the version.
A new entity class has also been introduced which represents the employee table.

IGNORE: java.sql.SQLFeatureNotSupportedException


You will also see extensive usage of lombok getter and setter. Lombok jar should be present on the classpath.
Lombok plugin needs to be installed on STS,Eclipse etc.
To add the plugin follow the below steps
1) Locate lombok-${version}.jar
2) run it from cmd prompt using Java -jar lombok-${version}.jar
3) A installer pop-up will appear. Provide the path by clicking on specify location and provide the path to the folder where eclipse.exe or sts.exe is present. 
4) Then click on install update
5) Restart your dev tool. You are ready to use lombok annotations.

Note: Lombok has been present in the project from tag v 0.0.01-lw.



