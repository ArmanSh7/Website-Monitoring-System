<img width="1357" height="512" alt="image" src="https://github.com/user-attachments/assets/9b6a0649-d39d-473f-b700-4feb049b20e7" /># Website-Monitoring-System
Website downtime costs businesses thousands of dollars per minute. 
This project implements a fully automated, serverless website monitoring system on AWS that detects failures in under 5 minutes, configurable to as low as 1 minute, and immediately alerts stakeholders, ensuring teams can respond before losses escalate

# Technologies used
Python, AWS Lambda, Amazon SQS, Amazon SNS, Amazon EventBridge, IAM, CloudWatch, boto3

# Architecture Diagram
![Diagram](diagram.png)

# Code
![Checking website vailibility function](website_availibility_function.png)

![Sending_failure_details to _SQS](SQS_processing.png)

![Publishing an alert to SNS](SNS.png)

![Formatting alert message](format_alert.png)

![Email](result.png)
