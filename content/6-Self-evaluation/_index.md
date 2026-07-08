---
title: "Self-Assessment"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

Throughout my internship at the Bootcamp program from April 20, 2026, to July 12, 2026, I had the opportunity to comprehensively execute the entire roadmap from Task 1 to Task 12. This process helped me deeply transform my foundational knowledge of computer networks and systems into practical deployment capabilities on the AWS cloud environment and the Grafana Cloud centralized monitoring platform.

Across all work contents, I directly mastered core skills including: setting up automated monitoring and security alerting infrastructure (using CloudWatch Logs, Metric Filters to detect attacks and trigger Alarms via Amazon SNS to Email); configuring enterprise-scale containerized applications on AWS ECS Fargate infrastructure (optimizing Task Definitions integrated with OpenTelemetry OTel and JVM Micrometer environment variables to collect deep application-layer APM data); and System Performance Engineering.

In particular, during the final stage, I personally built a specialized monitoring area called "Stress Test Panel" on Grafana, synchronizing multi-tier data from the Application Load Balancer (ALB) (RequestCount, HTTPCode_Target_5XX_Count, and HTTPCode_ELB_5XX_Count errors), ECS application resources (CPUUtilization, MemoryUtilization), to the number of RDS database connections (DatabaseConnections on the minisocial-sqlserver instance). The system was successfully stress-tested through a k6 script scenario scaling up to 200 VUs, pushing real-time data via the Prometheus Remote Write mechanism for data visualization and triggering threshold-crossing Alert Rules.

Regarding my working style, I always maintained high discipline, ensuring the proposed progress of each task, collaborating effectively with team members, and proactively discussing with the Mentor to perfect the most optimal technical solution.

To provide an objective view of this practical experience from Task 1 to Task 12, I self-assess based on the following criteria:


| No. | Criteria                            | Description                                                                                      | Excellent | Good | Average |
| --- | ----------------------------------- | ------------------------------------------------------------------------------------------------ | --------- | ---- | ------- |
| 1   | **Professional Knowledge & Skills** | Understanding of the field, applying knowledge to practice, tool proficiency, quality of work    | ✅         | ☐    | ☐       |
| 2   | **Learning Ability** | Ability to absorb new knowledge and learn quickly                                                | ✅         | ☐    | ☐       |
| 3   | **Proactivity** | Proactive in work, seeking tasks without waiting for instructions                                | ✅         | ☐    | ☐       |
| 4   | **Sense of Responsibility** | Completing work on time and ensuring quality                                                     | ✅         | ☐    | ☐       |
| 5   | **Discipline** | Adhering to schedules, regulations, and work processes                                           | ✅         | ☐    | ☐       |
| 6   | **Desire for Advancement** | Ready to receive feedback and improve oneself                                                    | ✅         | ☐    | ☐       |
| 7   | **Communication Skills** | Presenting ideas and reporting work clearly                                                      | ☐         | ✅    | ☐       |
| 8   | **Teamwork** | Working effectively with colleagues and actively participating in group activities              | ✅         | ☐    | ☐       |
| 9   | **Professional Demeanor** | Respecting colleagues, partners, and the working environment                                     | ✅         | ☐    | ☐       |

### Areas for Improvement

*   **Communication Skills (Communication):** Need to optimize technical communication by consolidating complex analytical workflows, proactively updating task progress and core solutions concisely to ensure the Mentor and team members can easily grasp information and provide swift feedback.
*   **Problem Solving Mindset (Problem Solving):** Need to establish a more structured diagnostic framework when handling centralized log data, accelerating the scoping of impact boundaries and shortening the time required to isolate unexpected incidents across distributed infrastructure.