# Task 7: Netdata Monitoring on Ubuntu EC2

## Objective
Deployed Netdata, a lightweight, open-source monitoring tool, on an AWS EC2 instance running Ubuntu 22.04 to monitor system and application performance metrics. Documented the process for submission as part of a DevOps internship task.

## Tools Used
- **AWS EC2**: Hosted the Ubuntu 22.04 instance
- **Docker**: Ran the Netdata container
- **Netdata**: Monitored CPU, memory, disk, and Docker container metrics
- **GitHub**: Stored deliverables and documentation

## Implementation Steps

### 1. Launched an EC2 Instance
- Created Ubuntu 22.04 LTS instance (t2.micro) in AWS
- Security group configured to allow:
  - Port 22 (SSH)
  - Port 80 (HTTP)
  - Port 19999 (Netdata)
- Connected via SSH:
  ```bash
  ssh -i task7-key.pem ubuntu@<public-ip>
