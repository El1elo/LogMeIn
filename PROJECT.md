# Log Me In project


![Log Me In project](https://cyber-fullstack-assets.s3.amazonaws.com/M07-Network_Security/Project/src/LogMeIn.png)

Log Me In project

🎯 Goal
Design, implement, and document both a resilient network infrastructure and a secure CI/CD pipeline for LogMeIn's log aggregation platform. The network infrastructure must support high availability, segmentation, monitoring, and secure data flows between international branches. The CI/CD pipeline will automate testing and deployment of a simple log-generating application (frontend, backend, and database).

🧠 Context
You are hired as both a Network and Systems Engineer and a DevOps Engineer by LogMeIn, a French startup specializing in log aggregation. The company is expanding internationally and needs:

A robust and secure network connecting multiple branches worldwide for secure log transmission.
A modernized development and deployment process for their application through an automated CI/CD pipeline.
📌 Project Requirements: Part 1 – Network Infrastructure (GNS3 Simulation)
TIP
As a reminder, for convenience, you can use the GNS3 server hosted on our infrastructure to complete this exercise.

Start the remote server if it's not already done :

Your lab is ready to launch!
A new lab environment will be provisioned for you. This may take a few moments.

Start Lab
Feel free to refer to the GNS3 installation guide presented on the second day of this module ("Network Adressing") 🙂

Build a simulated network infrastructure on GNS3 that meets the following objectives:

✅ Network Redundancy:

Implement Link Aggregation Control Protocol (LACP) to prevent link failures and ensure continuous availability.

✅ Traffic Segmentation:

Configure VLANs to logically separate network traffic for improved security and performance.

✅ IP Addressing:

Use Variable Length Subnet Masking (VLSM) to efficiently allocate IP addresses for current and future needs.

✅ Secure Database Access:

Design access controls and network segmentation to protect the centralized logging database.

✅ Monitoring:

Deploy and configure Zabbix to monitor network devices, servers, and application components.

✅ Secure Remote Connectivity:

Set up VPN tunnels for international branches to securely forward logs to headquarters.

📑 Deliverables
Network Infrastructure Deliverables
Deliverable	Description
📄 Network Documentation	Architecture diagrams, VLAN and IP addressing plans, redundancy and VPN setup, security measures
🛠️ GNS3 Network Simulation	Configured topology simulating LACP, VLANs, VLSM, VPN, and Zabbix monitoring
✅ Evaluation Criteria
Network Infrastructure Evaluation Criteria
Axis	Criteria
Network Redundancy	Effective use of LACP and resilient network design
Traffic Segmentation	Correct VLAN setup to isolate traffic streams
IP Addressing	Proper use of VLSM for IP space optimization
Security	Robust VPN connectivity and secure database access
Monitoring	Zabbix deployed and configured to monitor network and app components
🛠️ Tools You May Use
Network Infrastructure Tools
Network Simulation: GNS3, Cisco IOS
VPN: Any VPN Solution
Monitoring: Zabbix
📌 Project Requirements: Part 2 – CI/CD Pipeline & Application
You are now acting as a DevOps Engineer for LogMeIn. The company has an existing application with a frontend and backend, but lacks proper automation and deployment practices.

They provide you with the code for the frontend and backend (download it from the resources). You will find a README.md file explaining how to run the application locally and some instructions left by the developers (aaah! we love our developers!).

Your goal is to design, implement, and document a secure CI/CD pipeline for the LogMeIn application, ensuring automated testing, deployment, and production readiness.

✅ Source Code Management and Dockerization

GitHub repository with frontend and backend code
Missing Dockerfile for the backend and the docker-compose file to deploy the application (running frontend, backend and database)
✅ CI Pipeline

Automated testing of backend code
Code scanning analysis
✅ CD Pipeline

Automated deployment to staging/production if CI pipeline is successful
Push the docker image to the container registry
✅ Infrastructure

Docker Swarm cluster (1 manager, 2 workers) running on whatever infrastructure you want (virtual machines, cloud, etc.)
Database accessibility for every backend instance
✅ Security Measures

Network security
Access control
📑 Deliverables
Deliverable	Description
📄 Technical Documentation	Includes: Architecture design, pipeline workflow, security measures, deployment strategy and security measures
🛠️ CI/CD Implementation	Working GitHub repository with GitHub Actions
🐳 Docker Configuration	Dockerfile and docker-compose files
🎥 Demo Video	Video demonstration of the CI/CD pipeline and production deployment
✅ Evaluation Criteria
Axis	Criteria
Containerization	Your Docker containers must work consistently across all environments (local, CI/CD, production).
CI/CD Pipeline	Your pipeline must automatically test, build, and deploy your application when code changes.
Infrastructure	Your Docker Swarm cluster must handle dynamic scaling and ensure high availability.
Security	Your deployment must follow security best practices and protect against unauthorized access.
🛠️ Tools You May Use
You can use any tool you want. Here are some suggestions:

CI/CD: GitHub Actions, Jenkins, GitLab CI
Container: Docker, Docker Compose, Docker Swarm
Code Quality: SonarQube, ESLint, Pylint, Trivy, Black, Flake8
Monitoring: Prometheus, Grafana
Load Balancing: Nginx, Traefik
Version Control: Git, GitHub
Project Management: GitHub Projects, Trello
📣 Final Word
This project allows you to demonstrate your skills in two critical domains: building a secure, scalable network infrastructure and automating deployment through CI/CD pipelines. Take this opportunity to build a solid foundation that will empower LogMeIn's international growth!
