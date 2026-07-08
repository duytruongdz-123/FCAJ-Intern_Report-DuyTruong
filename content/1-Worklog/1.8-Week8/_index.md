---
title: "Week 8 Worklog"
date: 2026-06-08
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---


### Week 8 Objectives:
* Provision minimal access security policies for external cloud data retrieval.
* Formulate spike load test profiles and establish direct streaming endpoints from local agents to Grafana Cloud.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Navigate to the AWS IAM Console to construct a programmatic access identity | 06/08/2026 | 06/08/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Attach the managed system policy `CloudWatchReadOnlyAccess` to enforce the principle of least privilege | 06/09/2026 | 06/09/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Write an aggressive JavaScript test script (`stress_test.js`) in `k6` to cycle sudden concurrent user traffic | 06/10/2026 | 06/10/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Extract Prometheus Remote Write credentials (URL, User ID, and Instance Password Tokens) | 06/11/2026 | 06/11/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Configure local environment system variables and execute the load generation engine | 06/12/2026 | 06/12/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |

### Week 8 Achievements:
* Enforced secure data integration pipelines between distributed platforms using audited IAM policies.
* Built standardized high-throughput API automation scripts to validate platform resiliency parameters.
* Successfully piped decoupled open-source load metrics straight into unified cloud dashboards.

---

### Week 8 Evidence Images

#### 1. Successfully Creating a New IAM User Identity inside AWS Management Console
![Successfully created IAM user](/images/1-Worklog/Week8/Picture35.png)

#### 2. Attaching CloudWatchReadOnlyAccess Permission Policy Directly to the Created IAM User
![Attaching CloudWatchReadOnlyAccess policy](/images/1-Worklog/Week8/Picture36.png)

#### 3. Generating and Retrieving AWS Programmatic Access Keys (Access Key ID & Secret Access Key)
![Retrieving AWS Access Keys](/images/1-Worklog/Week8/Picture37.png)

#### 4. Integrating and Successfully Querying AWS CloudWatch Data Source inside Grafana Cloud
![Successfully connected CloudWatch Data Source in Grafana](/images/1-Worklog/Week8/Picture38.png)

#### 5. Configuring Performance Monitoring Dashboard for ALB Response Times and CPU/RAM Utilization
![Configuring performance metrics dashboards](/images/1-Worklog/Week8/Picture39.png)

#### 6. Inspecting Hosted Prometheus Instance Details and Query Endpoints on Grafana Labs
![Inspecting Prometheus instance details on Grafana](/images/1-Worklog/Week8/Picture40.png)

#### 7. Reviewing Prometheus Remote Write Endpoints, Instance IDs, and Password API Tokens
![Reviewing Remote Write Endpoints information](/images/1-Worklog/Week8/Picture41.png)

#### 8. Final Live Dashboard Tracking Database Connections and K6 Load Testing Performance Metrics
![Finalized dashboard tracking K6 load test and RDS connections](/images/1-Worklog/Week8/Picture42.png)

#### 9. Go to the AWS office
![Group Meeting](/images/1-Worklog/Week8/1206_meeting_w9.JPG)