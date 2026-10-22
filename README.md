# aws-web-security-lab
AWS Cloud Security project featuring EC2, Ubuntu, Nginx, AWS WAF, Linux hardening and penetration testing with Kali Linux.


# 🔐 AWS Web Security Project

> Secure deployment of a web application on AWS using Ubuntu, Nginx, AWS WAF and Security Testing with Kali Linux.

> Despliegue seguro de una aplicación web en AWS utilizando Ubuntu, Nginx, AWS WAF y pruebas de seguridad con Kali Linux.

---

# 🇺🇸 English

##  Overview

This project demonstrates the deployment, protection and validation of a web application hosted on AWS.

The infrastructure was built using Amazon EC2 with Ubuntu Server, Nginx as the web server, AWS Security Groups for network filtering and AWS WAF to mitigate common web attacks.

The environment was tested from Kali Linux using penetration testing techniques to validate the implemented security controls.

---

## Objectives

- Deploy a web application on AWS EC2
- Configure Ubuntu Server
- Install and configure Nginx
- Implement AWS Security Groups
- Configure AWS WAF
- Perform security testing
- Document security findings
- Build a practical cloud security portfolio project

---

## Architecture

```text
Internet
   │
   ▼
AWS WAF
   │
   ▼
CloudFront
   │
   ▼
Ubuntu EC2 Instance
   │
   ▼
Nginx Web Server
   │
   ▼
Web Application
```

---

## Technologies Used

- AWS EC2
- Ubuntu Server
- Nginx
- AWS WAF
- AWS Security Groups
- Git & GitHub
- Kali Linux
- Nmap
- UFW Firewall

---

## Security Controls Implemented

### Infrastructure Security

- EC2 deployment
- Public access restriction
- Security Group configuration

### Operating System Security

- System updates
- Linux hardening
- UFW Firewall

### Application Security

- Nginx configuration
- Access control

### Web Protection

- AWS WAF
- SQL Injection protection
- Cross Site Scripting (XSS) protection
- Bad input filtering

---

##  Security Testing

The security validation includes:

### Reconnaissance

- Nmap scan

### Vulnerability Validation

- SQL Injection tests
- XSS tests

### Verification

- WAF response validation
- Access control verification

---

##  Repository Structure

```text
aws-web-security-project/

├── README.md
├── screenshots/
│
├── deployment/
│   ├── ec2-setup.md
│   ├── nginx-config.md
│   └── security-groups.md
│
├── waf/
│   ├── waf-configuration.md
│   └── test-results.md
│
├── pentesting/
│   ├── nmap.md
│   ├── sql-injection.md
│   └── xss-tests.md
│
└── website/
```

---

##  Evidence

Project evidence and screenshots are stored inside the `screenshots` folder.

Examples:

- EC2 creation
- Security Groups
- SSH connection
- Nginx installation
- AWS WAF configuration
- Security testing results

---

##  Skills Demonstrated

- Cloud Security
- AWS Fundamentals
- Linux Administration
- Web Security
- Security Hardening
- AWS WAF Management
- Ethical Hacking
- Penetration Testing
- Documentation

---

##  Future Improvements

- HTTPS with SSL/TLS
- Custom WAF Rules
- AWS CloudWatch Monitoring
- Automated Deployments
- Infrastructure as Code (Terraform)

---

##  Author

John Correa

Software Engineering Student

Cybersecurity Enthusiast

---

# 🇪🇸 Español

##  Descripción General

Este proyecto demuestra el despliegue, protección y validación de una aplicación web alojada en AWS.

La infraestructura fue construida utilizando Amazon EC2 con Ubuntu Server, Nginx como servidor web, Security Groups para el filtrado de red y AWS WAF para mitigar ataques web comunes.

El entorno fue evaluado desde Kali Linux aplicando técnicas de pentesting para validar los controles de seguridad implementados.

---

##  Objetivos

- Desplegar una aplicación web en AWS EC2
- Configurar Ubuntu Server
- Instalar y configurar Nginx
- Implementar Security Groups
- Configurar AWS WAF
- Realizar pruebas de seguridad
- Documentar hallazgos de seguridad
- Construir un proyecto práctico para portafolio

---

## Arquitectura

```text
Internet
   │
   ▼
AWS WAF
   │
   ▼
CloudFront
   │
   ▼
Instancia EC2 Ubuntu
   │
   ▼
Servidor Web Nginx
   │
   ▼
Aplicación Web
```

---

## Tecnologías Utilizadas

- AWS EC2
- Ubuntu Server
- Nginx
- AWS WAF
- AWS Security Groups
- Git y GitHub
- Kali Linux
- Nmap
- Firewall UFW

---

## Controles de Seguridad Implementados

### Seguridad de Infraestructura

- Despliegue en EC2
- Restricción de acceso público
- Configuración de Security Groups

### Seguridad del Sistema Operativo

- Actualización del sistema
- Hardening de Linux
- Firewall UFW

### Seguridad de la Aplicación

- Configuración de Nginx
- Control de acceso

### Protección Web

- AWS WAF
- Protección contra SQL Injection
- Protección contra XSS
- Filtrado de entradas maliciosas

---

## Pruebas de Seguridad

La validación de seguridad incluye:

### Reconocimiento

- Escaneo con Nmap

### Validación de Vulnerabilidades

- Pruebas de SQL Injection
- Pruebas XSS

### Verificación

- Validación de respuestas del WAF
- Verificación de controles de acceso

---

## Estructura del Repositorio

```text
aws-web-security-project/

├── README.md
├── screenshots/
│
├── deployment/
│   ├── ec2-setup.md
│   ├── nginx-config.md
│   └── security-groups.md
│
├── waf/
│   ├── waf-configuration.md
│   └── test-results.md
│
├── pentesting/
│   ├── nmap.md
│   ├── sql-injection.md
│   └── xss-tests.md
│
└── website/
```

---

## Evidencias

Las evidencias del proyecto y capturas de pantalla se almacenan dentro de la carpeta `screenshots`.

Ejemplos:

- Creación de EC2
- Configuración de Security Groups
- Conexión SSH
- Instalación de Nginx
- Configuración de AWS WAF
- Resultados de pruebas de seguridad

---

## Competencias Demostradas

- Seguridad en la Nube
- Fundamentos de AWS
- Administración Linux
- Seguridad Web
- Hardening de Sistemas
- Gestión de AWS WAF
- Ethical Hacking
- Pentesting
- Documentación Técnica

---

## Mejoras Futuras

- HTTPS con SSL/TLS
- Monitoreo con CloudWatch
- Despliegues automatizados
- Infraestructura como código con Terraform

---

## Autor

John Correa

Estudiante de Ingeniería de Software

Apasionado por la Ciberseguridad