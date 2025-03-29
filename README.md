# cyberlab-infra

Infrastructure-as-Code (IaC) project to deploy a local cybersecurity lab using Docker. It includes Damn Vulnerable Web Application (DVWA), a deliberately vulnerable web application designed for practicing penetration testing techniques in a safe and controlled environment.

## Description

This project uses Docker Compose to automate the setup of DVWA and a MySQL database. It allows users to launch a vulnerable web application locally, ideal for training in ethical hacking and web application security.

## What is DVWA?

DVWA (Damn Vulnerable Web Application) is a PHP/MySQL web application intentionally designed with security flaws. It is commonly used to learn and test common web vulnerabilities including:

- SQL Injection
- Cross-site Scripting (XSS)
- Command Injection
- Brute Force Attacks
- CSRF (Cross-Site Request Forgery)

DVWA allows users to practice offensive security techniques and understand how vulnerabilities can be exploited.

## Requirements

- Docker Desktop (Windows, macOS, or Linux)
- Git
- Internet connection (to pull Docker images)

## Usage

1. Clone the repository:

```bash
git clone https://github.com/dekapala/cyberlab-infra.git
cd cyberlab-infra
```

2. Start the lab:

```bash
docker compose up -d
```

3. Access DVWA in your browser:

```bash
http://localhost:8080
```
4. Inside the application, click "Create/Reset Database" to initialize the MySQL connection.

Security Notice
This project is intended for local use only. The DVWA container is intentionally vulnerable and should never be exposed to the internet or a production environment.

To keep your machine safe:

Only run this lab in isolated or personal environments

Shut it down after use:
```bash
docker compose down
```
Do not connect DVWA to public or shared networks

Author
Gabriel Palazzini
https://github.com/dekapala

License
This project is released under the MIT License. DVWA is distributed under its own open-source license.