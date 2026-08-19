# Dockerized Python Web Application Deployment

> *Project Overview:* I created a simple Python and HTML web application and deployed it using Docker, Docker Hub, and AWS EC2. I first prepared the application locally, installed Docker on my local machine, built the Docker Image, uploaded it to Docker Hub, and then deployed the same Image on an AWS EC2 Instance. Finally, I accessed the running application through the EC2 Public IP and Port 5000 using a web browser.
> ![Project](https://github.com/user-attachments/assets/f79c5f47-dc54-453e-8821-3957114d7ade)

---

## 1. Docker Installation on Local Machine

* I installed Docker on my local machine.
* I used the local terminal to verify that Docker was installed and ready to use.
* Docker was used to containerize the web application.

> ![Docker Installation](https://github.com/user-attachments/assets/5243a834-f220-4fd6-9370-8555b42d6945)
---

## 2. Docker Build

* I created a Dockerfile for the application.
* I used Docker Build to build the application based on the Dockerfile.
* After the build process was completed, the application was packaged into a Docker Image.

> ![Docker Build](https://github.com/user-attachments/assets/5b54fbdd-9e30-47b2-952d-55669a03869f)

---

## 3. Docker Image

* After completing the build process, I verified that the Docker Image was created successfully on my local machine.
* The Docker Image contains the application and everything required to run it inside a Docker Container.

> ![Docker Image](https://github.com/user-attachments/assets/5973ff30-89f7-41ba-825e-34bbfdcb5c74)

---

## 4. Docker Hub Login, Tagging and Image Push

**Docker Hub Account, Login, Tagging, and Image Push**

* Created a Docker Hub account to store and manage the Docker Image.
* Logged in to Docker Hub from the local terminal.
* Tagged the Docker Image using my Docker Hub username and repository name.
* Pushed the Docker Image from my local machine to Docker Hub.
* The Docker Image was successfully uploaded to Docker Hub and is ready to be deployed on AWS EC2.

> ![Docker Hub Login, Tagging and Push](https://github.com/user-attachments/assets/66d82dff-b584-45a0-923d-cefdccc946f5)

---

## 5. Docker Image on Docker Hub

* I opened my Docker Hub Repository and verified that the Docker Image was uploaded successfully.
* The Image was available online and ready to be pulled by the AWS EC2 Instance.

> ![Docker Hub Repository](https://github.com/user-attachments/assets/ca54323a-d34f-4830-96e7-5fa52043b443)

---

## 6. AWS Security Group

* I configured the EC2 Security Group to allow inbound traffic through Port 5000.
* This allowed the web application running inside the Docker Container to be accessed from outside the EC2 Instance.

> ![AWS Security Group](https://github.com/user-attachments/assets/2747e9fd-6d1d-40b5-ab48-724a7c3a8653)

-----

## 7. AWS EC2 Instance

* I created and opened an AWS EC2 Instance.
* The EC2 Instance was used as the server where the Docker Container would run.
* I connected to the EC2 Instance through the terminal.

> ![AWS EC2 Instance](https://github.com/user-attachments/assets/ff51e1b4-7715-42bd-82d6-f02b288cfd87)


---


## 8. Docker Installation on EC2

* I installed Docker on the AWS EC2 Instance.
* Docker was prepared to run containers on the EC2 server.
* I verified that Docker was available on the EC2 Instance.

> ![Docker on EC2](https://github.com/user-attachments/assets/59fcf5cc-1889-4374-829a-7462f60ed5ab)



---

## 9. Pull Docker Image from Docker Hub

* From the EC2 terminal, I pulled the Docker Image from my Docker Hub Repository.
* The Image was downloaded from Docker Hub to the EC2 Instance.
* After the Pull operation, the Image became available locally on the EC2 server.

> ![Pull image ](https://github.com/user-attachments/assets/8d42b6c7-213f-4e34-9db0-03d670cda630)


---

## 10. Run the Docker Container

* I used the Docker Image pulled from Docker Hub to run the application.
* A Docker Container was created and started on the EC2 Instance.
* Port 5000 was mapped to allow access to the web application.

> ![Docker Run ](https://github.com/user-attachments/assets/d2f69153-1845-4003-b110-5cbb4ac8dddd)

---

## 11. Running Docker Container

* After running the Docker Container, I verified that the container was running successfully.
* The Python web application was now running inside the Docker Container on the AWS EC2 serve

---

## 12. Access the Application from Web Browser

* After the Docker Container was running successfully, I opened a web browser.
* I entered the Public IP address of the AWS EC2 Instance.
* I added Port 5000 to the Public IP address.
* The web application opened successfully in the browser.

> ![Web Browser Result](https://github.com/user-attachments/assets/d5f4d72e-5f71-4d89-9804-be9e4d270b54)

---

## Project Workflow

> *The complete deployment process I performed:*

```text
Python + HTML Files
        ↓
Docker Installed Locally
        ↓
Dockerfile
        ↓
Docker Build
        ↓
Docker Image
        ↓
Docker Hub Login
        ↓
Docker Tag
        ↓
Docker Push
        ↓
Docker Image on Docker Hub
        ↓
AWS EC2 Instance
        ↓
Docker Installed on EC2
        ↓
Docker Pull
        ↓
Docker Run
        ↓
Docker Container Running
        ↓
EC2 Public IP + Port 5000
        ↓
Web Browser
        ↓
Web Application
