# Project-1

## Installing Jenkins on ubuntu
### get keys
$ sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
###
$ echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
### update apt repositories  
$ sudo apt-get update
### install java
$ sudo apt install fontconfig openjdk-17-jre
### install jenkins
$ sudo apt-get install jenkins
### enable jenkins
$ sudo systemctl enable jenkins
### start jenkins
$ sudo systemctl start jenkins
### defualt port of jenkins is 8080
### password for Unlock Jenkins
$ /var/jenkins/secrets/initialAdminPassword
 


