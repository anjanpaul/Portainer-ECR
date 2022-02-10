# Install Portainer

## Community Edition 
![alt text](https://github.com/anjanpaul/Portainer-ECR/blob/main/Output/Screenshot%202022-02-10%20at%2011.11.37%20AM.png)

Set up a new Portainer Server installation for Docker Swarm

## Docker Swarm
Install Portainer with Docker Swarm on Linux

## Deployment
Portainer can be directly deployed as a service in your Docker cluster. Note that this method will automatically deploy a single instance of the Portainer Server, and deploy the Portainer Agent as a global service on every node in your cluster.
First, retrieve the stack YML manifest:

```
curl -L https://downloads.portainer.io/portainer-agent-stack.yml \
    -o portainer-agent-stack.yml
```
Then use the downloaded YML manifest to deploy your stack:

```
docker stack deploy -c portainer-agent-stack.yml portainer

```

Portainer Server and the Agents have now been installed. You can check to see whether the Portainer Server and Agent containers have started by running docker ps:

```
docker ps

```

## Logging In

Now that the installation is complete, you can log into your Portainer Server instance by opening a web browser and going to:

```
https://YourIp:9443

```
![alt text](https://github.com/anjanpaul/Portainer-ECR/blob/main/Output/Screenshot%202022-02-10%20at%2011.27.41%20AM.png)

## Dashboard

![alt text](https://github.com/anjanpaul/Portainer-ECR/blob/main/Output/Dashboard.png)

Then Create default user and password. 

AND GOOD TO GO :)

## AWS ECR
```
Install AWS cli
Create an iam role for an user
Then type 
aws configure on your terminal
it will give a shell to give aws access key and aws secret key
the go to ecr 
create a repo
first you have to decide what you will do? the repository will be private or public
then give a name of your repo
then create repo
to see how to push just click on view push

and good to go

```
