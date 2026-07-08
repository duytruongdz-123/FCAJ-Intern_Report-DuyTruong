---
title: "Week 5 Worklog"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---


### Week 5 Objectives:

* Integrate AWS monitoring metrics securely into Grafana Cloud.
* Design an executive infrastructure dashboard to supervise computing, networking, and data tiers in parallel.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Research secure IAM cross-cloud authorization protocols following the principle of least privilege | 05/18/2026 | 05/18/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Create a dedicated IAM User on AWS and attach the managed policy `CloudWatchReadOnlyAccess` <br> - Generate secure AWS Access Keys for external integration | 05/19/2026 | 05/19/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Configure AWS as an external CloudWatch data source inside the Grafana Cloud console using the IAM credentials | 05/20/2026 | 05/20/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Design ingress and core computation panels covering ALB Response Time, ALB Throughput, and AWS ECS Fargate CPU/RAM Utilization metrics | 05/21/2026 | 05/22/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Develop persistence layer monitoring panels focused on Amazon RDS Database Connections and related storage load indicators | 05/22/2026 | 05/22/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |


### Week 5 Achievements:

* Implemented secure cloud authorization boundaries by isolating data visibility to read-only scopes via IAM policies.
* Connected the AWS CloudWatch metrics pipeline directly into the centralized Grafana Cloud environment.
* Successfully constructed an Infrastructure Dashboard visualizing critical stack tiers (ALB, ECS Fargate, and Amazon RDS) side-by-sides.
* Achieved real-time scannability over hardware allocations and system metrics, simplifying platform bottleneck identification.

---

### Week 5 Evidence Images

#### 1. Preparing an IAM Access Key on AWS
![Configuring source code storage on Amazon S3](/images/1-Worklog/Week5/Picture10.png)

#### 2. Integrating AWS CloudWatch into Grafana
![Creating CloudFront Distribution for the system](/images/1-Worklog/Week5/Picture11.png)

#### 3. Configure the three charts on Grafana
![Successfully configured Route 53 hosted zone records](/images/1-Worklog/Week5/Picture12.png)