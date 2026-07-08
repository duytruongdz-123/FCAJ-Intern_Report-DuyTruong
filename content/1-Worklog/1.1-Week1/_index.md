---
title: "Week 1 Worklog"
date: 2026-04-20
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---



### Week 1 Objectives:

* Set up automated security log monitoring and anomaly detection using AWS CloudWatch.
* Configure real-time security alerts via Amazon SNS to notify administrators of potential attacks.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Route system and application log files from EC2 instances into CloudWatch Logs | 04/20/2026 | 04/20/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 3 | - Create CloudWatch Log Groups <br> - Configure a global Metric Filter using `{ $.type = "SECURITY" }` to capture all security-related incidents | 04/21/2026 | 04/21/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Setup granular Metric Filters to count specific attack types: <br> &emsp; + SQL Injection: `{ $.msg = "*type=SQL_INJECTION*" }` <br> &emsp; + XSS: `{ $.msg = "*type=XSS_ATTACK*" }` <br> &emsp; + Path Traversal: `{ $.msg = "*type=PATH_TRAVERSAL*" }` <br> - Assign Metric Value as 1 and Default Value as 0 | 04/22/2026 | 04/22/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Create an Amazon SNS Standard Topic named `Security-Alerts` <br> - Create an Email Subscription targeting `duytruongsb30@gmail.com` <br> - Access the email inbox and confirm the subscription | 04/23/2026 | 04/23/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Create a CloudWatch Alarm bound to the `SecurityAttackCount` metric <br> - Configure alarm condition: Greater than or equal to 1 incident within a 1-minute period <br> - Map the `In Alarm` state actions to trigger the `Security-Alerts` SNS Topic | 04/24/2026 | 04/24/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Week 1 Achievements:

* Successfully established a centralized logging pipeline from EC2 to CloudWatch Logs.
* Mastered pattern matching syntax in CloudWatch Metric Filters to detect and classify web application attacks (SQLi, XSS, Path Traversal).
* Created a functional Amazon SNS alerting topic and successfully verified email registration protocol.
* Configured automated threshold-based CloudWatch Alarms to transition to `In Alarm` state and instantly notify administrators upon security breaches.
* Validated the end-to-end integration architecture: `[Log File] -> [CloudWatch Metric Filter] -> [Alarm] -> [SNS Topic] -> [Admin Email]`.

---

### Week 1 Evidence Images

#### 1. Online team meeting on Google Meet
![Meeting Online](/images/1-Worklog/Week1/2604_meetingOnl_w1.png)