---
title: "Week 10 Worklog"
date: 2026-06-22
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Week 10 Objectives:
* Link AWS CloudWatch infrastructure data namespaces directly into Grafana Cloud.
* Build layered core monitoring panels and implement automated rule thresholds for email alerts.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Generate system credentials for operational AWS access | 06/22/2026 | 06/22/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Add a new CloudWatch Data Source inside Grafana Cloud | 06/23/2026 | 06/23/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 4 | - Construct visualization panels querying `AWS/EC2`, `AWS/ApplicationELB`, and `ECS/ContainerInsights` | 06/24/2026 | 06/25/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Create an administrative Contact Point in Grafana Alerting | 06/26/2026 | 06/26/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Define Alert Rules for request counts and set evaluation resolutions | 06/27/2026 | 06/27/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |

### Week 10 Achievements:
* Established end-to-end data syncing pipelines by configuring certified CloudWatch integrations.
* Designed an executive full-stack infrastructure panel spanning computing, networking, and databases.
* Enabled automated system self-auditing by implementing localized warning rules.

---

### Week 10 Evidence Images

#### 1. Creating an OTLP Token (otlp-token) under Cloud Access Policies Section on Grafana Cloud Dashboard
![Creating otlp-token on Grafana Cloud](/images/1-Worklog/Week10/Picture43.png)

#### 2. Managing Active Status and Security Credentials for AWS IAM Account Access Keys
![Managing AWS IAM Access Key credentials](/images/1-Worklog/Week10/Picture44.png)

#### 3. Live Analytical Monitoring Dashboard Representing Real-time CPU Utilization, Request Count, and RAM Metrics
![Live monitoring dashboard for CPU, Requests, and RAM](/images/1-Worklog/Week10/Picture45.png)