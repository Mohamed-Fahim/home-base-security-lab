# Home Base Security Lab

## Overview

Welcome to the Home Base Security Lab repository! This project aims to provide a comprehensive setup for practicing cybersecurity monitoring and incident response using Docker and Virtualbox for Wazuh, TheHive, Elasticsearch, and Kibana.

## About ME
   As a Computer Science graduate with a passion for cybersecurity, I've developed this home base lab to deepen my expertise and prepare for a career transition into a Security Operations Center (SOC) as a Tier 1 Analyst. This repository showcases my hands-on experience with essential security tools like Wazuh, TheHive, Elasticsearch, and Kibana. Through this project, I aim to enhance my skills in threat detection, incident response, and security monitoring, laying a strong foundation for my career in cybersecurity.

## Tools
   Docker Desktop
   Virtual Box
   Wazuh
   Thehive
   Elasticsearch
   Kibana

## Setup Instructions

### Wazuh

1. **Download and Import Wazuh Virtual Appliance**
   - Download the Wazuh .ova file.
   - Import the .ova file into VirtualBox or your preferred virtualization platform.
   - Start the Wazuh virtual machine.

2. **Configure Wazuh**
   - Access the Wazuh Manager’s web interface (`https://<Wazuh-VM-IP>`) and follow the setup wizard.
   - Configure network settings, registration with the Wazuh API, and integration with Elasticsearch.

### TheHive

1. **Run TheHive Docker Container**
   - Install Docker Desktop from [Docker Hub](https://www.docker.com/products/docker-desktop) if not already installed.
   - Open Docker Desktop and navigate to the "Containers/Apps" section.

2. **Pull and Start TheHive Container**
   - Click on "Pull" and search for `thehiveproject/thehive:latest`.
   - After pulling the image, click on "Run" and configure with the following settings:
     - **Ports**: Map port `9000` on the container to port `9000` on your host machine.
     
3. **Access TheHive**
   - Open a web browser and navigate to `http://localhost:9000`.
   - Complete the initial setup to configure admin credentials and database connection.

### Elasticsearch

1. **Run Elasticsearch**
   - Download and extract Elasticsearch from [Elastic](https://www.elastic.co/downloads/elasticsearch).
   - Navigate to the Elasticsearch directory and start Elasticsearch:
     ```bash
     cd elasticsearch-x.y.z/
     ./bin/elasticsearch
     ```

2. **Verify Elasticsearch**
   - Open a web browser and go to `http://localhost:9200` to verify Elasticsearch is running.

### Kibana

1. **Run Kibana**
   - Download and extract Kibana from [Elastic](https://www.elastic.co/downloads/kibana).
   - Navigate to the Kibana directory and start Kibana:
     ```bash
     cd kibana-x.y.z/
     ./bin/kibana
     ```

2. **Access Kibana**
   - Open a web browser and navigate to `http://localhost:5601` to access the Kibana dashboard.

## SIEM
  
<img src="https://img.shields.io/badge/-Wazuh-1E90FF?style=flat-square&logo=Wazuh&logoColor=white" />   <img src="https://img.shields.io/badge/-TheHive-FFA500?style=flat-square&logo=Docker&logoColor=white" /> <img src="https://img.shields.io/badge/-Elasticsearch-005571?style=flat-square&logo=Elasticsearch&logoColor=white" /> <img src="https://img.shields.io/badge/-Kibana-FF69B4?style=flat-square&logo=Kibana&logoColor=white" />

### VirtualBox

<img src="https://img.shields.io/badge/-VirtualBox-183A61?style=flat-square&logo=VirtualBox&logoColor=white" />

### Docker

<img src="https://img.shields.io/badge/-Docker%20Desktop-2496ED?style=flat-square&logo=Docker&logoColor=white" />



