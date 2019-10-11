```bash
#!/bin/sh
sudo yum update -y
sudo amazon-linux-extras install docker -y
sudo systemctl enable docker
sudo systemctl start docker
sudo docker container run --publish 8080:80 --name c9 --restart unless-stopped --detach secobau/4399-c9
# sudo docker container exec -ti c9 sh
# curl FPFISSUPP-4399-C9-ca7a5c5bc71e5f90.elb.eu-central-1.amazonaws.com:8080/API/ -H "Content-Type: application/json" -X POST -d '{"colour":"red", "size":"small"}' ; echo
# curl FPFISSUPP-4399-C9-ca7a5c5bc71e5f90.elb.eu-central-1.amazonaws.com:8080/API/;echo
```
