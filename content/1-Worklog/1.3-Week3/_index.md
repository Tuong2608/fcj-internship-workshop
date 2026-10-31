---
title: "Week 3 Worklog"
date: 2026-10-23
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

## Daily Worklog — Friday, 23 October 2026

**Topic:** Reviewing Amazon VPC and Amazon EC2; learning IAM Roles for EC2 and AWS Cloud9.

### Activities

- Attended the internship office to review and consolidate previously studied networking and compute modules, while continuing with the next two tutorials in the First Cloud Journey learning path:
  - **Amazon VPC (Review & Deep Dive):** Reviewed VPC design across public and private subnets, route tables, Internet Gateways, and NAT Gateways; explored VPC Security Groups, Network ACLs, VPC Resource Map, Reachability Analyzer, Systems Manager Session Manager, VPC Flow Logs, and Site-to-Site VPN concepts.
  - **Amazon EC2 (Review & Practice):** Reviewed launching and connecting to Windows Server and Amazon Linux 2023 instances (via RDP and SSH), deploying web stacks (LAMP, XAMPP, Node.js), managing EBS snapshots and Custom AMIs, recovering instance access, and applying IAM policies for EC2 cost and usage governance.
  - **IAM Roles for EC2:** Studied instance profiling and how to grant applications running on EC2 secure access to AWS services (such as Amazon S3) using temporary credentials via IAM Roles instead of hard-coding IAM User access keys.
  - **AWS Cloud9:** Explored the browser-based Cloud IDE, setting up a Cloud9 development environment on EC2, using the integrated terminal, and running AWS CLI commands directly from the IDE.

### Results and lessons learned

- Strengthened understanding of VPC network isolation, routing between public and private subnets, and troubleshooting connectivity.
- Consolidated practical skills in configuring EC2 instances, creating backups with EBS snapshots and AMIs, and enforcing fine-grained IAM restrictions.
- Understood why attaching an IAM Role (Instance Profile) to EC2 is a critical security best practice compared to embedding long-term access keys in application code.
- Gained familiarity with AWS Cloud9 as a convenient cloud-based development and CLI management environment.

### References

1. [Networking Essentials with Amazon Virtual Private Cloud (VPC)](https://000003.awsfcaj.com/)
2. [Compute Essentials with Amazon Elastic Compute Cloud (EC2)](https://000004.awsfcaj.com/)
3. [Instance Profiling with IAM Roles for EC2](https://000048.awsfcaj.com/)
4. [Cloud Development with AWS Cloud9](https://000049.awsfcaj.com/)

---

## Weekly Worklog — 19–23 October 2026

### Weekly objectives

- Review and deepen practical knowledge of Amazon VPC and Amazon EC2 architectures.
- Learn how to securely grant AWS service permissions to EC2 instances using IAM Roles.
- Get familiar with cloud-based development workflows using AWS Cloud9.

### Activities completed

| Date | Activity | Reference |
|---|---|---|
| 23 October 2026 | Reviewed and practiced Amazon VPC networking components, NAT Gateway, security controls, and connectivity tools at the office. | [Amazon VPC](https://000003.awsfcaj.com/) |
| 23 October 2026 | Reviewed Amazon EC2 instance deployment (Linux/Windows), EBS snapshots, Custom AMIs, and IAM cost governance policies. | [Amazon EC2](https://000004.awsfcaj.com/) |
| 23 October 2026 | Studied and practiced granting applications on EC2 access to AWS services via IAM Roles (Instance Profiles). | [IAM Roles for EC2](https://000048.awsfcaj.com/) |
| 23 October 2026 | Explored creating and using a browser-based development environment with AWS Cloud9 and integrated AWS CLI. | [AWS Cloud9](https://000049.awsfcaj.com/) |

### Weekly results

- Consolidated foundational knowledge of VPC networking and EC2 compute operations through review and hands-on practice at the office.
- Mastered the security best practice of using IAM Roles for EC2 to eliminate hard-coded credentials when interacting with services like Amazon S3.
- Learned how to provision and utilize AWS Cloud9 for writing code and executing AWS CLI commands in the cloud.
- Prepared a solid networking, compute, and security foundation for upcoming database, container, and auto-scaling modules.

### Areas for further study

- Practice troubleshooting network paths between private subnets and AWS services using VPC Reachability Analyzer and Session Manager.
- Continue applying least-privilege IAM Role policies when integrating EC2 with other AWS services.
- Ensure all lab resources (NAT Gateways, Elastic IPs, EC2 instances, Cloud9 environments) are cleaned up after practice to prevent unintended charges.
