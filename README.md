### spring-cloud-config-server-svn
This is a sample project for the spring cloud config server with subversion

### Client 

For the client and add the starter dependency:

```
  <dependency>
	<groupId>org.springframework.cloud</groupId>
	<artifactId>spring-cloud-starter-config</artifactId>
  </dependency>
  
```

Create a file "bootstrap.yml" and put it in the src/main/resources folder:

```
spring:
  application:
    name: appname
  profiles:
    active: qa
  cloud:
    config:
      fail-fast: true 
      uri: http://localhost:8761
      username: admin
      password: admin
      name: appname
      profile: qa 
      label: label
      
   ````
 
