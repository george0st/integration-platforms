## 1. Summary

When to choose Apache NiFi:
- You need maximum flexibility and customization with focus on technology connectors
  (business connectors are not needed)
- You have technical resources for solution support, deployment and CI/CD
- You are able to accept or cover security topics/limitations
- You prefer CAPEX & PEREX costs (inicial investment to your own infrastructure and support)

When to choose Boomi:
- You are able to rely on a vendor-managed solution
- You prioritize ease of use and rapid deployment (instead of full control)
- You work primarily with cloud-based applications and SaaS connectors
- You don't want to have a team to manage and operate the infrastructure
- You prefer OPEX costs (iPaaS model, "pay as you go", etc.)

## 2. Heat matrix
tbd.


## 3. Compare

### 3.1 Pricing & Support
|                    | Apache NiFi                                    | Boomi                                                                                                             |
|--------------------|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Vendor lock-in     | No                                             | Yes (typically annual payment)                                                                                   
| Pricing            | Open source                                    | Paid solution                                                                                                     
| Pricing model      | Free                                           | Pricing depends on the number of used connectors, workflow, environments, modules, etc. (with 30-day free trial). 
| Support level      | Only free support (Slack, StackOverflow, etc.) | Strong support (inc. platform Dev & Assurance, platform arch, enterprise arch, etc.)                                                                                                     
| Support channel    | Portal                                         | Portal, Phone, Chat 
| SLA                | Without SLA                                    | SLA based on support level (24x7, etc.)                                                                           
| Training           |                                                |

### 3.2 Architecture & Scaling
|                    | Apache NiFi                                                         | Boomi                      |
|--------------------|---------------------------------------------------------------------|----------------------------|
| Architecture       |                                                                     |
| Cloud architecture | Without iPass (own hosting is needed)                               | Full cloud solution (SaaS) 
| Scaling            | Without limitations for scale up/out (also solutions with 1k nodes) | Cluster size till 10 moleculas/nodes

NOTE:
 - Boomi, has limit in maximal amount of moleculas/nodes in one cluster 

### 3.3 Integration
|                 | Apache NiFi                                                                                  | Boomi                      |
|-----------------|----------------------------------------------------------------------------------------------|----------------------------|
| Integration     | ~100 connectors/processors, focus on technology connectors (SFTP, Mongo, MySQL, Kafka, etc.) | >1.000 connectors, technology connectors + business connectors (Salesforce, SAP, NetSuite, etc.)
| Native formates | CSV, XML, JSON                                                                               | CSV, TXT, XML, JSON, EDI
| Limits          | Missing business connectors (SalesForce, SAP, MS Dynamics, etc.)                             |


### 3.4 Development & Tests
|                     | Apache NiFi                                                                                  | Boomi                                                                      |
|---------------------|----------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
| Runtime environment | Java 21 (in NiFi v2.6)                                                                       | Java 11 (in Boomi v ??)
| Dev GUI             | Drag & Drop UI, without content hierarchy                                                    | Drag & Drop UI, content hierarchy
| Sub-flow            | Yes (main flow & sub-flow, shared controllers)                                               | Yes (main flow & sub-flow, shared connectors)
| Code management     | Limited own versioning (for extended functionalities, ext tools are needed GitHub/Lab, etc.) | Build in versioning in tool
| Testing             | In the GUI (flow & processor/controller levels)                                              | In the GUI (test flow)

NOTE:
- NiFi, Dev GUI without content hierarchy
- Boomi, older Java version (limited features & performance and can generate issue in case of build our own connectors)

### 3.5 Deployment
|                     | Apache NiFi                                 | Boomi                                                                      |
|---------------------|---------------------------------------------|----------------------------------------------------------------------------|
| Env. configuration  | Yes (via ???)                               | Yes (via extensions)
| CI/CD               | No (only exp/imp flow files, without CI/CD) | Yes (full support versioning/packaging, deployment/rollback, env. configuration) 


### 3.6 Security
|                        | Apache NiFi                        | Boomi                      |
|------------------------|------------------------------------|----------------------------|
| Security certification | Without enterprise certifications  | Enterprise compliance (e.g. HIPAA, SOC2, etc.) 
| Security SSO           |                                    |
| Security RBAC          |                                    |

### 3.7 Maintenance
|                                | Apache NiFi                                        | Boomi                      |
|--------------------------------|----------------------------------------------------|----------------------------|
| Monitoring and alerts          | Basic functionalities, external tooling is needed  | Native monitoring, allerts, audit logs               
| Reporting                      |                                                    | 

TBD. Known limits


## 4. Details
TBD.