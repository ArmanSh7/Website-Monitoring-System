# Website Monitoring System
Website downtime costs businesses thousands of dollars per minute. 
This project implements a fully automated, serverless website monitoring system on AWS that detects failures in under 5 minutes, configurable to as low as 1 minute, and immediately alerts stakeholders, ensuring teams can respond before losses escalate

# Technologies used
Python, AWS Lambda, Amazon SQS, Amazon SNS, Amazon EventBridge, IAM, CloudWatch, boto3

# Architecture Diagram
EventBridge triggers the WebsiteChecker Lambda function every X minutes.n/ 
On failure, a message is sent to an SQS queue which automatically triggers the FailureProcessor Lambda function. 
The failure details are then published to an SNS topic which delivers an email alert to all subscribers.

![Diagram](diagram.png)

# Code
![Checking website vailibility function](website_availibility_function.png)

![Sending_failure_details to _SQS](SQS_processing.png)

![Publishing an alert to SNS](SNS.png)

![Formatting alert message](format_alert.png)

# Results
## Email Alert
![Email](result.png)
