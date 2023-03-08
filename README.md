# LearningCenter - Backend

Personal project based on the sample project of the Open Source Application Development course.  
I hope this project can help you during the course :)

## Project Configuration

- Maven
- Java 19
- Spring Boot 3.0.4

## Dependencies

- Spring Security
- Spring Boot Dev Tools
- Spring Web
- Spring Data JPA
- Lombok
- MySQL Driver
- I/O Validation

### JWT

– Json Web Token
```xml
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-api</artifactId>
    <version>0.11.5</version>
</dependency>
```

### Mapper

– Model Mapper 
```xml
<dependency>
    <groupId>org.modelmapper</groupId>
    <artifactId>modelmapper</artifactId>
    <version>3.1.1</version>
</dependency>
<dependency>
    <groupId>org.modelmapper.extensions</groupId>
    <artifactId>modelmapper-spring</artifactId>
    <version>3.1.1</version>
</dependency>
```
## Configure Spring Datasource, JPA and App properties

Open `src/main/resources/application.properties`
```
# DataSource Configuration Properties
spring.datasource.url= jdbc:mysql://localhost:3306/testdb?useSSL=false
spring.datasource.username= root
spring.datasource.password= 12345678

# Hibernate Configuration
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
spring.jpa.hibernate.ddl-auto=

# JWT Configuration Properties
authorization.jwt.secret = WriteHereYourSecretStringKeyForTokenSigningCredentials
authorization.jwt.expiration.days = 7
```