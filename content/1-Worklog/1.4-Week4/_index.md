---
title: "Week 4 Worklog"
date: 2026-10-30
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

## Daily Worklog — Friday, 30 October 2026

**Topic:** Learning and practicing Amazon RDS, Amazon Lightsail, Amazon Lightsail Containers, and EC2 Auto Scaling.

### Activities

- Attended the internship office and studied four core tutorials in the First Cloud Journey learning path covering managed databases, simplified cloud compute/containers, and application scaling:
  - **Amazon RDS:** Studied relational database management on AWS; practiced preparing VPC subnets, DB Subnet Groups, and Security Groups, launching an Amazon RDS database instance, connecting a web application running on EC2 to RDS, and configuring automated backups and manual snapshots.
  - **Amazon Lightsail:** Explored deploying virtual private servers and managed databases using Lightsail OS and Application Blueprints (WordPress, PrestaShop, and Akaunting); practiced configuring Static IPs, firewall rules, manual/automatic snapshots, instance vertical scaling, and monitoring alarms.
  - **Amazon Lightsail Containers:** Studied simplified container orchestration with Lightsail Container Service; learned how to select container capacity (power and scale), deploy Docker container images, and publish applications via built-in HTTPS endpoints.
  - **EC2 Auto Scaling:** Studied high-availability and fault-tolerant web architectures combining VPC, RDS, Custom AMIs, Launch Templates, Application Load Balancers (ALB) with Target Groups, and EC2 Auto Scaling Groups (ASG); explored manual scaling, scheduled scaling, dynamic scaling with CloudWatch metrics, and predictive scaling.

### Results and lessons learned

- Understood how to decouple the database tier from the compute tier using Amazon RDS and secure communication between EC2 and RDS via dedicated Security Groups and DB Subnet Groups.
- Recognized when to choose Amazon Lightsail and Lightsail Containers for rapid, predictable-cost deployments of web applications and containerized workloads versus full VPC/EC2/ECS setups.
- Grasped how Elastic Load Balancing (ALB) and EC2 Auto Scaling work together across multiple Availability Zones to maintain application availability and automatically adjust capacity to workload demand.

### References

1. [Database Essentials with Amazon Relational Database Service (RDS)](https://000005.awsfcaj.com/)
2. [Simplified Computing with Amazon Lightsail](https://000045.awsfcaj.com/)
3. [Container Deployment with Amazon Lightsail Containers](https://000046.awsfcaj.com/)
4. [Scaling Applications with EC2 Auto Scaling](https://000006.awsfcaj.com/)

---

## Weekly Worklog — 26–30 October 2026

### Weekly objectives

- Learn how to provision, secure, and back up managed relational databases with Amazon RDS.
- Explore simplified compute and container deployment options using Amazon Lightsail and Lightsail Containers.
- Understand how to design and deploy scalable, highly available web applications using Elastic Load Balancing and Amazon EC2 Auto Scaling.

### Activities completed

| Date | Activity | Reference |
|---|---|---|
| 30 October 2026 | Studied and practiced deploying an Amazon RDS instance, configuring DB Subnet Groups and Security Groups, connecting an EC2 app, and managing backups. | [Amazon RDS](https://000005.awsfcaj.com/) |
| 30 October 2026 | Worked through the Amazon Lightsail workshop to deploy application blueprints, attach Static IPs, create snapshots, scale instances, and configure alarms. | [Amazon Lightsail](https://000045.awsfcaj.com/) |
| 30 October 2026 | Learned how to deploy and manage containerized web applications with public endpoints using Amazon Lightsail Containers. | [Lightsail Containers](https://000046.awsfcaj.com/) |
| 30 October 2026 | Studied and practiced building a scalable web tier using Launch Templates, Application Load Balancers, and EC2 Auto Scaling policies. | [EC2 Auto Scaling](https://000006.awsfcaj.com/) |

### Weekly results

- Successfully expanded knowledge from single-instance compute to multi-tier architectures combining EC2, ALB, and Amazon RDS.
- Gained practical familiarity with Amazon Lightsail for both blueprint-based virtual servers and containerized workloads.
- Understood the differences and use cases among manual, scheduled, dynamic (CloudWatch-driven), and predictive scaling strategies in EC2 Auto Scaling.
- Practiced systematic cleanup of multi-component environments (Auto Scaling Groups, Load Balancers, Target Groups, RDS instances, and Lightsail services) to control cloud spend.

### Areas for further study

- Review Multi-AZ deployment options and read replicas in Amazon RDS for higher database availability and read performance.
- Practice fine-tuning CloudWatch alarms and dynamic scaling policies to avoid rapid scale-in/scale-out thrashing (cooldown periods).
- Compare Lightsail Containers with Amazon ECS and AWS Fargate for more complex container orchestration requirements.
