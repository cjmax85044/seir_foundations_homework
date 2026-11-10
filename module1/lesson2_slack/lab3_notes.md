For this week, we are being asked to generate messages from the Balerica Bank instance into Slack.

## Homework 1

Read hw1_hello_slack.py
Change hw1_hello_slack.py by adding your name
Run python hw1_hello_slack.py
Output:  
> "Delivered! Go look at #balerica-alerts. That message is yours."
Result:  Message delivered to Slack\#balerica-alerts channel


## Homework 2

Read hw2_hello_slack.py
Run hw2_hello_slack.py
Output:  
> INFO     -> DELIVERED to Slack
> WARNING  -> DELIVERED to Slack
> ERROR    -> DELIVERED to Slack
> CRITICAL -> DELIVERED to Slack
Result:  Four messages delivered to Slack\#balerica-alerts channel.

Changed .env from severity = INFO to ERROR
Output:  
> INFO     -> skipped by your threshold
> WARNING  -> skipped by your threshold
> ERROR    -> DELIVERED to Slack
> CRITICAL -> DELIVERED to Slack

Question:  Which severities arrived, and WHY those?
Answer:  Only two messages arrived at Slack, because I changed the threshold to ERROR or above and only two alerts met that threshold.


## Homework 3

Read hw3_server_time.py
Run hw3_server_time.py
Output:
> Skipped — check SLACK_ALERT_SEVERITY in .env.
> Local fact: the server believes it is Sunday November 08, 2026 at 20:30:23 UTC.

Question:  How many hours apart are server time and my clock? The answer is, the server time is seven hours ahead of my local time.


## Homework 4

Read hw4_disk_watch.py
Run hw4.disk_watch.py

Output:
> Disk is 25.3% used -> severity INFO.
> Skipped by threshold — that can be correct behavior!

Question:  Why is a quiet INFO here GOOD design, not a failure?
Answer:  Since this is not concerning behavior, there is not need to alert someone to take any action.


## Homework 5

Read hw4_load_check.py
Run hw4_load_check.py
Output:
> Load: 0.02 / 0.02 / 0.00 on 2 CPU(s) -> INFO
> Skipped by threshold.

Question:  What would make this number spike on the Balerica bank?
Answer:  This task take the reading of the CPUs over three time frames. If the load over the second time frame, over the course of 5 minutes is larger than the number of CPUs, then the a severity alert of WARNING will be generated.


## Homework 6

Read hw6_incident_drill.py
Run hw6_incident_drill.py
Output:
> Drew incident DRILL-1116: [ERROR] FastAPI /payments endpoint responded 500 twice in one minute.
> Delivered!

Question:  which of these fake incidents deserves to wake a human at 3 AM?


## Homework 7

Read hw7_morning_report.py
Run hw7_morning_report.py
Output:
> MORNING REPORT — Balerica AI server
> - Time: 2026-11-08 21:04:52 UTC
> - Host: ip-172-31-19-201.ec2.internal (Linux x86_64)>
> - Python: 3.9.25
> - Disk on / : 25.3% used
> - Load (1m): 0.00
> - Status: all checks ran. The bank greets the day.

> Skipped — set SLACK_ALERT_SEVERITY=INFO to receive reports.


## Additional Experiments

1. Set SLACK_ALERT_SEVERITY=CRITICAL in .env and rerun script 2. Predict first: How many of the four messages will arrive?

Prediction = 1

> INFO     -> skipped by your threshold
> WARNING  -> skipped by your threshold
> ERROR    -> skipped by your threshold
> CRITICAL -> DELIVERED to Slack

2. Set SLACK_ALERTS_ENABLED=false and run script 1. What happens, and why is a kill switch like this useful during maintenance windows?

> Skipped. Check .env: SLACK_ALERTS_ENABLED must be true and SLACK_ALERT_SEVERITY=INFO (see homework README).

This could be useful during maintenance windows because a lot of alerts may be generated that don't need to be addressed.

3. Open hw4_disk_watch.py in nano and change the WARNING threshold from 75 to a number below your current disk usage. Rerun. Did the severity change?

> Disk is 25.4% used -> severity WARNING.
> Skipped by threshold — that can be correct behavior!

When I edited the threshold from 75% to 5% and ran the script, it changed the severity level to WARNING.

Put everything back: SLACK_ALERT_SEVERITY=INFO, SLACK_ALERTS_ENABLED=true.