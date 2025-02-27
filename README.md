# Java Web Application Deployment with Vagrant, Nagios, and Docker
## Introduction
This project demonstrates how to deploy a Java-based web application across multiple virtual machines (VMs) using Vagrant. It includes manual setup, automation using Bash scripts, health monitoring with Nagios, and containerization using Docker. The goal is to showcase DevOps skills by creating a scalable, monitored, and containerized deployment.

## Purpose
To practice and demonstrate DevOps concepts, including deployment automation, system health monitoring, and containerization, in a simulated multi-VM environment.

## Tools
- Vagrant
- VirtualBox
- Tomcat
- Nginx
- RabbitMQ
- Memcached
- MariaDB
- Maven
- Git Bash
- Nagios
- Docker
- Docker Compose

## Steps
### 1. Manual Deployment
- Configured VMs for:
  - **VM1**: Tomcat for hosting the Java application.
  - **VM2**: Nginx as a reverse proxy.
  - **VM3**: MariaDB for the database.
  - **VM4**: Memcached for caching.
  - **VM5**: RabbitMQ for message queuing.
- Deployed the application manually on these VMs.

### 2. Automation with Bash Scripts
- Automated the setup process, including:
  - Installing required packages.
  - Configuring services (e.g., Tomcat, Nginx).
  - Setting up environment variables.

### 3. Health Monitoring
- Added Nagios to monitor:
  - Application uptime.
  - VM resource usage (CPU, RAM).
  - Network availability.

### 4. Containerization with Docker
- Containerized the Java web application using Docker.
- Created a `Dockerfile` to define the application environment.
- Used `docker-compose.yml` to orchestrate the multi-container application setup, including:
  - **Tomcat**: To host the Java application.
  - **Nginx**: As a reverse proxy.
  - **MariaDB**: For the database.
  - **Memcached**: For caching.
  - **RabbitMQ**: For message queuing.

## What I Learned
This project provided valuable learning experiences across several areas of DevOps:
1. **Efficient VM Creation**: 
   - Learned how to create and configure multiple virtual machines using a single `Vagrantfile`, significantly reducing the time and effort required for manual configuration.
2. **Using `expect` in Bash Scripts**: 
   - Gained hands-on experience with the `expect` command in Bash scripts to manage interactive command outputs and automate responses, further streamlining the automation process.
3. **Monitoring and Troubleshooting**: 
   - Acquired skills in setting up and using Nagios to monitor the health of virtual machines and identify potential issues early.
   - Discovered and resolved a compatibility issue between the Java application (developed with Java 11) and the virtual machines running Java 17, which initially prevented the website from functioning.
4. **Containerization**:
   - Learned how to containerize a Java web application using Docker.
   - Gained experience with Docker Compose to manage multi-container applications efficiently.

These learnings enhanced my understanding of automation, system compatibility, monitoring, and containerization in a multi-VM environment.
