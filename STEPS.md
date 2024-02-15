# <b> *Fourth WorkShop Distribuidos* </b>

## <b> STEP BY STEP </b> 

To set up DNS resolution for microservices, follow these steps:

1. Begin by installing the dnsmasq service, which facilitates DNS functionality.

2. Next, create a configuration file named '10-consul' within the directory etc/dnsmasq.d. In this file, specify the server address with the loopback IP and port. For instance:

      Server=/consul/127.0.0.1#8600
   
3.Restart the dnsmasq service to apply the changes made in the configuration file.
4. Modify the resolv.conf file to enable DNS resolution for services hosted on the local machine. Add the following line to the file:

      nameserver 127.0.0.1
      
5.Verify that the DNS service is correctly resolving the IP addresses of each microservice. Use the command dig .service.consul in the terminal. Ensure that the localhost address (127.0.0.1) and port (8500) are accessible through the browser

## <b> Microservices registered in Consul </b> 

![image](https://github.com/PaulaTrujillo27/sd-workshop4/assets/71205932/14e91c91-9f94-405d-865d-cd26dc4757ca)

## <b> By: </b>


+ [Paula Andrea Trujillo Mejia](https://github.com/PaulaTrujillo27 "Paula T.")
+ [Icesi-Ops](https://github.com/icesi-ops")




<br>


