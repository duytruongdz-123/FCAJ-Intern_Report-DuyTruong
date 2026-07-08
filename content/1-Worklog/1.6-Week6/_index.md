---
title: "Week 6 Worklog"
date: 2026-05-25
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---


### Week 6 Objectives:

* Evaluate cloud infrastructure resiliency and breakpoint limitations under severe traffic conditions.
* Stream local test execution load metrics directly into Grafana Cloud dashboards for correlation analysis.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Learn how to formulate advanced load profiles using the open-source `k6` stress testing framework | 05/25/2026 | 05/25/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 3 | - Write a specialized JavaScript load test script in `k6` designed to ramp up concurrent traffic aggressively from 50 to 400 Virtual Users (VUs) | 05/26/2026 | 05/26/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 4 | - Run local stress tests against target systems and log execution timelines | 05/27/2026 | 05/27/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 5 | - Audit system baseline values against high-load stress metrics (noting instances where CPU maxed at 100%, Target Response Time hit around 7.5 seconds, and active database sessions doubled) | 05/28/2026 | 05/28/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |
| 6 | - Configure the Prometheus Remote Write Endpoint in the local `k6` agent <br> - Stream local execution metrics directly onto Grafana Cloud dashboards | 05/29/2026 | 05/29/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04/> |


### Week 6 Achievements:

* Developed structured automated testing profiles to expose infrastructure limits.
* Successfully verified system behavior under 8x scaling spikes, recording critical latency spikes (~7.5s response delay) and computing bottlenecks.
* Consolidated decoupled load metrics by configuring Prometheus Remote Write pipelines.
* Achieved cross-environment correlation capabilities, allowing unified performance analysis of load generators alongside live hardware infrastructure dashboards.

---

### Week 6 Evidence Images

#### 1. Generating Token and Obtaining Token Link
![Configuring OTLP or Spring Boot Metrics on Grafana Cloud to get Endpoint URL and API Token](/images/1-Worklog/Week6/Picture13.png)

![Creating automated Alerting Rule within Grafana Cloud Console](/images/1-Worklog/Week6/Picture14.png)

![Setting alert conditions for HTTP 500 errors or RAM CPU exceeding 85 percent within 1 minute](/images/1-Worklog/Week6/Picture15.png)

#### 2. Creating Local Backend Application
![Connecting contact points to configure automatic email routing](/images/1-Worklog/Week6/Picture16.png)

#### 3. Launching Application and Streaming Data
![Writing specialized JavaScript load test script in k6 from 50 to 400 VUs](/images/1-Worklog/Week6/Picture17.png)

#### 4. Streaming Local Data to Display on Grafana Server Dashboards
![Executing local k6 stress tests and logging execution timeline](/images/1-Worklog/Week6/Picture18.png)

![Auditing high load metrics showing CPU utilization maxed at 100%](/images/1-Worklog/Week6/Picture19.png)

![Monitoring system behavior with target response time hitting 7.5 seconds](/images/1-Worklog/Week6/Picture20.png)

![Verifying metrics where active database sessions doubled](/images/1-Worklog/Week6/Picture21.png)

#### 5. Configuring Alert Notification Email Address
![Configuring Prometheus Remote Write Endpoint within local k6 agent](/images/1-Worklog/Week6/Picture22.png)

#### 6. Creating Alert Rule
![Screenshot of Grafana Cloud Dashboard with real time metrics streaming from local backend](/images/1-Worklog/Week6/Picture23.png)

#### 7. Receiving Automated Alert Notification Emails Dispatched from Grafana Cloud System
![Screenshot of mailbox showing automated alert notification emails from Grafana Cloud](/images/1-Worklog/Week6/Picture24.png)

#### 8. Group Meeting
![Group Meeting](/images/1-Worklog/Week6/2905_meeting_w6.JPG)