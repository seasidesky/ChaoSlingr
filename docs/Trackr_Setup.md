# Trackr Initial Setup

Create a new CoudTrail for Trackr.

Create a new CloudWatch alarm. Select the Custom Metric, CoudTrailMetrics. Select Metric Name, SecurityGroupEventCount. Trigger when SecurityGroupEventCount is >= 1.

Create a new CloudWatch Rule. Set up Event Source as so:

![alt text](trackr-rule.png)

Go to the Trackr Lambda function and add trigger, CloudWatch Events, and use the CloudWatch Rule created earlier.
