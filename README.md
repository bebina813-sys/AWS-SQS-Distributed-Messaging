[AWS SQS Workshop.docx](https://github.com/user-attachments/files/33025723/AWS.SQS.Workshop.docx)
[AWS SQS Workshop.docx](https://github.com/user-attachments/files/33025717/AWS.SQS.Workshop.docx)
# AWS-SQS-Distributed-Messaging

Hands-on AWS SQS project demonstrating distributed messaging, producer-consumer architecture, message processing, and queue management.
Overview

This project demonstrates the use of Amazon Simple Queue Service (SQS) for asynchronous and distributed messaging.

AWS Service Used
Amazon SQS
Standard Queue
What I Implemented
Created an SQS Standard Queue named Orders
Sent an order message to the queue
Received the message using Poll for messages
Verified the message body and message details
Deleted the message after processing
Polled the queue again and verified that no messages were available
Message Flow
Producer
   ↓
Amazon SQS – Orders Queue
   ↓
Receive / Poll Message
   ↓
Process Message
   ↓
Delete Message
Key Concepts Learned
Producer

The producer sends messages to the SQS queue.

Queue

Amazon SQS temporarily stores messages until they are received and processed.

Consumer

The consumer receives and processes messages from the queue.

Visibility Timeout

After a message is received, SQS temporarily hides it from other consumers. If it is not deleted within the visibility timeout, it can become visible again.

Message Deletion

After successful processing, the consumer deletes the message from the queue.

Practical Result

Successfully completed the basic SQS message workflow:

Create Queue → Send Message → Receive Message → Process → Delete Message

Skills Demonstrated
AWS SQS
AWS Management Console
Distributed Messaging
Producer-Consumer Architecture
Asynchronous Communication
Cloud Fundamentals
Workshop Reference

AWS Hands-on Workshop – Send Messages Between Distributed Applications
