VPC Peering with Different Availability Zones and regions


step1: create VPC's in the different regions with different subnets like us-east a1(App-server),b1(Web-server) and ohio a2(Db-server) as shown in the below diagram 
step2: launch ec2 instances with in the VPC's and try to ping each others ip to establish connection between them so it will not ping because of different vpc with                 different availability zones
step3: so establish communication between these ec2 instances we need to create vpc peering 
step4: go to VPC's click on vpc peering and create vpc with target vpc for example app-server wants to connect with web-server so we mention app-web and db-app db-web in the name of vpc peering and select subnet you want to make peering.
step 5: go to vpc peering which are created click on action to accept request.
step 6: go to route table of each vpc and edit the route table with targeted vpc subnets do this task for every zones and regions. 
step 7: now the vpc peering is done so now try to ping with each others ip and you will get response.

