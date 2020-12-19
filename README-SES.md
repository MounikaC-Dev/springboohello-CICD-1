# Pre-Requisites:
    - Install Jenkins
    - Create SMTP Credentials in SES
    - Verify Emails Address in SES
# Install Java
    yum install java-1.8.0-openjdk -y
# Install Jenkins:
    sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins.io/redhat-stable/jenkins.repo
    sudo rpm --import http://pkg.jenkins.io/redhat-stable/jenkins.io.key
    sudo yum install jenkins -y
    service jenkins start
# Create SMTP Credentials in SES and Verify Emails Address in SES
  [SMTP Credentials and Verifying Email Address](https://github.com/Naresh240/AWS-Document/blob/main/Simple%20Email%20Service.md)
# Configure SES with Jenkins
  Goto Jenkins --> Manage Jenkins --> Configure System
  
  1. Please check "System Admin e-mail address" provided or not

  ![image](https://user-images.githubusercontent.com/58024415/102684258-f9983d00-41fc-11eb-8cc6-086ccea78fde.png)

  2. Provide SES details with jenkins
  
  ![image](https://user-images.githubusercontent.com/58024415/102684282-319f8000-41fd-11eb-8601-77a0b7debe96.png)
  
  Click on Test Configuration
  
  ![image](https://user-images.githubusercontent.com/58024415/102684332-83e0a100-41fd-11eb-9c40-4851620213aa.png)

# Create jenkins job with Jenkins-SES and Build
  ![image](https://user-images.githubusercontent.com/58024415/102684393-1a14c700-41fe-11eb-9176-d60dae64e2ed.png)

  Go and Check whether you get mail or not
