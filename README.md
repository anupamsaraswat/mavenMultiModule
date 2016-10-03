# mavenMultiModule

*) create new maven project 

mvn archetype:generate -DgroupId=com.anupam.app -DartifactId=my-app -DinteractiveMode=false -DarchetypeArtifactId=maven-archetype-quickstart

change packaging type in pom.xml to >pom<.


*) create new web project 

mvn archetype:generate -DgroupId=com.anupam.app -DartifactId=my-webapp -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false


*) create new service project 

mvn archetype:generate -DgroupId=com.anupam.app -DartifactId=my-service -DinteractiveMode=false -DarchetypeArtifactId=maven-archetype-quickstart


*) create new web project 

mvn archetype:generate -DgroupId=com.anupam.app -DartifactId=my-rest-webapp -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false



*) run web application --- my-rest-webapp
to run multiple web application  using jetty as in  this example my-rest-webapp, my-webapp

-- mvn jetty:run -pl my-rest-webapp (appliation will run on default port 8080)
open another terminal session and run 
-- mvn jetty:run -Djetty.http.port=8081 -pl my-webapp (application will run on port 8081 provided port is available)
