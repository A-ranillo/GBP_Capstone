# SOFTWARE
This will cover software that is being used. This includes operating system of VM.
<br><br>
## ROUTER/FIREWALL/NIDS
We will be using opnsense. Why opnsense? because it's the bleeding edge and when doing something that is very ambitious like this capstone- getting frequent updates and features is very handy. Initially it was supposed to be pfsense BUT I've heard from people that pfsense just lacks the support of new features so; opnsense it is. opnsense has also a built in NIDS called Suricata.
<br><br>
## VM1/SERVER VM
This VM will be using Linux Mint XFCE. This is our "victim". This will host alot of our software such has container, local AI, and SIEM. We could've done a headless system without a desktop environment such as ubuntu server but- for troubleshooting purposes having a desktop environment is super duper handy. 
<br><br>
## CONTAINER
For containerization we used docker for ease of use. To manage the docker containers we have portainer. All docker containers are in docker-compose/docker stack. the docker-compose.yml file will be in another folder.
<br><br>
## SIEM
**OH BOY- OH BOY- I HAVE SUCH A PROBLEM WITH THE INTIAL SIEM DECISION.** SO- originally- the decision was to use elastic stack ELK. E = elasticsearch, L = Logstash, K = Kibana. I was following the official [github repo](https://github.com/elastic/elasticsearch/tree/main/docs/reference/setup/install/docker) of how to deploy elastic docker stack. THE DOCKER COMPOSE FILE IS 2 YEARS OLD AND THERES SO MANY CONFIGURATION MISSING.
