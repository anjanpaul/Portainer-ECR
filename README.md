# Install Portainer

## Community Edition 
![alt text]()

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
![alt text]()

## Portainer Admin Panel

![alt text]()

## Dashboard

![alt text]()

Then Create default user and password. 

AND GOOD TO GO :)