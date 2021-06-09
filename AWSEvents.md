# AWS: Events

- **Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server**

    In Express server you connect and send HTTP requests to a specific endpoints and connect them with handler functions on the same server, while using AWS you can separate the routing process and the function handler, where you send the HTTP request using AWS API Gateway and integrate them with Lambda functions as they will be triggered when specific route been hit, and all this process will be serverless.(both uses RESTful api and uses HTTP for res/req , both uses function to handle those requests and create proper response.)

- **List the AWS Database offerings and talk about the pros and cons of each**

    - Relational:
Traditional applications, ERP, CRM, e-commerce

    - Key-value:
High-traffic web apps, e-commerce systems, gaming applications
    - In-memory
Caching, session management, gaming leaderboards, geospatial applications
    - Document
Content management, catalogs, user profiles
    - Wide column
High scale industrial apps for equipment maintenance, fleet management, and route optimization

    - Graph
Fraud detection, social networking, recommendation engines
    - Time series
IoT applications, DevOps, industrial telemetry
    - Ledger
Systems of record, supply chain, registrations, banking transactions

[source](https://aws.amazon.com/products/databases/)

Amazon Relational Database: is a distributed relational database service by Amazon Web Services. It is a web service running "in the cloud" designed to simplify the setup, operation, and scaling of a relational database for use in applications.
Amazon DynamoDB is a fully managed proprietary NoSQL database service that supports key–value and document data structures and is offered by Amazon.com as part of the Amazon Web Services portfolio. DynamoDB exposes a similar data model to and derives its name from Dynamo, but has a different underlying implementation.

- **What’s the difference between a FIFO and a standard queue?**

    FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing.

- **How can the server be assured a message was properly received?**

    By listening to a trigger on the delivered side which works when the message is received

<hr>

## Term
- **Serverless API:**
<!-- Using API Gateway, you can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, as well as web applications.[source](https://aws.amazon.com/api-gateway/) -->
 is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers

- **Triggers:**
are what cause a function to run. A trigger defines how a function is invoked and a function must have exactly one trigger. Triggers have associated data, which is often provided as the payload of the function

- **Dynamo vs Mongo:**
MongoDB is vendor agnostic, Open Source, and can be deployed anywhere. DynamoDB is only available on AWS.

DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas.

DynamoDB as an integrated AWS service makes it easier to develop end to end solutions.

DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents.

DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions.
[source](https://www.xplenty.com/blog/dynamodb-vs-mongodb-differences/)

- Dynamoose vs Mongoose:Dynamoose is a modeling tool for Amazon’s DynamoDB (inspired by Mongoose)
Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node. js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.

<hr>

### Preparation Materials

- SQS and SNS:simple notification service and simple queue service 
![sns](https://miro.medium.com/max/1004/1*mdUPKzrfJFuXa4d43KhKUQ.png)
Amazon SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. Amazon SNS makes it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services.

![sqs](https://miro.medium.com/max/1700/1*7eL3udb6Cto4I9Ly1sN8oA.jpeg)
SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can’t be received by multiple receivers at the same time. Any one receiver can receive a message, process and delete it. Other receivers do not receive the same message later.
Polling inherently introduces some latency in message delivery in SQS unlike SNS where messages are immediately pushed to subscribers.
[source](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

<hr>

 [SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)

 [AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)


### Bookmark

- [SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)

- [SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)