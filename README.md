# Eureka-ServiceDiscovery
This project demonstrates use of Service Discovery in microservice Environment
So we have created a eureka server project which will be using as a service discoverory and Service resitory fo multiple microservices communication
We also have demonstrated client side service discovery and load balancing
We are going to register the microservice instances during the startup 
And when a microservice makes a request to another microservice using Feign Client we will make use of eureka server for providing the list of ips of request services
Client will decide which instance to be used from the returned list of ips based on load balancing stratery in our case we are using derfault stratergy to select the instance
And after selection will make a requst and send a response 
We have also integrated configuration server usign spring cloud to handle congifurations in a centeralized manner 
Conguration sever uses git repository to maintain all the configurations
So first configuration server needs to be started
Then eureka follwed by accounts, loans and cards
We have to first create images of all the projects and then run docker compose file for which ever environment you want

