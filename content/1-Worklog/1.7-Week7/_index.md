---
title: "Week 7 Worklog"
date: 2026-06-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---



### Week 7 Objectives:

* Instrument Application Performance Monitoring (APM) using the OpenTelemetry standard.
* Gain internal code-level execution telemetry over running web applications on containerized infrastructure without service downtime.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Study OpenTelemetry (OTel) agent injection configurations and OTLP network exporter endpoints | 06/01/2026 | 06/01/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 3 | - Initialize a secure Access Policy and export the encrypted OTLP authentication token on Grafana Cloud | 06/02/2026 | 06/02/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 4 | - Embed OTLP environment variables (`OTEL_EXPORTER_OTLP_ENDPOINT`, `OTEL_EXPORTER_OTLP_HEADERS`) directly into the target AWS ECS Task Definition | 06/03/2026 | 06/03/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Trigger a rolling update execution using the `Force new deployment` feature on the live AWS ECS Service to reload telemetry profiles with zero downtime | 06/04/2026 | 06/04/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Integrate and customize the JVM Micrometer Dashboard (ID: 4701) inside Grafana Cloud <br> - Perform deep real-time code-level analysis over running Java/Spring Boot applications | 06/05/2026 | 06/05/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |


### Week 7 Achievements:

* Standardized distributed logging and telemetry capture using cloud-agnostic OpenTelemetry configurations.
* Successfully mapped secure OTLP tokens into highly available container deployment definitions.
* Maintained infrastructure platform uptime standards by mastering zero-downtime container updating mechanisms.
* Achieved complete diagnostic visibility into runtime app lifecycles via JVM heap memory allocation monitoring and garbage collection trace analytics.

---

### Week 7 Evidence Images

#### 1. Initializing and Setting Up API Token for OpenTelemetry on Grafana Cloud
![Initializing OpenTelemetry API Token](/images/1-Worklog/Week7/Picture25.png)

#### 2. Appending and Copying Generated OpenTelemetry Exporter Environment Configurations
![Configuring OpenTelemetry environment parameters](/images/1-Worklog/Week7/Picture26.png)

#### 3. Successfully Creating New Amazon ECS Task Definition Integrated with OpenTelemetry
![ECS Task Definition created successfully](/images/1-Worklog/Week7/Picture27.png)

#### 4. Verifying Active Infrastructure Status of Amazon ECS Clusters
![Checking active Amazon ECS Clusters](/images/1-Worklog/Week7/Picture28.png)

#### 5. Reviewing MiniSocial-Backend-Service Inside Amazon ECS Cluster Environment
![Backend service running on ECS Cluster](/images/1-Worklog/Week7/Picture29.png)

#### 6. Updating Service Configurations and Forcing New Deployments on Amazon ECS
![Updating and deploying new ECS task version](/images/1-Worklog/Week7/Picture30.png)

#### 7. Monitoring Running Container Status and Health Metrics on AWS Fargate Tasks
![Monitoring running container instance tasks](/images/1-Worklog/Week7/Picture31.png)

#### 8. Tracking System Performance and CPU Usage Percentage Analytics Charts
![Tracking system CPU usage charts](/images/1-Worklog/Week7/Picture32.png)

#### 9. Detailed Dashboard Monitoring Real-time CPU and Memory Utilization
![CPU and Memory utilization monitoring dashboard](/images/1-Worklog/Week7/Picture33.png)

#### 10. Inspecting and Analyzing Spring Boot Application Log Events via Amazon CloudWatch
![Inspecting log events inside Amazon CloudWatch](/images/1-Worklog/Week7/Picture34.png)

#### 11. Go to the AWS office
![Group Meeting](/images/1-Worklog/Week7/0406_meeting_w7.JPG)