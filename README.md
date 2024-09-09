# Building a (SOC) on VULTR with ELK Stack + Fleet Server + Real-Time Threat Detection & Incident Response

<br>
<br>

<img src="https://github.com/bayulus/SOC-ELK-IR-ThreatDetection/blob/main/img/mydfir30days.drawio.png" >

# Introduction

This project is centered around building a comprehensive Security Operations Center (SOC) environment in a cloud-based infrastructure, leveraging industry-standard tools and technologies. The goal is to create a simulated network setup hosted on VULTR, where both defensive and offensive security techniques can be practiced. The overall objective is to develop the skills necessary for identifying and responding to security threats. By using tools like Elastic Agents, Elasticsearch, and Kibana, this project will provide hands-on experience in monitoring logs, identifying threats, and responding to real incidents. The ultimate goal is to build a thorough understanding of SOC operations, log analysis, and incident response in a cloud environment.

# Here's a Highlight of the steps I'll be taking as Shown In the Image Above:

**1.  Cloud Setup on VULTR:**

  - I created my servers(ELK and Fleet Server) within a Virtual Private Cloud (VPC) on VULTR.

**2. Server Configuration:** 

  - I have a Windows server with RDP enabled and an Ubuntu server with SSH enabled. Additionally, I will set up a Fleet server, which is crucial for managing Elastic Agents and devices across a distributed environment. These agents collect data (like logs or metrics) from endpoints (my Windows and Ubuntu servers) and send them to Elasticsearch for analysis. Enabling RDP will also allow us to monitor events and detect potential threats originating from different locations, ensuring better visibility and response to actions by threat actors.

**3. Elastic & Kibana Setup:**

  - Logs collected by the Elastic Agents will be analyzed by Elastic & Kibana(Dashboards). If any suspicious or malicious activity is detected, alerts will be sent to the ticketing system based on the analysis results.

**4.  SOC Analyst & Attacker Roles:**

  - The SOC Analyst Focuses on defensive security, this system will be used to analyze the logs and determine whether alerts are true positives, false positives, or benign true positives (B-TP) needing further action. The Attackers Laptop focuses on offensive security, this system will be used to perform various attacks (such as brute force) on the Windows and Ubuntu servers.
