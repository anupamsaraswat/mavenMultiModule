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



*) run my-rest-webapp

mvn clean package jetty:run -pl my-rest-webapp

to run all the web apps mvn clean package jetty:run
