```bash
#!/bin/sh
sudo yum update -y
sudo amazon-linux-extras install docker -y
sudo systemctl enable docker
sudo systemctl start docker
# PUT BELOW THE OUTPUT OF UCP-1 DEPLOYMENT (WORKER TOKEN)
sudo docker swarm join --token XXXXXXXXXX X.X.X.X:2377

#docker image build --tag secobau/4399-aws2c9 https://raw.githubusercontent.com/secobau/4399/aws2c9/Dockerfile
#docker container run --publish 8888:80 --name aws2c9 --restart unless-stopped --detach secobau/4399-aws2c9
```
