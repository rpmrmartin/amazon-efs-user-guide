# Monitoring tools<a name="monitoring_automated_manual"></a>

AWS provides various tools that you can use to monitor Amazon EFS\. You can configure some of these tools to do the monitoring for you, but some of the tools require manual intervention\. We recommend that you automate monitoring tasks as much as possible\.

## Automated monitoring tools<a name="monitoring_automated_tools"></a>

You can use the following automated monitoring tools to watch Amazon EFS and report when something is wrong:
+ **Amazon CloudWatch Alarms** – Watch a single metric over a time period that you specify, and perform one or more actions based on the value of the metric relative to a given threshold over a number of time periods\. The action is a notification sent to an Amazon Simple Notification Service \(Amazon SNS\) topic or Amazon EC2 Auto Scaling policy\. CloudWatch alarms do not invoke actions only because they are in a particular state; the state must have changed and been maintained for a specified number of periods\. For more information, see [Monitoring Amazon EFS with Amazon CloudWatch](monitoring-cloudwatch.md)\.
+ **Amazon CloudWatch Logs** – Monitor, store, and access your log files from AWS CloudTrail or other sources\. For more information, see [Monitoring Log Files](https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html) in the *Amazon CloudWatch User Guide*\.
+ **Amazon CloudWatch Events** – Match events and route them to one or more target functions or streams to make changes, capture state information, and take corrective action\. For more information, see [What is Amazon CloudWatch Events](https://docs.aws.amazon.com/AmazonCloudWatch/latest/events/WhatIsCloudWatchEvents.html) in the *Amazon CloudWatch User Guide*\.
+ **AWS CloudTrail Log Monitoring** – Share log files between accounts, monitor CloudTrail log files in real time by sending them to CloudWatch Logs, write log processing applications in Java, and validate that your log files have not changed after delivery by CloudTrail\. For more information, see [Working with CloudTrail Log Files](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-working-with-log-files.html) in the *AWS CloudTrail User Guide*\. 

## Manual monitoring tools<a name="monitoring_manual_tools"></a>

Another important part of monitoring Amazon EFS involves manually monitoring those items that the Amazon CloudWatch alarms don't cover\. The Amazon EFS, CloudWatch, and other AWS Management Console dashboards provide an at\-a\-glance view of the state of your AWS environment\. We recommend that you also check the log files on file system\.
+ From the Amazon EFS console, you can find the following items for your file systems:
  + The current metered size
  + The number of mount targets
  + The lifecycle state
+ CloudWatch home page shows:
  + Current alarms and status
  + Graphs of alarms and resources
  + Service health status

  In addition, you can use CloudWatch to do the following:
  + Create [customized dashboards](https://docs.aws.amazon.com/AmazonCloudWatch/latest/DeveloperGuide/CloudWatch_Dashboards.html) to monitor the services that you use\.
  + Graph metric data to troubleshoot issues and discover trends\.
  + Search and browse all your AWS resource metrics\.
  + Create and edit alarms to be notified of problems\.