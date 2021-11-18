# Set up EC2 instance for Rancher
- To setup Airflow on AWS
- Login to AWS
- Create new EC2
  - AMI: Amazon Linux 2
  - t2.small
  - Add security group rules
    - http
    - https
  - Connect to VM using SSH
- Install packages
```
sudo yum update -y
sudo amazon-linux-extras install docker
sudo service docker start
sudo usermod -a -G docker ec2-user
exit
```
- Connect to EC2 again using SSH
```
docker run -d --restart=unless-stopped --name rancher --hostname rancher -p 80:80 -p 443:443rancher/rancher:v2.3.2
docker ps
Copy Public IP of EC2 instance and open in browser
```
