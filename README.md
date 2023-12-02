# Jenkins CI/CD Pipeline - SonarQube, Docker, Github Webhooks on AWS
-------------------

![Devops Project](https://github.com/Kanakaprasad/Devops-Project/assets/106590219/2bba7102-28a5-423e-803f-534924061f5f)

-------------------

## Launch 3 EC2 instances

1. Jenkins
2. SonarQube
3. Docker

-------------------
![image](https://github.com/Kanakaprasad/Devops-Project/assets/106590219/c04adb03-da3e-4c3d-a2f8-7e0c774c8a2f)

-------------------

# 1. Jenkins------------>

### Connect instance with command prompt


Change Jenkins machine host name

   		hostnamectl set-hostname Jenkins
		/bin/bash

Update instance

		sudo apt-get upadate

Install java version 17 Run Time Environment

		sudo  apt install openjdk-17-jre

		sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \ https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
		echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \ https://pkg.jenkins.io/debian-stable binary/ |
		sudo tee \ /etc/apt/sources.list.d/jenkins.list > /dev/null

		sudo apt-get update

		sudo apt-get install jenkins

Verify jenkins & to copy the jenkins secrete key

		systemctl status jenkins

Goto Jenkins EC2 instance add 8080 port number to inbound traffic

	
### Open the jenkins machine in browser with ip(jenkins):8080

	- paste the jenkins secrete key
   	- install suggested plugins
   	- create a jenkins admin user
