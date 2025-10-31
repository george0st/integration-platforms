# NiFi SWOT analysis

The SWOT analysis from perspective of Strengths, Weaknesses, Opportunities
and Threats. 

Last update: 2025/10 (Apache NiFi 2.6)

## 1. Strengths
  Strengths: items as advantages, benefits.

  ### 1.1 Licence & Support
  - **Licence**
    - Free (open source)
  - **Support** 
    - Not available (without iPaaS, only open source community support)
    - Only available as solution of 3rd party SW (in products Cloudera, Snowflake, Ksolves, etc.)

  ### 1.2 Functionalities
  - **Environment**
    - on-prem, cloud
  - **Reliability**
    - Prevention of system overloading (via throttling)
    - Throttling as default (via amount of items in queue and total queue size)
  - **Scaling**
    - Parallel processing as default (amount of executors, data distribution via queues)
  - **Streaming**
    - tbd.
  - **Native formats**
    - CSV, XML, JSON

  ### 1.3 Connectors
  - File transfer, AWS S2, Azure BlobStorage
    - Azure BlobStorage, AWS S3, Google CloudBucket, Google Drive, Azure DataLake, SFTP/FTP,   
  - SQL
    - MySQL, JDBC,
  - NoSQL
    - DynamoDB, Mongo, Google BigGuery
  - Event streaming (MQ, Kafka)
    - AMQP, Azure EventHub, Google Cloud PubSubs, JMS, Kafka, KinesisStream, MQTT, 
  - Other
    - WebSocket, Amazon Lambda, Splunk, SalesForce
    - ElasticSearch, IMAP, POP3, Slack, Twitter, DropBox, ZenDesk, Amazon Glue 

  ### 1.4 Environment
  - Java 21
  - CI/CD - own, GitHub, GitLab

  ### 1.5 Architecture
  - Pear-to-pear cluster architecture
  - Node coordination and primary node definition via Zookeeper
  - Unlimited amount of nodes (real clusters use from 2 to 1k nodes)

  ### 1.6 Key contributors
  - Cloudera
  - Snowflake
  - Ksolves
  - Etc. (see https://nifi.apache.org/community/powered-by/)

## 2. Weaknesses
  Weaknesses: items as disadvantages, limited functions.

  ### 2.1 Connectors

  ### 2.2 Testing
  - Missing default E2E test for validation of new Apache NiFi versions  

  ### 2.3 Security
  - Limited privileges (without setting in project, flow level)

  ### 2.4 Others
  - Without deployment functionalities (package & env. extensions)
  - Only external relation on CI/CD

## 3. Opportunities

  Opportunities: items could exploit to its advantage, future direction.

## 4. Threats

  Threats: items that could cause trouble, risk.