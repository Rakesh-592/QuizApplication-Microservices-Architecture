************************************Micro Services

Cloud Ready VS Cloud-Native

12-Factor App

******************************************10:16 AM 9/21/2025

doing load balancing b/w microservices

Api Gateway, Service Registry, Load Balancer

Faile Fast 

Building is Easy, learn connecting them 


=>Spring Web, PostgreSQL Driver, DATA JPA, Lombok } add these dependencies at spring io


**************************11:06 AM 9/23/2025

Adding HttpResponse codes to your code 
Error handling the app

SQL queries, Native Queries

***********************************6:08 AM 9/28/2025
Complete buiding a Monlithic quiz app

will be creating Microservices out of it

=> Open Feign, Eureka Discovery Client

******************11:32 AM 10/3/2025

Running the Question Service and we are using multiple instances(port nos)

Problem faced: pgadmin 4 server timeout or expired error 
open services from search window -> go to PostgreSQL, run it 
then reopen the app

-Dserver.port=8081

****************8:30 PM 10/3/2025

building quiz service(this have it's own quiz db 
& this service interacts with question service 

=>Spring Web, PostgreSQL Driver, DATA JPA, Lombok, Eureka Client, OpenFeign } add these dependencies at spring io

=> Need of Service Discovery 

 we use Feign to interact with service
we use discovery client to discover server 

we need to get Eureka server, eureka client and open feign

=> Creating a Service Registry 
 creating an Eureka Server 

add eureka server dependency and download prjct service-registry from spring initializr 

add @EnableEurekaServer annotation 

start the eureka-registry 

then go to question service, enable eureka client in pom &
start the service 

******************9:11 AM 10/4/2025

feign client connection 

make your Quiz model return a list of integers and 
then the annotation should be @ElementCollection not 
@ManyToMany

Add @EnableFeignClients for the spring Application to enable 
Feign client

In Question service implement logic

in app properties add port num to 8090 and application name

=> Microservice calling a microservice

http://localhost:8090/quiz/create



***********************************5:14 PM 10/5/2025

=>Completing the 2 microservices

Restart app after code changes before making any api calls


=>Load Balancing 
spring with it's dependencies by default balances load &
openfeign helps to manage it

use Environment to check it on console(like printing which port it's running on)

ok my net is fast i didn't see other port Lol

=>API GateWay

add Gateway, Eureka Client dependencies in Spring Initializr
