# Gerenciador de super heróis da Marvel e da DC em uma API reativa com Spring Boot

Nesta sessão vamos desenvolver uma API de gerenciamento de heróis utilizando Spring WebFlux, utilizada por empresas como Netflix e Pivotal, junto com a library reativa Reactor que atualmente é mantida pela VmWare. Além disso, usaremos o banco DynamoDb localmente para armazenar nossos dados 
e demonstrarei como realizar testes unitários da sua API com Junit e como gerar documentações simples por meio do Postman e também do Swagger.

## Stack utilizada:

  * Java 11
  * Spring Webflux
  * Spring Data
  * DynamoDB
  * JUnit
  * SL4J
  * Reactor
  

### Executar Dynamo: 

Na pasta em que o jar está baixado:

````
java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
````
 
Para listar as tabelas criadas:  

````
aws dynamodb list-tables --endpoint-url http://localhost:8000
````

Documentacao gerada pela aplicação: swagger: http://localhost:8080/swagger-ui-heroes-reactive-api.html

##### Slides de palestra: https://speakerdeck.com/kamilahsantos/live-coding-dio-api-de-herois-com-spring-webflu
