# spring-microservice-archetype
Simple Maven Archetype to initialize a Microservice Spring Project with initial dependencies

## List of Dependencies:
- Spring Web
- JPA
- DevTools
- Lombok
- Flyway
- Validation
- Actuator
- OpenFeign
- MySQL Driver
- Zipkin
- Eureka Client
- Swagger UI

## Criando o archetype
$ mvn archetype:create-from-project no root do projeto
- adicionar settings.xml em  user/username/.m2
```
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
					  https://maven.apache.org/xsd/settings-1.0.0.xsd">
</settings>
```

Em ~/target/generated-sources/archetype
- $ mvn clean install
- isso adiciona a pasta do build do projeto em .m2/repositories


## Criando um projeto apartir do archetype

No local onde irá criar o projeto
- $ mvn archetype:generate -DarchetypeGroupId=br.com.erudio -DarchetypeArtifactId=rest-with-spring-boot-and-java-archetype
