<div id="top"></div>



<details>
  <summary>Table of Contents </summary>
  <ol>
  <li><a href="#technical">Technical Architecture</a></li>
    Project</a>
        <ul>
          <li><a href="#about-the-project">About The Project
          <li><a href="#overview">Overview</a></li>
          <li><a href="#key-features">Key Features</a></li>
        </ul>
    </li>
     <li><a href="#technoloy">Technologies Used</a></li>
    <li><a href="#Built With">Built With</a></li>
    <li><a href="#Dependencies">Dependencies</a></li>
    <li><a href="#challenges">Challenges</a></li>
  </ol>
</details>


# Event-Driven Architecture Notification App using AWS Services

## Technical Architecture 

![nba_API](https://github.com/user-attachments/assets/5e19635e-0685-4c07-9601-330f7d1231f9)

<p align="right">(<a href="#top">back to top</a>)</p>

 
### About The Project


This project uses an event-driven architecture built with AWS services like Lambda, event bridge and SNS. It processes updates in real time, making the system scalable, reliable, and efficient.

### Overview

* [Repo Codes](https://github.com/ijayhub/game-day-notifications-aws)

* [documentation]()

<p align="right">(<a href="#top">back to top</a>)</p>


## **Key features**  
  
- **Notifications**: Using Amazon SNS to send a well-formatted score updates to subscribers.

- **Live NBA Scores**: Using API from [sportsdata.io](https://sportsdata.io/) to get real-time NBA game scores.

- **Scheduled Updates**: Automates regular score updates with Amazon EventBridge.  


- **Lambda Function**: Used to invoke API calls for processing and execution of AWS SNS service to emails.

  

## **Built With**

- **AWS Lambda**: Serverless computing for processing events.

- **Amazon SNS**: Messaging service for notifications.

- **AWS EventBridge**: Event bus for connecting applications using events.

- **API**: - Free account with subscription and API Key at [sportsdata.io](https://sportsdata.io/)

- **IAM Security**:
  - Least privilege policies for Lambda, SNS, and EventBridge.

## **Technologies Used**

- Python

- AWS services

- API

## **Dependencies**

- boto3

- urllib.requests

- os

- json

## **Challenges**  
1. In this project, my subscription to AWS SNS kept automatically deleting, and an ID was required; otherwise, I couldn't move on.  

**Solution**: Go to the email you used as the endpoint when creating the subscription and resubscribe.  

Before I knew that, oh my!!!

<img src="error.png">


2. I didn't know why my Lambda function refused to work, so I had to re-check my region and configuration settings before everything worked correctly.
<p align="right">(<a href="#top">back to top</a>)</p>
