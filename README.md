# SIEM Deployment with ELK Stack (Elasticsearch, Logstash, Kibana)

## Overview
This project implements a **Security Information and Event Management (SIEM)** system using **ELK Stack** to centralize security logs from multiple endpoints.

## Technologies Used
- **Elasticsearch** for log storage and searching
- **Kibana** for visualization and alerting
- **Filebeat & Winlogbeat** for log forwarding from Linux & Windows hosts
- **Multipass VM** for cloud-like infrastructure setup
- **Linux Hardening & Firewall Security (UFW)**

## Security Detections Implemented
**SSH Brute-Force Detection**  
**Privilege Escalation Alerts**  
**Windows Event Monitoring for RDP Logins**  

## Lessons Learned
- Debugging network issues when setting up **Filebeat communication**.
- Optimizing **Elasticsearch performance** for large log ingestion.
- Creating **security rules in Kibana using KQL**.

---
### **Install ELK Stack**
```bash
sudo apt install elasticsearch kibana logstash
```

