---
Copyright:
  years: 2018, 2019
lastupdated: "2019-04-24"

subcollection: databases-for-postgresql

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# Security and Compliance
{: #security-compliance}

## Protection Against Unauthorized Access

{{site.data.keyword.databases-for-postgresql_full}} use the following methods to protect data in transit or in storage.
- All {{site.data.keyword.databases-for-postgresql}} connections use TLS/SSL encryption for data in transit. The current supported version of this encryption is TLS 1.2.
- Access to the Account, Management Console UI, and API is secured via [Identity and Access Management (IAM)](/docs/services/databases-for-postgresql?topic=cloud-databases-iam).
- Access to the database is secured through the standard access controls provided by the database. These access controls are configured to require valid database-level credentials that are obtainable only through prior access to the database or through our Management Console UI or API.
- All {{site.data.keyword.databases-for-postgresql}} storage is provided on storage encrypted with [{{site.data.keyword.keymanagementserviceshort}}](/docs/services/key-protect?topic=key-protect-about). Bring-your-own-key (BYOK) for encryption is also available through [Key Protect integration](/docs/services/databases-for-postgresql?topic=cloud-databases-key-protect)
- IP Whitelisting - All deployments support [whitelisting IP addresses](/docs/services/databases-for-postgresql?topic=cloud-databases-whitelisting) to restrict access to the service.
- Public and Private Networking - {{site.data.keyword.databases-for-postgresql}} is integrated with [Service Endpoints](/docs/services/databases-for-postgresql?topic=cloud-databases-service-endpoints). You can select whether to use connections over the public network, the {{site.data.keyword.cloud_notm}} internal network, or both.

## Data Resilience

- [Backups](/docs/services/databases-for-postgresql?topic=cloud-databases-dashboard-backups) are included in the service. {{site.data.keyword.databases-for-postgresql}} backups reside in [{{site.data.keyword.cos_full_notm}}](/docs/services/cloud-object-storage?topic=cloud-object-storage-about-ibm-cloud-object-storage) and are also [encrypted](/docs/services/cloud-object-storage?topic=cloud-object-storage-security).
- {{site.data.keyword.databases-for-postgresql}} deployments are configured with replication. Deployments contain a cluster with two data members. Both members contain a copy of your data using asynchronous replication, with a distributed consensus mechanism to maintain cluster state and handle failovers. 
- If you deploy to an [{{site.data.keyword.cloud_notm}} Single-Zone Region (SZR), each database node resides on a different host in the datacenter. 
- If you deploy to an {{site.data.keyword.cloud_notm}} Multi-Zone Region (MZR), the nodes are spread over the region's availability zone locations. 

## SOC 2 Type 1 Certification

{{site.data.keyword.IBM_notm}} provides a Service Organization Controls (SOC) 2 Type 1 report for {{site.data.keyword.databases-for-postgresql}}. The reports evaluate IBM's operational controls according to the criteria set by the American Institute of Certified Public Accountants (AICPA) Trust Services Principles. The Trust Services Principles define adequate control systems and establish industry standards for service providers such as IBM Cloud to safeguard their customers' data and information.

You can request an SOC 2 Type 1 report from the customer portal or contact your sales representative. Alternatively, you can open a support ticket with [IBM Cloud support](https://cloud.ibm.com/unifiedsupport/supportcenter){:new_window}

## General Data Protection Regulation (GDPR) 

If you have an account with IBM Cloud, your personal data is held by {{site.data.keyword.cloud_notm}}. The {{site.data.keyword.IBM_notm}} Data Processing Addendum (Addendum) applies to the processing of client's personal data by {{site.data.keyword.IBM_notm}} on behalf of client in order to provide {{site.data.keyword.IBM_notm}} standard services.  
[IBM DPA](https://www.ibm.com/support/customer/zz/en/dpa.html){:new_window}

{{site.data.keyword.databases-for-postgresql}} processes limited client Personal Information (PI) in the course of running the service and optimizing the user experience. 

{{site.data.keyword.databases-for-postgresql}} provides a [Data Sheet Addendum (DSA)](https://www.ibm.com/software/reports/compatibility/clarity-reports/report/html/softwareReqsForProduct?deliverableId=CD09D2E06DC811E8A0B560E89C071ECC){:new_window} with its policies as a Data Processor regarding content and data protection. 

## HIPAA

{{site.data.keyword.databases-for-postgresql}} meets the required {{site.data.keyword.IBM_notm}} controls that are commensurate with the Health Insurance Portability and Accountability Act of 1996 (HIPAA) Security and Privacy Rule requirements. These requirements include the appropriate administrative, physical, and technical safeguards required of Business Associates in 45 CFR Part 160 and Subparts A and C of Part 164. HIPAA must be requested at the time of provisioning and requires a representative to sign a Business Associate Addendum (BAA) agreement with {{site.data.keyword.IBM_notm}}.

## Terms

- [The IBM Privacy Policy](https://www.ibm.com/privacy/us/en/)
- [The IBM Cloud Notices and Terms of Use](/docs/overview/terms-of-use?topic=overview-terms)


