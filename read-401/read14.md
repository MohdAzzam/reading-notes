## AWS — Difference between **SQS** and **SNS** 



* **SNS** is a distributed publish-subscribe system.
* Messages are pushed to subscribers as and when they are sent by publishers to **SNS**.


* **SQS** is distributed queuing system , Messages are not pushed to receivers, Receivers have to poll or pull messages from SQS.


### Entity Type

* **SQS**: Queue 
* **SNS**: Topic (Pub/Sub system)

### Message consumption

* **SQS**: Pull Mechanism - Consumers poll and pull messages from **SQS**
* **SNS**: Push Mechanism - **SNS** Pushes messages to consumers

### Use Case

* **SQS**: Decoupling two applications and allowing parallel asynchronous processing
* **SNS**: Fanout - Processing the same message in multiple ways
### Persistence

* **SQS**: Messages are persisted for some (configurable) duration if no consumer is available (maximum two weeks), so the consumer does not have to be up when messages are added to queue.
* **SNS**: No persistence. Whichever consumer is present at the time of message arrival gets the message and the message is deleted. If no consumers are available then the message is lost after a few retries.
### Consumer Type

* **SQS**: All the consumers are typically identical and hence process the messages in the exact same way (each message is processed once by one consumer, though in rare cases messages may be resent)
* **SNS**: The consumers might process the messages in different ways
### Sample applications

* **SQS**: Jobs framework: The Jobs are submitted to **SQS** and the consumers at the other end can process the jobs asynchronously. If the job frequency increases, the number of consumers can simply be increased to achieve better throughput.
* **SNS**: Image processing. If someone uploads an image to S3 then watermark that image, create a thumbnail and also send a Thank You email. In that case S3 can publish notifications to an **SNS** topic with three consumers listening to it. The first one watermarks the image, the second one creates a thumbnail and the third one sends a Thank You email. All of them receive the same message (image URL) and do their processing in parallel.
