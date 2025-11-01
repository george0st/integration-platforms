## 1. Summary

**When to choose Apache NiFi:**
- You need maximum flexibility and customization with focus on technology connectors
  (business connectors are not needed)
- You have technical resources for solution support, deployment and CI/CD
- You are able to accept or cover security topics/limitations
- You prefer CAPEX & PEREX costs (initial investment to your own infrastructure and support)

**When to choose Boomi:**
- You are able to rely on a vendor-managed solution
- You prioritize ease of use and rapid deployment (instead of full control)
- You work primarily with cloud-based applications (on-prem is possible)
- You don't want to have a team to manage and operate the infrastructure
- You prefer OPEX costs (iPaaS model, "pay as you go", etc.)

## 3. Compare

### 3.1 Basic information
|                 | Apache NiFi                                          | Boomi                                                                                                             |
|-----------------|------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Founded         | 2006 (Apache NiFi v2.0 in 2024)                      | 2000
| Current version | v2.6                                                 | v???
| Vendor lock-in  | No                                                   | Yes (one vendor, typicall licence with annual payment)                                                                                   
| Licence         | Open source (Apache License 2.0)                     | Commercial ([complex pricing + free trial 30 days](https://boomi.com/pricing/))
| Pricing         | Free                                                 | [Free trial](https://boomi.com/pricing/#free-trial) (only 30 days, limited functionalities)]; [Pay-as-you-go](https://boomi.com/pricing/#pay-as-you-go); [Subscription plans](https://boomi.com/pricing/#subscription-plans) (for Integration, API Management, Data Hub, Data Integration)
| Customers       | Cloudera, Snowflake, Apple, SAP, EPAM, Ksolves, etc. | Dell, NNIT, Novartis, BNP Paribas, Chevron, Sky, etc.

NOTE:
 - NiFi, is abbreviation of NiagaraFiles
 - Nifi, uses the 3rd parties into own solutions such as Cloudera (in Cloudera Data Flow and Cloudera Flow Manager)
   or Snowflake (in Snowflake Openflow), or Ksolves (in Data Flow Manager)

### 3.2 Support & Customers
|                 | Apache NiFi                                          | Boomi                                                                                                             |
|-----------------|------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Support level   | Only free support (Slack, StackOverflow, etc.)       | [Levels](https://boomi.com/services/support/) Basic Support, Enhanced Support, Advocate Bundle, Side by Side Bundle                                                                                                     
| Support channel | Portal                                               | Portal, Phone, Chat
| Support SLA     | Without SLA                                          | SLA based on support level (24x7, 12x7, etc.)

### 3.3 Architecture & Environments & Scaling
|              | Apache NiFi                                                         | Boomi                      |
|--------------|---------------------------------------------------------------------|----------------------------|
| Architecture | Pear-to-pear cluster architecture, coordination/synch via Zookeeper | Client-server architecture
| Environments | On-prem, Cloud, Multi-cloud, Hybrid                                 | On-prem, Cloud, Multi-cloud, Hybrid
| Service type | Without service support (own infra or hosting is needed)            | iPaaS 
| Scaling      | Without limitations for scale up/out (also solutions with 1k nodes) | Unlimited scale up, limited scale out (cluster can have maximal 10 moleculas/nodes)

NOTE:
 - Boomi, has limit for maximal amount of moleculas/nodes in one cluster

### 3.4 Integration & Formats
|                | Apache NiFi                                                                                      | Boomi                      |
|----------------|--------------------------------------------------------------------------------------------------|----------------------------|
| Integration    | ~100 connectors/processors and focus on technology connectors (SFTP, Mongo, MySQL, Kafka, etc.) | >1.500 connectors, technology connectors + business connectors (Salesforce, SAP, NetSuite, etc.)
| Native formats | CSV, XML, JSON                                                                                   | CSV, TXT, XML, JSON, EDI
| Limits         | Missing business connectors (SalesForce, SAP, MS Dynamics, etc.)                                 |

NOTE:
 - Boomi, provides unexpected amount of connectors (include business connectors) and support EDI format

### 3.5 Development & Tests
|                     | Apache NiFi                                                                                  | Boomi                                                                      |
|---------------------|----------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
| Runtime environment | Java 21                                                                                      | Java 11
| Sub-flow            | Supported (main flow & sub-flow, shared controllers)                                         | Supported (main flow & sub-flow, shared connectors)
| Dev GUI             | Drag & Drop UI, without content hierarchy                                                    | Drag & Drop UI, content hierarchy
| Code management     | Limited own versioning (for extended functionalities, ext tools are needed GitHub/Lab, etc.) | Build in versioning in tool
| Testing             | In the GUI (flow & processor/controller levels)                                              | In the GUI (test flow)

+Terminology 

NOTE:
- NiFi, Dev GUI without content hierarchy
- Boomi, older Java version (limited features & performance and can generate issue in case of build our own connectors)

### 3.6 Deployment
|                     | Apache NiFi                                 | Boomi                                                                      |
|---------------------|---------------------------------------------|----------------------------------------------------------------------------|
| Env. configuration  | Yes (via ???)                               | Yes (via extensions)
| CI/CD               | No (only exp/imp flow files, without CI/CD) | Yes (full support versioning/packaging, deployment/rollback, env. configuration) 

### 3.7 Security
|                        | Apache NiFi                        | Boomi                      |
|------------------------|------------------------------------|----------------------------|
| Security certification | Without enterprise certifications  | Enterprise compliance (e.g. HIPAA, SOC2, etc.) 
| Security SSO           |                                    |
| Security RBAC          |                                    |

### 3.8 Maintenance
|                                | Apache NiFi                                        | Boomi                      |
|--------------------------------|----------------------------------------------------|----------------------------|
| Monitoring and alerts          | Basic functionalities, external tooling is needed  | Native monitoring, allerts, audit logs               
| Reporting                      |                                                    |

### 3.9 Knowledge
|                | Apache NiFi                                                                                                                                                 | Boomi                                                                                                             |
|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Training       | Low (paid Udemu, free tutorials in YouTube, Webs, etc.)                                                                                                     | High (free [trainings](https://train.boomi.com/page/course-catalog))
| Certification  | Low (paid Udemy, etc.)                                                                                                                                      | High (free [certifications](https://train.boomi.com/page/course-catalog#type_certification))
| Community      | Medium (free [NiFi](https://nifi.apache.org/community/), [LinkedIn](https://www.linkedin.com/company/apache-nifi/), [Slack](https://apachenifi.slack.com/)) | High (free [Boomi](https://community.boomi.com/), [LinkedIn](https://www.linkedin.com/company/boomi-inc/))
| Community size | [~4k clients](https://enlyft.com/tech/products/apache-nifi), ~30k users in LinkedIn                                                                         | [~23k clients](https://canvasbusinessmodel.com/blogs/growth-strategy/boomi-growth-strategy)

TBD. Known limits


## 4. Details
TBD.