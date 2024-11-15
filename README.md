# jenkins-mini-project
This is an introductory mini project for jenkins





#### Set up an AWS instance using Ubuntu AMI 
![image](https://github.com/user-attachments/assets/190481fd-0968-4bf6-b2d6-9693a602c8cd)





#### Update the package repositories
sudo apt update
![image](https://github.com/user-attachments/assets/a5067de2-d1b3-42fc-b5da-209976d49d61)


#### install JDK
sudo apt install openjdk-17-jre
![image](https://github.com/user-attachments/assets/f552bdeb-ad2b-481b-8d79-45e2c3d57f6b)


#### Install Jenkins
curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
![image](https://github.com/user-attachments/assets/84c23a4b-b287-4994-80a5-b07313f78529)


#### Check if Jenkins is installed, and Up and Running 
sudo systemctl status jenkins 
![image](https://github.com/user-attachments/assets/8e962254-e3b0-40f6-b648-02deeb12fa4b)

#### In the Jenkins instance, create new inbound rule for port 8080 in the security group 
By default Jenkins listens on port 8080
![image](https://github.com/user-attachments/assets/1fc9dedf-ed3f-43c0-9300-9e1703279d8d)


#### Set up Jenkins on Web console 
i. Input jenkins instance ip address on the web browser 
ii. On the Jenkins server, run "sudo cat /var/lib/jenkins/secrets/initialAdminPassword" to get the password
![image](https://github.com/user-attachments/assets/a4f9b847-1fb0-4308-9b18-d4d81fd7c16f)

![image](https://github.com/user-attachments/assets/b1e172d9-ba10-4266-a58b-176b21ca70b9)

#### Install suggested plugins 
![image](https://github.com/user-attachments/assets/2c5b537d-7d71-48f8-add6-0ab08a9072cf)


#### Create a user account
![image](https://github.com/user-attachments/assets/42eafb53-bf70-4ecf-af73-7100b5d8a681)



#### Log in to jenkins 
![image](https://github.com/user-attachments/assets/fce34885-d8c1-4b6e-86c9-333ec5c3801f)



## This mini project showcases the foundational knowledge of jenkin. It is an introduction to how jenkins is created. Next we will running jobs on the jenkins already set up. 


































