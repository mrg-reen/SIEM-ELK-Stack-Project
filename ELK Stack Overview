# Summary of ELK Stack Deployment and Troubleshooting

## Overview
This project's goal is to set up ELK stack for future logging and security lab work and target Windows, MacOS and Linux endpoints with the help of filebeat.

Step 1: Ubuntu ELK Stack Installation (Server-Side)
Added elasticsearch repo: 
  - wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -
  - sudo apt-add-repository "deb https://artifacts.elastic.co/packages/8.x/apt stable main"
  - sudo apt update
  - sudo apt install elasticsearch kibana logstash
Configured elasticsearch.yml:
  - disabled all xpack security features (will configure this once I make expand to mature network infrastructure.)
  - set discovery.type to single-node
  - uncommented and set http.port to 9200
  - set network-host to 127.0.0.1, kee[ing it only accessible to localhost.
(Make sure you allow port 9200, 5601, and 5044 on ufw)

Configured kibana.yml:
  - set server.port to 5601
  - set server.host to 0.0.0.0
  - elasticsearch.hosts set to "http://localhost:9200"
  - keep everything else commented

Configured logstash.yml:
  - Make sure pipeline.ecs_compatibility is disabled. 

## Lessons Learned
- discovery.type is not added to the elasticsearch.yml by default, this must be added for single-node.

---


- Future documentation - Work in Progress
