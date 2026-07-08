---
title: "Week 4 Worklog"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---



### Week 4 Objectives:

* Monitor production application logs in real-time to intercept exceptions and runtime execution faults.
* Implement automated alerting bounds using threshold metrics and simulate system failures to audit alarm accuracy.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Audit application runtime logging patterns stored inside CloudWatch Logs | 05/11/2026 | 05/11/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Configure custom CloudWatch Metric Filters using real-time log scanning syntax to parse specific error keywords like `?Exception` and `?SQL_INJECTION` | 05/12/2026 | 05/12/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Construct a CloudWatch Alarm bound to the newly derived error metrics <br> - Establish alarm thresholds to activate whenever error frequencies reach greater than or equal to 1 occurrence within a 1-minute tracking window | 05/13/2026 | 05/13/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Map the CloudWatch Alarm's `In Alarm` breach handler to push alerts automatically to the predefined SNS email channel | 05/14/2026 | 05/14/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Use Postman to trigger repeated web requests towards invalid application URLs to explicitly force error logs <br> - Verify that the system transitions smoothly to the `In Alarm` state and successfully fires email notifications | 05/15/2026 | 05/15/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Week 4 Achievements:

* Implemented structural real-time metric filtering across high-velocity CloudWatch log groups.
* Successfully configured logic rules for capturing critical software runtime failures and security exceptions.
* Engineered proactive monitoring boundaries by standardizing threshold metrics down to 1-minute resolution limits.
* Validated the resilience and performance of the error alerting workflow using practical API fault injection tests with Postman.

---

### Week 4 Evidence Images

#### 1. Creating CloudWatch Metric Filter for Backend Services
![Successfully created Spring Boot Error Filter](/images/1-Worklog/Week4/Picture5.png)

#### 2. Initializing CloudWatch Alarm Configuration for Spring Boot Fargate
![CloudWatch Alarm initialized with Insufficient Data](/images/1-Worklog/Week4/Picture6.png)

#### 3. AWS Notification Subscription Confirmation Verification
![AWS Subscription confirmed successfully](/images/1-Worklog/Week4/Picture7.png)

#### 4. Alarm Condition Triggered Transitioning System to "In Alarm" State
![CloudWatch Alarm status changes to In Alarm](/images/1-Worklog/Week4/Picture8.png)

#### 5. Production Alert Email Delivered to Admin Inbox Detailing Backend Failures
![Real-time Spring Boot Fargate failure email notification](/images/1-Worklog/Week4/Picture9.png)

#### 6. Group Meeting
![Group Meeting](/images/1-Worklog/Week4/1505_meeting_w4.JPG)