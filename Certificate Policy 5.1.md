#Thailand National Root Certification Authority
#Certificate Policy
#Version 5.1
#Certificate Policy Identifier (OID): 2.16.764.1.1.1

1	Introduction
1.1	Overview
The Electronic Transactions Act sets out the legal framework for the public key infrastructure (PKI) with the objective of facilitating the use of electronic transactions in a secure manner for commercial and other purposes. The PKI is composed of many elements, including legal obligations, policies, hardware, software, databases, networks, personnel, and operating procedures. The center of trust in the PKI is Certification Authority (CA), who issues a digital certificate to a person or legal entity (who may be another CA) by using a collection of hardware, software, personnel, and operating procedures. The digital certificate will bind a public key to that person or legal entity. It allows Relying Parties to trust signatures or assertions made by the person or legal entity using the private key that corresponds to the public key contained in the certificate. A digital certificate when combined with private key can be used to verify the identity in electronic transactions using the Digital Signature mechanism. Any person or legal entity who wishes to use a digital certificate MUST pass the Certification Authority’s authentication procedures.
In an environment where there are multiple Certification Authorities, certificate usage and authentication will be troublesome if the Certification Authorities are not in a Trust Relationship model. The basic way to solve the problem is to build a trust relationship between each pair of Certification Authorities, which will be unmanageable in the long run. Therefore, the Electronic Transactions Commission (ETC) has agreed to form a trust relationship in the hierarchical model for all Certification Authorities in Thailand.
In 2007 (B.E. 2550), the Ministry of Information and Communication Technology (MICT) has established the Thailand National Root Certification Authority or Thailand NRCA with the objective to centralize the management of trust relationship and serve as the hub of trust, so called Trust Anchor, so that certificates issued by Subordinate Certification Authorities can seamlessly work together both locally and internationally.
A Certificate Policy (CP) is the principal statement of policy governing the Thailand NRCA. The CP applies to all Subordinate Certification Authorities under Thailand NRCA and thereby provides assurances of uniform trust throughout the Thailand NRCA. The CP sets forth requirements that Subordinate Certification Authorities under Thailand NRCA MUST meet. 
The mission of Thailand NRCA includes:
•	Certificate issuance, publication, and revocation for certification authorities located in Thailand; and
•	Coordinating with overseas certification authorities to enable seamlessly international usage of certificates issued by local certification authorities.
The purpose of this document is to identify a baseline set of security controls and practices to support the secure issuance of certificates. This baseline set of controls has been written in the form of the CP. As defined by ITU Recommendation X.509, a Certificate Policy is “a named set of rules that indicates the applicability of a certificate to a particular community and/or class of application with common security requirements.” That is, a Certificate Policy defines the expectations and requirements of the Relying Party community that will trust the certificates issued by its CAs. The governance structure that represents the Relying Party is known as a Policy Authority (PA). As such, the PA is responsible for identifying the appropriate set of requirements for a given community and oversees the CAs that issue certificates for that community. CAs which are operated under Thailand NRCA Trust Model MUST conform to this Certificate Policy.
Thailand NRCA conforms to the current versions of both the SSL/TLS and S/MIME Baseline Requirements for the Issuance and Management of Publicly Trusted Certificates, and the Network and Certificate System Security Requirements published at http://www.cabforum.org, and the current version of the CCADB Policy published at https://www.ccadb.org/policy. In the event of any inconsistency between this document and those requirements, those requirements take precedence over this document.
This Certificate Policy is consistent with the Internet Engineering Task Force (IETF) Public Key Infrastructure X.509 (IETF PKIX) Certificate Policy and Certificate Practices Framework [RFC 3647].
Thailand NRCA in this CP supports the following types of SSL/TLS Certificates:
Type of Certificate	Policy OID
SSL/TLS – Domain Validation	2.23.140.1.2.1
SSL/TLS – Organization Validation	2.23.140.1.2.2
SSL/TLS – Individual Validation	2.23.140.1.2.3
Table 1: Type of SSL/TLS Certificate
Thailand NRCA in this CP supports the following types of S/MIME Certificates:
Type of Certificate	Generation	Policy OID
S/MIME – Mailbox Validation	Multipurpose	2.23.140.1.5.1.2
S/MIME – Mailbox Validation	Strict	2.23.140.1.5.1.3
S/MIME – Organization Validation	Multipurpose	2.23.140.1.5.2.2
S/MIME – Organization Validation	Strict	2.23.140.1.5.2.3
S/MIME – Sponsor Validation	Multipurpose	2.23.140.1.5.3.2
S/MIME – Sponsor Validation	Strict	2.23.140.1.5.3.3
S/MIME – Individual Validation	Multipurpose	2.23.140.1.5.4.2
S/MIME – Individual Validation	Strict	2.23.140.1.5.4.3
Table 2: Type of S/MIME Certificates 
