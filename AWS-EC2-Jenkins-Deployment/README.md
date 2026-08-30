# Jenkins Deployment on AWS EC2

## Objective

Deploy Jenkins on an Ubuntu EC2 instance and access Jenkins through a web browser.

## Technologies Used

- AWS EC2
- Ubuntu
- SSH
- Java
- Jenkins
- AWS Security Group

---

## 1. AWS EC2 Instance Creation

Created an Ubuntu EC2 instance in AWS.

![AWS EC2 Instance](00-aws-ec2-instance-created%5B1%5D.png)

---

## 2. SSH Connection

Connected to the Ubuntu EC2 instance using SSH through MobaXterm.

![SSH Connection](01-ssh-connection%5B1%5D.png)

---

## 3. Java Installation

Installed Java on the Ubuntu EC2 instance as a prerequisite for Jenkins.

![Java Installation](02-java-installation%5B1%5D.png)

---

## 4. Verify Java Version

Verified that Java was successfully installed.

```bash
5.java -version5. Jenkins Installation

Installed Jenkins on the Ubuntu EC2 instance.

6. Check Jenkins Service Status

Checked the Jenkins service and verified that it was running.

sudo systemctl status jenkins

7. Configure Jenkins Port 8080

Configured the AWS EC2 Security Group to allow inbound traffic on port 8080 so that Jenkins could be accessed through a web browser.

Jenkins commonly runs on port 8080 by default.

8. Jenkins Initial Setup

Retrieved the Jenkins initial administrator password required for the first-time setup.

Security Note: Never expose passwords, private keys, or other sensitive credentials in a public GitHub repository.

9. Jenkins Dashboard

Successfully accessed the Jenkins application through the browser.

Result

Successfully deployed Jenkins on an AWS EC2 Ubuntu instance, connected to the server using SSH, installed Java and Jenkins, configured port 8080, and accessed the Jenkins dashboard through a web browser.
