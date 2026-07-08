---
title: "Week 11 Worklog"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---


### Week 11 Objectives:
* Create a dedicated high-priority visualization layout named "Stress Test Panel".
* Map and evaluate full-stack resource interaction benchmarks during high-stress automation events.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Initialize a structural priority Row section titled "Stress Test Panel" | 06/29/2026 | 06/29/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 3 | - Formulate the Network Ingress Panel using the `AWS/ApplicationELB` namespace | 06/30/2026 | 06/30/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 4 | - Engineer the Failure Tracking Panel monitoring error metrics | 07/01/2026 | 07/01/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Construct the Core Container Compute Panel for live ECS cluster services | 07/02/2026 | 07/02/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Develop the Persistence Panel and trigger the K6 engine script audit | 07/03/2026 | 07/03/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |

### Week 11 Achievements:
* Built an organized infrastructure dashboard row optimized for evaluating traffic spikes.
* Achieved full-stack visibility by capturing network load, container memory, and database metrics.
* Audited platform performance metrics under heavy user load to guide auto-scaling designs.

---

### Week 11 Evidence Images

#### 1. Overview Dashboard Representing Baseline System Metrics (ALB Throughput, Error Rate, ECS Compute, and RDS Connections) Before Testing
![System overview dashboard before stress testing](/images/1-Worklog/Week11/Picture46.png)

#### 2. Executing Command-Line Stress Test Script (`stress-test.js`) Using K6 Framework with a Peak of 200 Virtual Users (VUs)
![Executing K6 stress test on terminal](/images/1-Worklog/Week11/Picture47.png)

#### 3. Real-time Dashboard Analytics Capturing Significant Spikes in ALB Throughput and ECS Fargate CPU Utilization Under Load
![System metrics dashboard visualization during active load testing](/images/1-Worklog/Week11/Picture48.png)

#### 4. Group Meeting
![Group Meeting](/images/1-Worklog/Week11/Picture5.jpg)