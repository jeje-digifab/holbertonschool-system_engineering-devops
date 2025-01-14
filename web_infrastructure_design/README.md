### README Summary

#### 0. Simple Web Stack
- **Objective**: Design a one-server web infrastructure for hosting www.foobar.com.
- **Components**:
  - 1 server
  - 1 web server (Nginx)
  - 1 application server
  - 1 application files (code base)
  - 1 database (MySQL)
  - 1 domain name (foobar.com) configured with a www record pointing to server IP 8.8.8.8
- **Explanation Requirements**:
  - Role of each component (server, domain name, DNS record, web server, application server, database)
  - Communication method between server and user's computer
  - Issues: SPOF, downtime during maintenance, scalability limitations
- **Repository**:
  - GitHub: holbertonschool-system_engineering-devops
  - Directory: web_infrastructure_design
  - File: 0-simple_web_stack

#### 1. Distributed Web Infrastructure
- **Objective**: Design a three-server web infrastructure for hosting www.foobar.com.
- **Components**:
  - 2 additional servers
  - 1 web server (Nginx)
  - 1 application server
  - 1 load-balancer (HAproxy)
  - 1 set of application files (code base)
  - 1 database (MySQL)
- **Explanation Requirements**:
  - Reason for adding each component
  - Load balancer distribution algorithm
  - Active-Active vs. Active-Passive setup
  - Primary-Replica (Master-Slave) database cluster
  - Differences between Primary and Replica nodes
  - Issues: SPOF, security (no firewall, no HTTPS), no monitoring
- **Repository**:
  - GitHub: holbertonschool-system_engineering-devops
  - Directory: web_infrastructure_design
  - File: 1-distributed_web_infrastructure

#### 2. Secured and Monitored Web Infrastructure
- **Objective**: Design a secured, encrypted, and monitored three-server web infrastructure for hosting www.foobar.com.
- **Components**:
  - 3 firewalls
  - 1 SSL certificate for HTTPS
  - 3 monitoring clients (data collector for Sumologic or other monitoring services)
- **Explanation Requirements**:
  - Reason for adding each component
  - Role of firewalls
  - Importance of HTTPS
  - Purpose of monitoring
  - Data collection method by monitoring tool
  - Monitoring web server QPS
  - Issues: SSL termination at load balancer, single MySQL server for writes, servers with identical components
- **Repository**:
  - GitHub: holbertonschool-system_engineering-devops
  - Directory: web_infrastructure_design
  - File: 2-secured_and_monitored_web_infrastructure

#### 3. Scale Up
- **Objective**: Scale up the web infrastructure by adding components and splitting responsibilities.
- **Components**:
  - 1 additional server
  - 1 additional load-balancer (HAproxy) configured as a cluster
  - Separate servers for web server, application server, and database
- **Explanation Requirements**:
  - Reason for adding each component
- **Repository**:
  - GitHub: holbertonschool-system_engineering-devops
  - Directory: web_infrastructure_design
  - File: 3-scale_up

This summary provides an overview of the tasks and their requirements for the web infrastructure design project.