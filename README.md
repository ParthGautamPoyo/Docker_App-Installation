# Docker_App-Installation
![Screenshot 2024-12-07 192946](https://github.com/user-attachments/assets/07d65aef-9908-4e1c-ad4d-94b852aec7ed)
https://github.com/user-attachments/assets/b9608d5f-1286-443c-ac26-d41f35942763

# Project Contributors
- **Parth Gautam**
  - PGDM-BDA (2023-25)
  - FORE School of Management

---

# Tic Tac Toe Application Installation on Docker

## Project Overview
This project involves the installation and deployment of a Tic Tac Toe game application using Docker. The game was set up to run on a local server accessible via `localhost:4000`. Docker, as a containerization platform, was used to efficiently pull and run the application from a free source repository.

## Objectives
- Understand the process of containerizing applications using Docker.
- Deploy a functional game application using Docker containers.
- Demonstrate the ability to access and interact with the application through a local server.

## Tools and Technologies
- **Docker**: Used for containerizing the application and ensuring consistent runtime environments.
- **PowerShell**: Command-line interface for executing Docker commands on Windows.

## Steps Performed

### 1. Docker Image Pull
The Docker image for the Tic Tac Toe application was pulled from the repository `bign8/games`. This was done using the following command:
```bash
docker pull bign8/games
```
- The `docker pull` command downloads the specified image from Docker Hub.
- The `latest` tag was used to pull the most up-to-date version of the application.

### 2. Running the Docker Container
After successfully pulling the image, a container was created and run with the following command:
```bash
docker run -d -p 4000:4000 --name games bign8/games:latest
```
Explanation of the command:
- `-d`: Runs the container in detached mode (in the background).
- `-p 4000:4000`: Maps port 4000 of the host to port 4000 of the container.
- `--name games`: Assigns the name "games" to the container for easy reference.
- `bign8/games:latest`: Specifies the image and tag to use for the container.

### 3. Accessing the Application
Once the container was running, the Tic Tac Toe game was accessible via a web browser by navigating to:
```
http://localhost:4000
```
A video recording of the game interface and functionality has been provided to showcase the application in use.


## Project Files
1. **Video**: Demonstrates the game interface accessible at `localhost:4000`.
2. **Screenshot**: Captures the Docker commands executed during the installation process.

## Challenges Faced
- Initial unfamiliarity with Docker commands.
- Ensuring the proper mapping of ports to avoid conflicts with other local applications.

## Learnings
- Gained hands-on experience with Docker's core functionalities, including pulling images and running containers.
- Learned how to map ports between the host and container for seamless application access.
- Understood the importance of container names for better container management.
- Discovered the convenience of deploying lightweight, pre-configured applications through Docker Hub.

## Conclusion
This project successfully demonstrated the use of Docker for deploying a simple yet interactive web-based Tic Tac Toe game. By leveraging Docker's capabilities, the application was quickly set up and made accessible, highlighting the efficiency and portability of containerized solutions.

---
