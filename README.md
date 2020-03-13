# Using tinylog with Spring Boot

There are two possibilities how to use tinylog together with Spring Boot. The simplest way is to add the tinylog API and configure logging via Spring. In thise case, just add tinylog-jul or tinylog-jboss as dependency. [See profile "output via spring" in POM](https://github.com/pmwmedia/tinylog-spring-boot-example/blob/v2/pom.xml#L24)

The second way is to replace Spring Boot's Logback implementation with tinylog. In this case, all log entries from Spring will be redirected to tinylog and logging can be configured via tinylog. [See profile "output via tinylog" in POM](https://github.com/pmwmedia/tinylog-spring-boot-example/blob/v2/pom.xml#L48)
