//To update

sudo apt update

// To install java

sudo apt install openjdk-8-jdk -y


//add the key to your system

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc    


https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key

//Then add a Jenkins apt repository entry:

 echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]     
 
 https://pkg.jenkins.io/debian-stable binary/ | sudo tee    
 
 /etc/apt/sources.list.d/jenkins.list > /dev/null

 //Update your local package index, then finally install Jenkins:
 
sudo apt-get update

sudo apt-get install fontconfig openjdk-17-jre

sudo apt-get install jenkins

//To check the java version

java -version

//To start the jenkins:

sudo systemctl start jenkins

sudo systemctl enable jenkins

//To check the status of the jenkins:

sudo systemctl status jenkins


//Permission to run the jenkins in your webpage

sudo cat /var/lib/jenkins/secrets/initialAdminPassword

//To run it in your browser give the IP address of your EC2 instance which you created

<your IP address>:8080/

//To install git

sudo apt-get update

sudo apt-get install git
