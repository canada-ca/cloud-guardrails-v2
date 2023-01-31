# GC Cloud Guardrails

([Français](#mesures-de-protection-du-nuage-du-gc))

## 1. Introduction

### 1.1 Purpose

In August 2019, the Government of Canada (GC) established supply contracts for Protected B Cloud Services with AWS Canada and Microsoft Azure. In order for the GC to consume this supply in secure and responsible fashion, the Chief Technology Officer of the GC deemed that an underlying operationalization framework was required. An operationalization framework was established and endorsed by [GC EARB](https://gcconnex.gc.ca/file/view/53195105/enabling-secure-access-to-protected-b-cloud-services-gcearb-sept-19-2019?language=en) in September 2019 establishing a set of minimal security controls and architecture prior to departments consuming PB supply. The following figure provides an overview of the framework.

![Figure 1‑1 Operationalization Framework](/image.png "Figure 1‑1 Operationalization Framework")

Following OAG audit recommendation, the Cloud Guardrails have been updated to the current version.

### 1.2 Scope

This document focuses on a preliminary set of baseline security controls to ensure that the cloud service environment has a minimum set of configurations for the cloud environment.

It provides a starting point for project teams and was selected to achieve the following objectives:

- comply with [Directive on Service and Digital](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32601), [Appendix G: Standard on Enterprise Information Technology Service Common Configurations](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32713) - [GC Cloud Guardrails](https://github.com/canada-ca/cloud-guardrails)
- comply with the applicable mandatory procedures in the _[Directive on Security Management](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611)_
- meet the requirements of the [Direction on the Secure Use of Commercial Cloud Services: Security Policy Implementation Notice (SPIN)](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/direction-secure-use-commercial-cloud-services-spin.html)
- address the Canadian Centre for Cyber Security’s (Cyber Centre’s) [Top 10 Security Actions](https://www.cse-cst.gc.ca/en/top10)
- align with _[Government of Canada Security Control Profile for Cloud-Based GC Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-security-control-profile-cloud-based-it-services.html)_
- focus on the selection of security controls to those implemented in software components of information system solutions
- achieve threat protection objectives specified in the Cyber Centre’s Annex B Cyber Centre MEDIUM Cloud Profile Recommendations and the _[Government of Canada Security Control Profile for Cloud-Based GC Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-security-control-profile-cloud-based-it-services.html)_

## 2. Cloud Guardrails

This document focuses on a preliminary set of baseline security controls to ensure that the cloud service environment has a minimum set of configurations for the cloud environment. Departments are expected to must implement, validate, and report on in the first 30 business days.

Departments are responsible for implementing the minimum configurations identified in the table below. Validation of the guardrails will be performed by SSC Cloud Services Directorate. The [Standard Operating Procedure (SOP) on Validating Cloud Guardrails](https://www.gcpedia.gc.ca/gcwiki/images/1/19/SOP_for_Validating_Cloud_Guardrails.pdf) has been developed to support this activity.

For this document the following definitions will be used:

- Mandatory requirements: A set of baseline security controls that departments must implement, validate, and report on in the first 30 business days.
- Additional considerations: Additional security controls that are highly recommended and should be taken into consideration. While these are not expected to be implemented within 30 business days, they include best practices that should be considered as departments progress with the establishment of their cloud-based environments.

| ID. | Cloud Guardrails                                                                      |
| --- | ------------------------------------------------------------------------------------- |
| 01  | [Protect User Accounts and Identities](EN/01_Protect-user-accounts-and-identities.md) |
| 02  | [Manage Access](EN/02_Manage-Access.md)                                               |
| 03  | [Secure Endpoints](EN/03_Secure-Endpoints.md)                                         |
| 04  | [Enterprise monitoring accounts](EN/04_Enterprise-Monitoring-Accounts.md)             |
| 05  | [Data location](EN/05_Data-Location.md)                                               |
| 06  | [Protection of data-at-rest](EN/06_Protect-Data-at-Rest.md)                           |
| 07  | [Protection of data-in-transit](EN/07_Protect-Data-in-Transit.md)                     |
| 08  | [Segment and separate](EN/08_Segmentation.md)                                         |
| 09  | [Network security services](EN/09_Network-Security-Services.md)                       |
| 10  | [Cyber defense services](EN/10_Cyber-Defense-Services.md)                             |
| 11  | [Logging and monitoring](EN/11_Logging-and-Monitoring.md)                             |
| 12  | [Configuration of cloud marketplaces](EN/12_Cloud-Marketplace-Config.md)              |
| 13  | [Plan for Continuity](EN/13_Plan-for-Continuity.md)                                   |

<!-- The [applicable scope for the guardrails](EN/00_Applicable-Scope.md) for the guardrails are based on cloud usage profiles. -->

### 3. Post 30 Days

Implementing the guardrails is the one of the first steps to establishing a secure cloud-based environment. The figure below provides an overview of the activities beyond the first 30 days that are needed to establish an up to and including Protected B environment within the context of an IaaS service model.

!["Figure 2‑1 Summary of Responsibilities](/image2.png "Figure 2‑1 Summary of Responsibilities")

Departments are expected to continue implementing the security requirements as outlined in:

- [Direction on the Secure Use of Commercial Cloud Services: Security Implementation Notice (SPIN)](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/direction-secure-use-commercial-cloud-services-spin.html)
- [Government of Canada Security Control Profile for Cloud-Based GC Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-security-control-profile-cloud-based-it-services.html)

Departments should engage with their IT Security Risk Management teams to obtain advice and guidance on integrating security assessment and authorization activities as part of the implementation of the GC cloud environment. The [Government of Canada Cloud Security Risk Management Approach and Procedures](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/cloud-security-risk-management-approach-procedures.html) outlines activities for Departments to consider as part of the departmental risk management activities.
SSC will perform periodic audits of the Departmental tenant environment to ensure ongoing compliance to the initial 30 days guardrails.

## 4. Cloud Usage Profiles

### 4.1 Overview of Cloud Usage Profiles

The following table describes various profiles for cloud usage by a GC organization.

| ID                                                                                                                                                                                                                                                                                                                                                                                             | Profile                                                                                                         | Description                                                                                                                                                                                                                                                                                                                                                                                              | Applicable Cloud Service Model |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------ |
| 1.                                                                                                                                                                                                                                                                                                                                                                                             | Experimentation/ Sandbox                                                                                        | <ul><li>Cloud-based services used for experimentation/sandbox</li><li>No direct system to system network interconnections required with GC data centers </li></ul>                                                                                                                                                                                                                                       | IaaS, PaaS, SaaS               |
| 2.                                                                                                                                                                                                                                                                                                                                                                                             | Non-sensitive cloud-based services                                                                              | <ul><li>Cloud-based services hosting non-sensitive GC content</li><li>No direct system to system network interconnections required with GC data centers</li></ul>                                                                                                                                                                                                                                        | IaaS, PaaS, SaaS               |
| 3a.                                                                                                                                                                                                                                                                                                                                                                                            | Sensitive (up to PB) cloud-based services                                                                       | <ul><li>Cloud-based services hosting sensitive (up to Protected B) information </li><li>No direct system to system network interconnections required with GC data centers</li></ul>                                                                                                                                                                                                                      | IaaS, PaaS, SaaS               |
| 3b.                                                                                                                                                                                                                                                                                                                                                                                            | Sensitive (up to PB) cloud-based services (Hybrid IT - Extension of GC Data Centers)                            | <ul><li>Cloud-based services hosting sensitive (up to Protected B) information.</li><li>GC cloud-based systems required to interact with systems in GC data centers</li><li>Restricted environment for GC users only</li><li>No external user connections to/from GC cloud-based virtual private cloud and no publicly accessible services</li></ul>                                                     | PaaS, SaaS                     |
| 4a.                                                                                                                                                                                                                                                                                                                                                                                            | Sensitive (up to PB) cloud-based services for GC-wide SaaS Solutions                                            | <ul><li>Cloud-based services hosting sensitive (up to Protected B) information for GC-wide enterprise applications (SaaS)</li><li>No direct system to system network interconnections required with GC data centers</li></ul>                                                                                                                                                                            | SaaS                           |
| 4b.                                                                                                                                                                                                                                                                                                                                                                                            | Sensitive (up to PB) cloud-based services for GC-wide SaaS Solutions (Hybrid IT - Extension of GC Data Centers) |
| <ul><li>Cloud-based services hosting sensitive (up to Protected B) information for GC-wide enterprise applications (SaaS)</li><li>GC cloud-based systems required to interact with systems in GC data centers</li><li>Restricted environment for GC users only</li><li>No external user connections to/from GC cloud-based virtual private cloud and no publicly accessible services</li></ul> | SaaS                                                                                                            |
| 5.                                                                                                                                                                                                                                                                                                                                                                                             | GC to GC only (Hybrid IT - Extension of GC Data Centers)                                                        | <ul><li>Hybrid IT environment with an extension of GC network to cloud-based virtual private cloud (up to Protected B) information </li><li>GC cloud-based systems required to interact with systems in GC data centers</li><li>Restricted environment for GC users only</li><li>No external user connections to/from GC cloud-based virtual private cloud and no publicly accessible services</li></ul> | IaaS, PaaS                     |
| 6.                                                                                                                                                                                                                                                                                                                                                                                             | Cloud-based services with External user access and interconnection to GC data centers                           | <ul><li>Cloud-based services hosting sensitive (up to Protected B) information </li><li>GC cloud-based systems required to interact with systems in GC data centers</li><li>Environment accessible for both GC users and External users and services</li><li>Solution implemented, managed and operated by a GC department/agency</li></ul>                                                              | IaaS, PaaS                     |

### 4.2 Guardrails Mapping to Cloud Usage Profiles

The following table describes the applicability of the initial 30 days guardrails to be applied to each of the cloud usage profiles. Within each departmental cloud tenant, there will be various information systems being provided. Each cloud sub-account or resource group should be tagged with the relevant cloud usage profile to ensure that appropriate policies and validation is performed.

| ID  | Cloud Guardrails                    | Applicable Service Model | Profile 1 – Experimentation/Sandbox       | Profile 2 – Non-sensitive cloud-based services | Profile 3 (a & b) – Sensitive (up to PB) cloud-based services | Profile 4 (a & b) – Sensitive (up to PB) cloud-based services for GC-wide SaaS Solutions | Profile 5 – GC to GC only (Hybrid IT - Extension of GC Data Centers) | Profile 6 – Cloud-based Service Accessible to External users (Connections to GC Data Centers Required) |
| --- | ----------------------------------- | ------------------------ | ----------------------------------------- | ---------------------------------------------- | ------------------------------------------------------------- | ---------------------------------------------------------------------------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| 1   | Protect user accounts and IDs       | IaaS, PaaS, SaaS         | Required (minimum for Privileged Users)   | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 2   | Manage access                       | IaaS, PaaS, SaaS         | Required                                  | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 3   | Secure endpoints                    | IaaS, PaaS, SaaS         | Recommended                               | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 4   | Enterprise Monitoring Accounts      | IaaS, PaaS, SaaS         | Required (for billing)                    | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 5   | Data location                       | IaaS, PaaS, SaaS         | Recommended                               | Recommended                                    | Required (in Canada for GC storage of PB and above)           | Required (in Canada for GC storage of PB and above)                                      | Required (in Canada for GC storage of PB and above)                  | Required (in Canada for GC storage of PB and above)                                                    |
| 6   | Protection of data-at-rest          | IaaS, PaaS, SaaS         | Not required                              | Recommended                                    | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 7   | Protection of data-in-transit       | IaaS, PaaS, SaaS         | Recommended                               | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 8   | Segment and separate                | IaaS, PaaS               | Required (network filtering at a minimum) | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 9   | Network security services           | IaaS, PaaS, SaaS         | Recommended                               | Required                                       | Required                                                      | Required (Restrict to GC only)                                                           | Required (Deny External Access policy – GC only)                     | Required                                                                                               |
| 10  | Cyber defense services              | IaaS, PaaS, SaaS         | Not required                              | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 11  | Logging and monitoring              | IaaS, PaaS, SaaS         | Recommended                               | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 12  | Configuration of Cloud Marketplaces | IaaS, PaaS, SaaS         | Required                                  | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |
| 13  | Plan for continuity                 | IaaS, PaaS, SaaS         | Not required                              | Required                                       | Required                                                      | Required                                                                                 | Required                                                             | Required                                                                                               |

## 5. References

### 5.1 Related policy instruments

- [Directive on Security Management](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=32611)
- [Direction on the Secure Use of Commercial Cloud Services: Security Implementation Notice (SPIN)](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/direction-secure-use-commercial-cloud-services-spin.html) 2017-01
- [Directive on Service and Digital, Appendix G: Standard on Enterprise Information Technology Service Common Configurations](https://www.tbs-sct.canada.ca/pol/doc-eng.aspx?id=32713)

### 5.2 Additional references

- [Government of Canada Security Control Profile for Cloud-based GC Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-security-control-profile-cloud-based-it-services.html)
- [Government of Canada Cloud Security Risk Management Approach and Procedures](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/cloud-security-risk-management-approach-procedures.html)
- [Security categorization guide and tool](http://www.gcpedia.gc.ca/gcwiki/images/6/66/Tool-Security_Categorization.zip) (accessible only on the Government of Canada network)
- [Government of Canada CCloud-based services hosting sensitive (up to Protected B) information yber Security Event Management Plan (GC CSEMP) 2018](https://www.canada.ca/en/treasury-board-secretariat/services/access-information-privacy/security-identity-management/government-canada-cyber-security-event-management-plan.html)
- [Concept case for digital projects](https://www.tbs-sct.gc.ca/pol-cont/doc/32593-eng.docx)
- [Enterprise security architecture (ESA) template guides](http://www.gcpedia.gc.ca/wiki/ESA_Template_Guides) (accessible only on the Government of Canada network)
- [Guideline on Defining Authentication Requirements](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=26262)
- [Guideline on Identity Assurance](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=30678)
- [Considerations for Cryptography in Commercial Cloud Services](https://www.canada.ca/en/government/system/digital-government/modern-emerging-technologies/cloud-services/government-canada-consideration-use-cryptography-in-cloud.html)
- [IT Security Risk Management: A Lifecycle Approach (ITSG33)](https://cyber.gc.ca/en/guidance/it-security-risk-management-lifecycle-approach-itsg-33)
- [Guidance on Securely Configuring Network Protocols (ITSP.40.062)](https://cyber.gc.ca/en/guidance/guidance-securely-configuring-network-protocols-itsp40062)
- [Baseline Security Requirements for Network Security Zones in the Government of Canada (ITSG-22)](https://cyber.gc.ca/en/guidance/baseline-security-requirements-network-security-zones-government-canada-itsg-22)
- [Network Security Zoning: Design Considerations for Placement of Services within Zones (ITSG-38)](https://cyber.gc.ca/en/guidance/network-security-zoning-design-considerations-placement-services-within-zones-itsg-38)
- [ITSP.50.104 Guidance on defence in depth for cloud-based services](https://cyber.gc.ca/en/guidance/itsp50104-guidance-defence-depth-cloud-based-services)

## How to Contribute

See [CONTRIBUTING.md](CONTRIBUTING.md)

## License

Unless otherwise noted, the source code of this project is covered under Crown Copyright, Government of Canada, and is distributed under the [MIT License](LICENSE).

The Canada wordmark and related graphics associated with this distribution are protected under trademark law and copyright law. No permission is granted to use them outside the parameters of the Government of Canada's corporate identity program. For more information, see [Federal identity requirements](https://www.canada.ca/en/treasury-board-secretariat/topics/government-communications/federal-identity-requirements.html).

---

<!-- markdownlint-disable MD024 MD025 -->

# Mesures de protection du nuage du GC
