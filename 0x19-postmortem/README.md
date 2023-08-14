
![image](https://github.com/loveth007/alx-system_engineering-devops/assets/113848577/0bb7b482-0def-474a-b5c9-1c59d894c916)

![image](https://github.com/loveth007/alx-system_engineering-devops/assets/113848577/7df74cff-96b7-4962-968b-56e00d57c332)
https://medium.com/@lovethokwudiri/issue-summary-from-12-00-am-to-8-oo-am-losam-company-experienced-an-outage-on-cloud-a-that-ff04faeec014

Issue Summary
From 12:00 AM to 8:OO AM, losam company experienced an outage on Cloud A that affected www.losamfoods.com due to a prescheduled reboot that resulted in failure. The points of failure are coming from the rebooting of the load balancer or cache server. The Security Team issued a maintenance update and a reboot notification to a major Cloud A server on JUNE 3, 2023 for a window of 5hours (12:00 to 5:00 AM). 

Timeline (all times in Pacific Time)
9:00 AM: Reboot begins
11:30 AM: Outage begins
12:06 PM: Alerts sent to teams
12:16 PM: Lead SRE silenced all subsequent alerts due to server behavior being “normal”
12:30 PM: Server down and customers can’t reach the site

Root Cause
At 3:56 PM, the reboot of the load-balancer or cache server continued to fail. The secondary server did not come back up for for 3 hours. We did not expect the scheduled reboot to affect our systems. 

Corrective and Preventative Measures
In the last 3 days, we’ve made an internal review and analysis of the outage. The following measures are actions the team will follow for prevention and to improve response times in the future.
The database server provider during the performance degradation could have alerted teams the down server . It was updated to their systems to prevent further issues in the future are done accordingly.
