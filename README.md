# Java Web Application Deployment with Vagrant and Nagios

## Introduction
This project demonstrates how to deploy a Java-based web application across multiple virtual machines (VMs) using Vagrant. It includes manual setup, automation using Bash scripts, and health monitoring with Nagios. The goal is to showcase DevOps skills by creating a scalable and monitored deployment.

## Purpose
To practice and demonstrate DevOps concepts, including deployment automation and system health monitoring, in a simulated multi-VM environment.

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

## What I Learned
This project provided valuable learning experiences across several areas of DevOps:

1. **Efficient VM Creation**: 
   - Learned how to create and configure multiple virtual machines using a single `Vagrantfile`, significantly reducing the time and effort required for manual configuration.

2. **Using `expect` in Bash Scripts**: 
   - Gained hands-on experience with the `expect` command in Bash scripts to manage interactive command outputs and automate responses, further streamlining the automation process.

3. **Monitoring and Troubleshooting**: 
   - Acquired skills in setting up and using Nagios to monitor the health of virtual machines and identify potential issues early.
   - Discovered and resolved a compatibility issue between the Java application (developed with Java 11) and the virtual machines running Java 17, which initially prevented the website from functioning.

These learnings enhanced my understanding of automation, system compatibility, and monitoring in a multi-VM environment.

