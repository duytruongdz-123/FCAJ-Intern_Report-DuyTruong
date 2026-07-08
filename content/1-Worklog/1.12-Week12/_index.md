---
title: "Week 12 Worklog"
date: 2026-07-05
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Week 12 Objectives:

- Retrieve and analyze the existing monitoring dashboards for the application, AWS resources, and overall infrastructure.
- Extract and analyze system logs from AWS CloudWatch to diagnose database connectivity and connection pool issues.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| :--- | :--- | :--- | :--- | :--- |
| 2 | - Retrieve and review the Application and AWS Resources dashboards  | 07/06/2026 | 07/06/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04> |
| 3 | - Analyze the Overall Infrastructure dashboard including ALB, ECS, and RDS metrics  | 07/07/2026 | 07/07/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04> |
| 4 | - Extract CloudWatch logs to troubleshoot system errors <br> - Diagnose SQL Server and HikariPool timeouts  | 07/08/2026 | 07/08/2026 | <https://duytruongsb30.grafana.net/public-dashboards/7edfaa6aed8e474ca2efbaaa929c7c04> |

### Week 12 Achievements:

- **Dashboard Analysis:** Successfully retrieved and evaluated the 3 pre-configured Grafana dashboards covering Application health, AWS Resources, and Infrastructure metrics.
- **System Monitoring:** Extracted error logs directly from the AWS CloudWatch console for the `ecs/minisocial-backend` log group.
- **Troubleshooting (Database):** Identified critical `SQLServerException` errors caused by TCP/IP connection timeouts to the RDS instance on port 1433.
- **Troubleshooting (Connection Pool):** Diagnosed database connection exhaustion issues where `HikariPool-1` failed to validate connections or timed out after 30000ms.
- **Troubleshooting (Authentication):** Detected multiple `ExpiredJwtException` errors indicating issues with client token expiration during WebSocket authentication.

### Week 12 Evidence Images

#### 1. Application Dashboard on Grafana
![Application Performance Monitoring Dashboard on Grafana](/images/1-Worklog/Week12/Picture1.png)

#### 2. AWS Resources Dashboard on Grafana
![AWS Resources Monitoring Dashboard on Grafana](/images/1-Worklog/Week12/Picture2.png)

#### 3. Infrastructure Dashboard on Grafana
![Infrastructure Overview Monitoring Dashboard on Grafana](/images/1-Worklog/Week12/Picture3.png)

#### 4. Log groups list interface on Amazon CloudWatch
![Log groups list interface on Amazon CloudWatch](/images/1-Worklog/Week12/Picture4.png)

