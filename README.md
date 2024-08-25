# Security+

### Control categories


![Professor Messer - Security Controls - CompTIA Security+ SY0-701 - 1 1  STM3EUvL7wg - 1280x720 - 6m24s](https://github.com/user-attachments/assets/561c7512-14bd-4742-84c1-d2beffdee3d6)
![Professor Messer - Security Controls - CompTIA Security+ SY0-701 - 1 1  STM3EUvL7wg - 1280x720 - 6m24s](https://github.com/user-attachments/assets/8d27eb0c-5410-47aa-bc71-fc8eaf9ffb59)

![Professor Messer - Security Controls - CompTIA Security+ SY0-701 - 1 1  STM3EUvL7wg - 1280x720 - 6m36s](https://github.com/user-attachments/assets/6301a5b6-aa85-4d74-8720-e5ec4b3ad5e7)

![Professor Messer - Security Controls - CompTIA Security+ SY0-701 - 1 1  STM3EUvL7wg - 1280x720 - 10m37s](https://github.com/user-attachments/assets/ce17f29a-b290-4cc3-93d4-ea32ef82e102)

### Security controls

THE CIA TRIAD

## Non-repudiation
Non-repudiation is a key concept in cybersecurity and cryptography, particularly in the context of ensuring the integrity and authenticity of information. It is one of the core principles of information security, alongside confidentiality, integrity, and availability (often abbreviated as CIA).

### Definition:
**Non-repudiation** is the assurance that someone cannot deny the validity of their actions or the origin of a particular piece of data. In the context of digital communications, it means that once a party sends a message or performs an action, they cannot credibly deny having done so.

### Detailed Explanation:
- **Digital Signatures:** One of the most common mechanisms to achieve non-repudiation is through the use of digital signatures. A digital signature is a cryptographic value that is created using the sender's private key. When a sender signs a message or document digitally, they create a unique signature based on the content of that message and their private key. The recipient can verify this signature using the sender's public key. Because only the sender has access to their private key, the signature provides proof that the sender indeed sent the message.

- **Public Key Infrastructure (PKI):** Non-repudiation is often enforced using a PKI, which provides the necessary framework for managing digital certificates and keys. A certificate authority (CA) vouches for the authenticity of the public keys, adding an additional layer of trust.

- **Audit Trails and Logs:** Non-repudiation is also supported by maintaining secure and tamper-proof audit trails and logs. These records can be used to prove that a particular action was taken by a specific user or system at a given time.

- **Legal and Contractual Importance:** In legal contexts, non-repudiation can be critical. For example, in e-commerce, non-repudiation ensures that a buyer cannot deny making a purchase, and a seller cannot deny having received payment. Similarly, in email communication, non-repudiation can prevent someone from denying that they sent a particular message.

### Example Scenario:
Consider an online banking transaction. When you initiate a transfer, the bank’s system generates a digital record of the transaction, including your digital signature (or some form of authentication). This record is stored securely. If you later claim that you did not authorize the transaction, the bank can produce this record, showing that the transaction was indeed initiated by you, based on the digital signature. This ensures non-repudiation.

### Related Concepts:
- **Authentication:** Ensuring that the entity (user or system) is who they claim to be.
- **Integrity:** Ensuring that the data has not been altered or tampered with.
- **Confidentiality:** Ensuring that the data is accessible only to those authorized to access it.
- **Authorization:** Ensuring that an authenticated entity has the necessary permissions to perform a specific action.

### Additional Information:
- **Challenge-Response Systems:** These systems are often used in conjunction with digital signatures to provide an additional layer of non-repudiation.
- **Hash Functions:** A hash function is often used in creating digital signatures, as it allows the creation of a unique identifier for a set of data. If the data is altered, the hash changes, invalidating the signature.
- **Time Stamping:** Adding a time stamp to a digital signature can strengthen non-repudiation by recording the exact time an action was performed, making it even harder to dispute the action later.

Understanding non-repudiation and its mechanisms is crucial for passing the CompTIA Security+ exam, as well as for practical applications in the field of cybersecurity.
------------
### Proof of Integrity
![Professor Messer - Non-repudiation - CompTIA Security+ SY0-701 - 1 2  XxnCxPEllMg - 1280x720 - 1m31s](https://github.com/user-attachments/assets/4ddd7495-7cfe-4091-acd8-05fd6a187ca5)

- 

### Proof of Origin
**Proof of Origin** is a concept in cybersecurity that ensures data or a message can be traced back to its original source. It's closely related to authentication and non-repudiation, ensuring that the sender of a message or the creator of a piece of data can be verified and held accountable.

### Definition:
**Proof of Origin** refers to the mechanisms used to verify the identity of the sender of a message or the creator of a document. It guarantees that the origin of a piece of data or communication is authentic and can be confirmed as coming from a specific source.

### Detailed Explanation:
- **Digital Signatures:** One of the most effective methods for providing proof of origin is through digital signatures. When a sender digitally signs a message or document, they use their private key to create a signature that is unique to both the sender and the content. This signature can be verified by anyone using the sender's public key, proving that the message indeed originated from the sender and has not been altered.

  - **How It Works:** When a sender wants to provide proof of origin, they first create a hash of the message or document. Then, they encrypt this hash with their private key to create the digital signature. The recipient can decrypt this signature using the sender's public key, compare the decrypted hash to the hash they compute from the received message, and verify that the message is authentic and came from the claimed sender.

- **Public Key Infrastructure (PKI):** PKI plays a crucial role in enabling proof of origin. Within a PKI, digital certificates issued by a trusted Certificate Authority (CA) bind public keys to individuals or organizations. When someone receives a message signed with a digital signature, they can trust the origin if the public key is associated with a valid certificate.

- **Email Authentication Protocols:** Protocols such as **DKIM (DomainKeys Identified Mail)** and **SPF (Sender Policy Framework)** provide proof of origin for emails. These protocols help verify that an email actually came from the domain it claims to be from, reducing the likelihood of email spoofing and phishing attacks.

- **MAC (Message Authentication Code):** A MAC is another mechanism that can provide proof of origin, particularly in symmetric encryption systems. It uses a shared secret key to generate a code that both the sender and receiver can use to verify the authenticity of the message's origin. If the MAC matches, it confirms that the message originated from someone with access to the shared key.

### Example Scenario:
Imagine you're receiving an important legal document via email. The sender has digitally signed the document using their private key. Upon receiving it, you use the sender's public key to verify the signature. If the signature is valid, you have proof that the document indeed originated from the sender and was not altered during transmission.

### Related Concepts:
- **Non-repudiation:** Closely related to proof of origin, non-repudiation ensures that a sender cannot deny having sent a message. Proof of origin often relies on the same mechanisms (like digital signatures) to ensure that the sender cannot dispute their involvement.
  
- **Authentication:** While proof of origin specifically verifies the sender of a message, authentication broadly refers to verifying the identity of a user or device. Proof of origin is a form of authentication focused on the source of data.

- **Confidentiality:** Proof of origin often works alongside confidentiality to ensure that only authorized parties can access and verify the source of a message.

### Additional Information:
- **Digital Certificates:** In many secure communication systems, digital certificates play a vital role in proving the origin. A certificate binds a public key to an entity, ensuring that anyone who verifies a signature using that public key can trust that it belongs to the claimed sender.

- **Blockchain:** In blockchain technology, proof of origin can be ensured through the decentralized and transparent nature of the ledger. Every transaction or block added to the chain is verifiable and can be traced back to its origin, ensuring that the data's source is authentic.

- **Email Headers:** In emails, examining headers can help determine the origin of the message. Email headers contain information about the path the email took from the sender to the recipient, which can help in verifying the origin.

Understanding proof of origin is crucial for ensuring trust in digital communications and transactions, making it a vital concept for your Security+ exam and practical cybersecurity applications.


**Digital Signature Process**

## Authentication, Authorization, and Accounting - CompTIA Security+ SY0-701 - 1.2
1.The **Authentication, Authorization, and Accounting (AAA)** framework is a fundamental concept in cybersecurity, including the CompTIA Security+ SY0-701 exam. AAA is essential for managing user access to network resources, ensuring that only authorized individuals can access certain data, perform specific actions, and that all access and actions are logged and monitored.

### 1. **Authentication**
**Authentication** is the process of verifying the identity of a user, device, or entity trying to access a system or network. It answers the question, "Who are you?"

#### Key Points:
- **Credentials:** Authentication typically involves the use of credentials, such as passwords, biometrics, smart cards, or digital certificates, that a user must provide to prove their identity.
  - **Something You Know:** Passwords, PINs, security questions.
  - **Something You Have:** Smart cards, security tokens, mobile devices (for one-time passwords or multi-factor authentication).
  - **Something You Are:** Biometrics like fingerprints, retina scans, or facial recognition.
  - **Somewhere You Are:** Location-based authentication (e.g., IP address or GPS coordinates).
  - **Something You Do:** Behavioral biometrics, such as typing patterns or voice recognition.

- **Multi-Factor Authentication (MFA):** Combines two or more types of authentication methods to increase security. For example, using both a password and a fingerprint scan.
  
- **Single Sign-On (SSO):** Allows users to authenticate once and gain access to multiple systems without needing to log in again for each one.

#### Example:
When you log into your email account, you enter a username and password. The system checks these credentials against its database to confirm your identity. If correct, you are authenticated and granted access to your email.

### 2. **Authorization**
**Authorization** is the process of determining what an authenticated user is allowed to do. It answers the question, "What can you do?"

#### Key Points:
- **Access Control Models:**
  - **Discretionary Access Control (DAC):** The resource owner decides who can access the resource.
  - **Mandatory Access Control (MAC):** Access is controlled by a central authority based on multiple criteria, such as security clearances.
  - **Role-Based Access Control (RBAC):** Access is determined by the user's role within an organization. For example, an administrator has more privileges than a regular user.
  - **Attribute-Based Access Control (ABAC):** Access is based on a combination of attributes (e.g., user, resource, environment).

- **Least Privilege Principle:** Users are given the minimum levels of access—or permissions—necessary to perform their job functions.

- **Privilege Creep:** Over time, users may accumulate access rights that they no longer need, which can become a security risk. Regular audits help prevent this.

#### Example:
After logging into a network, a user may be authorized to access specific files and folders, but not others. An employee in the HR department might have access to payroll files, while a marketing employee does not.

### 3. **Accounting**
**Accounting** (also known as **Auditing**) involves tracking and logging user activities on a network. It answers the questions, "What did you do?" and "When did you do it?"

#### Key Points:
- **Audit Logs:** These logs record details about user activities, such as successful and failed login attempts, file access, system changes, and more. They are essential for forensic analysis in case of a security incident.
  
- **Monitoring:** Continuous monitoring of user actions can help detect unusual or unauthorized behavior, such as a user accessing files outside of their normal work hours.

- **Compliance:** Many industries have regulations that require detailed logging of activities for compliance purposes. For example, healthcare organizations must comply with HIPAA, which mandates strict controls over patient data access and auditing.

- **Incident Response:** Accounting data is crucial during an incident investigation to understand what happened, who was involved, and how to prevent future occurrences.

#### Example:
If a breach occurs, the IT team can review the audit logs to determine which accounts were accessed, what files were viewed or modified, and the time and date of these actions.

### AAA Framework in Context:
- **RADIUS (Remote Authentication Dial-In User Service):** A protocol that provides centralized Authentication, Authorization, and Accounting management for users who connect and use a network service.
  
- **TACACS+ (Terminal Access Controller Access-Control System Plus):** A protocol that handles authentication, authorization, and accounting separately, allowing for more granular control over the AAA process.

- **LDAP (Lightweight Directory Access Protocol):** Often used in conjunction with AAA to store user credentials and permissions in a centralized directory.

### Summary:
The AAA framework is crucial for securing networks by ensuring that only authenticated users gain access, that these users are authorized to perform certain actions, and that all actions are accounted for through logging and monitoring. Understanding and implementing AAA is essential for protecting information systems, making it a core concept for the CompTIA Security+ exam and real-world cybersecurity practices.

## Every department needs to have a log.

## Gap Analysis - CompTIA Security+ SY0-701 - 1.2
### Comparing the current security posture with the desired goal of organizaitons security
**Gap Analysis** is an essential process in cybersecurity, particularly within the context of the CompTIA Security+ exam (SY0-701), and it's a key component of an organization's overall risk management and security posture assessment. It involves comparing the current state of an organization's security controls and practices against a desired or required standard, such as regulatory requirements, best practices, or organizational goals, to identify gaps where improvements are needed.

### Definition:
**Gap Analysis** is the process of comparing the current security posture of an organization with desired or required standards to identify gaps in security controls, processes, or policies. The goal is to determine areas of weakness or non-compliance that need to be addressed to enhance security and reduce risk.

### Detailed Explanation:
- **Current State Assessment:**
  - The first step in a gap analysis is to thoroughly assess the organization's current security measures, controls, and processes. This includes reviewing policies, procedures, technology implementations, and user practices.
  - Tools such as security audits, vulnerability assessments, and penetration tests are often used to gather data on the current state of security.

- **Benchmarking Against Standards:**
  - The next step is to compare the current state to a standard or benchmark. This benchmark could be:
    - **Regulatory Requirements:** Such as GDPR, HIPAA, or PCI-DSS, which mandate specific security controls.
    - **Industry Best Practices:** Frameworks like NIST Cybersecurity Framework, ISO/IEC 27001, or CIS Controls.
    - **Organizational Goals:** Internal security policies or strategic objectives that the organization aims to achieve.

- **Identification of Gaps:**
  - The comparison highlights gaps, which are areas where the current security measures do not meet the required or desired standards. These gaps could be technical, such as outdated software, or procedural, such as the absence of a formal incident response plan.
  - Gaps may also be found in compliance, where the organization fails to meet legal or regulatory requirements.

- **Risk Assessment:**
  - Once gaps are identified, they are typically analyzed in terms of risk. This involves determining the potential impact of these gaps on the organization, including the likelihood of exploitation and the severity of consequences.
  - Prioritizing gaps based on risk allows the organization to address the most critical vulnerabilities first.

- **Remediation Planning:**
  - After identifying and assessing the gaps, the organization develops a plan to address them. This plan may include implementing new security controls, updating policies, providing employee training, or investing in new technologies.
  - The remediation plan should include timelines, resource allocation, and responsibilities.

- **Continuous Monitoring and Improvement:**
  - Gap analysis is not a one-time process. Continuous monitoring and regular reassessments are crucial to ensuring that new gaps do not emerge as the organization evolves and as threats change.

### Example Scenario:
Consider a financial institution that wants to comply with the Payment Card Industry Data Security Standard (PCI-DSS). The organization performs a gap analysis by comparing its current security controls with the requirements of PCI-DSS.

- **Current State:** The organization reviews its data encryption practices, access control mechanisms, and network security measures.
- **Benchmark:** PCI-DSS requirements.
- **Gap Identification:** The gap analysis reveals that while the organization encrypts stored data, it lacks encryption during data transmission, which is a PCI-DSS requirement.
- **Risk Assessment:** The risk of data interception during transmission is assessed as high.
- **Remediation:** The organization implements TLS encryption for data in transit and updates its security policies to reflect this change.

### Related Concepts:
- **Risk Assessment:** Gap analysis is often a part of a broader risk assessment, where identified gaps contribute to understanding the organization’s overall risk posture.
  
- **Security Audits:** Security audits often lead to gap analysis by identifying areas where current security practices fall short of requirements or best practices.
  
- **Compliance Audits:** Compliance gap analysis focuses specifically on identifying discrepancies between current practices and regulatory or legal requirements.

- **Vulnerability Management:** Gap analysis can highlight gaps in vulnerability management processes, such as missing patches or unprotected systems.

### Benefits of Gap Analysis:
- **Improved Security Posture:** By identifying and addressing gaps, organizations can enhance their overall security and reduce vulnerabilities.
  
- **Regulatory Compliance:** Helps ensure that the organization meets all relevant legal and regulatory requirements.
  
- **Resource Allocation:** Allows for better prioritization and allocation of resources by focusing on the most critical gaps first.

- **Strategic Planning:** Provides a clear roadmap for achieving long-term security goals and aligning security practices with business objectives.

### Summary:
Gap Analysis is a crucial process for identifying weaknesses in an organization’s security framework and is fundamental to maintaining compliance, enhancing security, and managing risk effectively. For the CompTIA Security+ SY0-701 exam, understanding how gap analysis fits into the broader context of security assessments and risk management is essential.

- requires many communication
- choosing a comparision like framework or laws
- 
![Professor Messer - Gap Analysis - CompTIA Security+ SY0-701 - 1 2  cuTVyyS5C7M - 1048x590 - 5m29s](https://github.com/user-attachments/assets/c395d99f-e150-463b-b5cc-325228a539a7)

## Zero Trust - CompTIA Security+ SY0-701 - 1.2
**Zero Trust** is a security framework and strategy that assumes no user, device, or system, whether inside or outside the organization's network, should be trusted by default. Instead, every access request must be authenticated, authorized, and continuously validated based on a strict set of security policies before granting access to any resources. This approach is essential for modern cybersecurity, particularly in environments where traditional network perimeters are no longer sufficient due to the rise of cloud services, mobile devices, and remote work.

### Key Principles of Zero Trust:

1. **Never Trust, Always Verify:**
   - In a Zero Trust model, trust is never granted automatically, even for internal network traffic. Every access request, whether it comes from within the network or from an external source, must be verified.
   - Continuous verification is required, meaning that even after initial authentication, users and devices are re-verified at regular intervals or whenever they request access to new resources.

2. **Least Privilege Access:**
   - Users and devices are granted the minimum level of access necessary to perform their tasks, reducing the attack surface and limiting potential damage if credentials are compromised.
   - Access controls are granular and based on the principle of least privilege, meaning that users are only given access to the data and resources they specifically need.

3. **Micro-Segmentation:**
   - Network resources are divided into small segments, often down to individual workloads or devices, each with its own access policies.
   - This approach limits the lateral movement of attackers within a network. If a breach occurs, it is confined to a small segment rather than spreading unchecked across the network.

4. **Multi-Factor Authentication (MFA):**
   - MFA is a critical component of Zero Trust, requiring users to provide multiple forms of verification (e.g., something they know, something they have, and something they are) before access is granted.
   - This reduces the likelihood of unauthorized access, even if a password is compromised.

5. **Continuous Monitoring and Logging:**
   - All user activities, access requests, and network traffic are continuously monitored and logged to detect suspicious behavior and potential security incidents.
   - Real-time analytics and threat detection tools are used to analyze these logs and provide immediate responses to threats.

6. **Device Security:**
   - Devices accessing the network must be authenticated and verified as secure, including checks for up-to-date security patches, compliant configurations, and security software.
   - The security posture of devices is constantly assessed to ensure they do not introduce vulnerabilities into the network.

7. **Dynamic and Adaptive Policies:**
   - Zero Trust policies are dynamic and adapt based on context, such as the user’s role, location, device security status, and the sensitivity of the data being accessed.
   - Policies can adjust in real-time based on changing conditions, such as detecting an unusual login location or device anomaly.

### Zero Trust in Practice:

- **Identity and Access Management (IAM):** Zero Trust requires robust IAM systems that enforce MFA, role-based access control (RBAC), and continuous user verification.
- **Endpoint Security:** Devices must meet security standards before being allowed to access the network. This might involve device health checks and ensuring the latest security updates are installed.
- **Data Protection:** Data is encrypted both at rest and in transit, and access is tightly controlled. Zero Trust ensures that sensitive data is only accessible to those who need it and under secure conditions.
- **Network Security:** The traditional perimeter-based defense is replaced with micro-segmentation and strict access controls at each layer of the network.

### Benefits of Zero Trust:

- **Reduced Attack Surface:** By eliminating implicit trust, Zero Trust significantly reduces the potential points of entry for attackers.
- **Improved Security Posture:** Continuous verification and least privilege access help protect against both external and insider threats.
- **Enhanced Compliance:** Zero Trust frameworks often help organizations meet stringent compliance requirements by ensuring data access is tightly controlled and monitored.
- **Flexibility:** Zero Trust is well-suited for modern IT environments, including cloud-based services, remote work, and Bring Your Own Device (BYOD) policies.

### Challenges of Zero Trust:

- **Complex Implementation:** Deploying a Zero Trust model can be complex, requiring significant changes to existing network architectures and security practices.
- **User Experience:** Frequent authentication requests may disrupt user experience, although adaptive authentication techniques can mitigate this.
- **Integration with Legacy Systems:** Legacy systems and applications may not easily support Zero Trust principles, requiring additional workarounds or upgrades.

### Zero Trust and the CompTIA Security+ SY0-701 Exam:

Understanding Zero Trust is crucial for the Security+ exam, as it reflects modern security best practices. Exam objectives related to Zero Trust include recognizing the importance of access control models, understanding secure network design, and knowing how to implement security measures that protect against advanced threats.

### Summary:

Zero Trust is a security framework that emphasizes strict verification, least privilege, and continuous monitoring, regardless of whether a user or device is inside or outside the network perimeter. It is designed to enhance security in an era where traditional perimeter defenses are no longer sufficient, making it a key concept in both cybersecurity practice and the CompTIA Security+ certification.
![Professor Messer - Zero Trust - CompTIA Security+ SY0-701 - 1 2  zC_Pndpg8-c - 1048x590 - 2m43s](https://github.com/user-attachments/assets/74389b9c-ab10-418b-af92-f6ff4207a806)

- The way it is done is taking all devices and dividing it into small components
- Controlling trust is 

These terms are central to the **Zero Trust** security model and are crucial for understanding how trust and access are controlled in a Zero Trust environment. Below is an explanation of each concept:

### 1. **Controlling Trust**
In the Zero Trust model, trust is not automatically granted based on the location of a user or device within the network. Instead, trust is controlled dynamically and is constantly reassessed based on various factors such as user identity, device security posture, and behavior. The core idea is that no entity is trusted by default, whether it is inside or outside the network.

#### Key Aspects:
- **Dynamic Trust Levels:** Trust is not static but is adjusted in real-time based on context (e.g., user behavior, location, time of access).
- **Continuous Verification:** Every access request is verified at the time of the request and continuously monitored during the session.
- **Minimization of Implicit Trust:** Even previously authenticated users and devices are subject to ongoing verification.

### 2. **Security Zones**
Security zones are a method of segmenting a network into different areas, each with specific security policies and controls. In a Zero Trust architecture, these zones are tightly controlled, and movement between zones is highly regulated.

#### Key Aspects:
- **Micro-Segmentation:** The network is divided into small, isolated segments (zones), each with its own security controls. This limits lateral movement within the network.
- **Policy Enforcement:** Each zone has specific access controls and policies, ensuring that only authorized users and devices can access resources within that zone.
- **Least Privilege:** Access within and between zones is granted based on the principle of least privilege, meaning users and devices have the minimum access necessary to perform their tasks.

#### Example:
A corporate network might be divided into several security zones, such as:
- **User Zone:** Where general employee workstations reside.
- **Sensitive Data Zone:** Where critical databases and servers are located.
- **External Access Zone:** For guest Wi-Fi and public-facing applications.

Access between these zones is tightly controlled, and policies are enforced at the boundaries to ensure security.

### 3. **Policy Enforcement Point (PEP)**
A Policy Enforcement Point (PEP) is a critical component of the Zero Trust architecture that is responsible for enforcing security policies whenever a user or device attempts to access a resource. The PEP intercepts access requests and applies the necessary controls as dictated by the security policy.

#### Key Aspects:
- **Access Control:** The PEP checks whether the request complies with the organization's security policies before granting or denying access.
- **Real-Time Decision Making:** The PEP operates in real-time, making instant decisions based on current security conditions and policies.
- **Scalability:** PEPs are deployed throughout the network, including at firewalls, routers, and other network devices, ensuring comprehensive policy enforcement.

#### Example:
When an employee tries to access a secure database, the request passes through a PEP. The PEP checks the user's identity, the security posture of their device, and other contextual information before allowing access.

### 4. **Policy Decision Point (PDP)**
The Policy Decision Point (PDP) is the component in the Zero Trust architecture that makes the actual decision on whether to grant or deny access to a resource. It uses predefined policies to evaluate the request and determines the appropriate action. The PDP works closely with the PEP, which enforces the decisions made by the PDP.

#### Key Aspects:
- **Centralized Policy Management:** The PDP centralizes the logic and rules that determine access, making it easier to manage and update security policies.
- **Contextual Evaluation:** The PDP evaluates various factors such as user identity, role, device security posture, time, location, and behavior to make informed decisions.
- **Policy Consistency:** Ensures that access decisions are consistent across the network, as all decisions are based on the same set of policies.

#### Example:
In the same scenario where an employee requests access to a secure database, the PEP forwards the request to the PDP. The PDP then checks if the request meets the security policies (e.g., the user's role and the device's security status) and decides whether to allow or deny access.

### How These Concepts Interact in a Zero Trust Model:
- **User Requests Access:** A user or device requests access to a resource.
- **PEP Intercepts the Request:** The request is intercepted by the Policy Enforcement Point (PEP), which checks if the request complies with the security policies.
- **PDP Evaluates the Request:** The PEP sends the request to the Policy Decision Point (PDP) for evaluation. The PDP uses a set of predefined rules to assess the request's legitimacy.
- **PDP Makes a Decision:** The PDP decides whether to grant or deny access based on the evaluation.
- **PEP Enforces the Decision:** The PEP enforces the PDP’s decision by either allowing or blocking the access request.
- **Continuous Monitoring:** Even after access is granted, the system continuously monitors the session to ensure ongoing compliance with security policies.

### Summary:
- **Controlling Trust**: In a Zero Trust model, trust is dynamically controlled and continuously verified.
- **Security Zones**: Networks are segmented into security zones, with strict access controls between them.
- **Policy Enforcement Point (PEP)**: The PEP enforces security policies by controlling access to resources.
- **Policy Decision Point (PDP)**: The PDP makes access decisions based on predefined security policies and contextual information.

These components work together to implement a Zero Trust architecture, ensuring that every access request is rigorously validated and monitored, reducing the risk of unauthorized access and improving overall network security. 





![Professor Messer - Zero Trust - CompTIA Security+ SY0-701 - 1 2  zC_Pndpg8-c - 1048x590 - 9m22s](https://github.com/user-attachments/assets/7e149393-2bd8-498a-9c08-d5dcc2f3c10f)


















------------------------------------------------









Security+
