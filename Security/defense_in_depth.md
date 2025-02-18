<u>Defense in Depth</u> is a <b>security strategy</b> that is common on AWS.
- uses multiple redundant defenses to protect your AWS accounts, workloads, data, and assets

Different Layers of Security on AWS:
1. Data Layer :
   1.1. Data at Rest : Encrypted using AWS Key Management Service : KMS service. Also ensure all data and models are versioned and backed up using S3 Versioning.
   1.2. Data at Transit: Services for encrypting data in transit include AWS Certificate Manager (<u>ACM</u>) and AWS Private Certificate Authority (AWS Private CA).
         Keep data within virtual private clouds (VPCs) using AWS PrivateLink.

2. Identity and Access Management (IAM) to ensure proper access to different services
3. Application Protection (services like AWS Shield, Amazon Cognito) ensure protection against data breaches, unauthorized access and Denial-of-Service (DoS)
4. Network and Edge Protection : protection of Infrastructure and boundaries of cloud env using AWS VPC (Cirtual Private Cloud) and AWS WAF (Web Application Firewall)
5. Infrastructure Protection : IAM, and ACLs (Access Control Lists)
6. Threat Detection (AWS Security Hub, Amazon GuardDuty) and Incident Response (AWS Lambda, Amazon EventBridge)
7. Implement protocol of Least Priviledge to limit access to absolute necessary

