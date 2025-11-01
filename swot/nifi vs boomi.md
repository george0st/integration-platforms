## 1. Summary

When to choose Apache NiFi:
- You need maximum flexibility and customization with focus on technology connectors
  (business connectors are not needed)
- You have technical resources for solution support, deployment and CI/CD
- You are able to accept or cover security topics/limitations
- You prefer CAPEX & PEREX costs (your own infrastructure and support)

When to choose Boomi:
- You are able to rely on a vendor-managed solution
- You prioritize ease of use and rapid deployment (instead of full control)
- You work primarily with cloud-based applications and SaaS connectors
- You don't want to have a team to manage and operate the infrastructure
- You prefer OPEX costs (see iPaaS model)

## 2. Compare

### 2.1 Pricing & Support
|                    | Apache NiFi                                    | Boomi                                                                                                             |
|--------------------|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Vendor lock-in     | None                                           | Yes, typically annual contracts                                                                                   
| Pricing            | Open source                                    | Paid solution                                                                                                     
| Pricing model      | Free                                           | Pricing depends on the number of used connectors, workflow, environments, modules, etc. (with 30-day free trial). 
| Support level      | Only free support (Slack, StackOverflow, etc.) | Strong support                                                                                                    
| Support channel    | On-line                                        |
| SLA                | Without SLA                                    | SLA based on support level (24x7, etc.)                                                                           
| Training           |                                                |

### 2.2 Architecture
|                                | Apache NiFi                                                | Boomi                      |
|--------------------------------|------------------------------------------------------------|----------------------------|
| Architecture                   |                                                            |
| Cloud architecture             | Without iPass (own hosting is needed)                      | Full cloud solution (SaaS) 

### 2.3 Integration

|                                | Apache NiFi                                                | Boomi                      |
|--------------------------------|------------------------------------------------------------|----------------------------|
| Integration                    | ~100 connectors/processors, focus on technology connectors (missing business connectors)     | >1.000 connectors, technology connectors + business connectors (Salesforce, SAP, NetSuite, etc.)

### 2.4 Development & Deployment
|                                | Apache NiFi                                                | Boomi                      |
|--------------------------------|------------------------------------------------------------|----------------------------|
| Code management                | Limited own versioning (for extended functionalities, ext tools are needed GitHub/Lab, etc.) | Build in versioning with CI/CD               
| Change management (inc. CI/CD) | Without support (only exp/imp flows)                                                         | Full support versioning/packaging, deployment/rollback, env. configuration
| Developer GUI                  | Drag & Drop UI, without content hierarchy                                                    | Drag & Drop UI, content hieararchy

### 2.5 Security
|                                | Apache NiFi                                                | Boomi                      |
|--------------------------------|------------------------------------------------------------|----------------------------|
| Security certification         | Without enterprise certifications (e.g. HIPAA, SOC2)                                         | Enterprise compliance
| Security SSO + RBAC            |                                                                                              |

### 2.6 Maintenance
|                                | Apache NiFi                                                | Boomi                      |
|--------------------------------|------------------------------------------------------------|----------------------------|
| Monitoring and alerts          | Basic functionalities, external tooling is needed                                            | Native monitoring, allerts, audit logs               
| Reporting                      |                                                                                              | 

TBD. Known limits


## 3. Details
TBD.