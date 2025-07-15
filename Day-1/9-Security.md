## 9. Security in the Cloud

Security in the cloud is a shared responsibility between the **cloud provider** and the **customer**. While providers secure the underlying infrastructure, customers must secure their applications, data, and configurations.

---

### 9.1 Shared Responsibility Model

| Responsibility Area        | Cloud Provider        | Cloud Customer         |
|----------------------------|------------------------|-------------------------|
| Physical data center       | ✅                    | ❌                     |
| Network infrastructure     | ✅                    | ❌                     |
| Virtualization layer       | ✅                    | ❌                     |
| Operating system           | ❌ (IaaS)              | ✅                     |
| Applications               | ❌                    | ✅                     |
| Data encryption & access   | ❌                    | ✅                     |
| Identity and access (IAM)  | ❌                    | ✅                     |

> *Note: In SaaS, the provider takes on more responsibility. In IaaS, the customer handles more.*

---

### 9.2 Identity and Access Management (IAM)

- Central to cloud security.
- **Principle of Least Privilege (PoLP)**: Users and services get only the access they need.
- **MFA (Multi-Factor Authentication)** adds an extra layer of protection.

**Examples**: AWS IAM, Azure AD, GCP IAM

---

### 9.3 Encryption

- **At-rest encryption**: Data stored on disks is encrypted.
- **In-transit encryption**: Data moving between services is encrypted (e.g., HTTPS, TLS).
- Most cloud providers support **customer-managed keys (CMK)** and **hardware security modules (HSMs)**.

---

### 9.4 Network Security

- **VPC (Virtual Private Cloud)**: Isolated networks within the cloud.
- **Security groups and firewalls**: Define rules for incoming/outgoing traffic.
- **Private endpoints**: Access services over private networks, not public internet.

---

### 9.5 Monitoring and Logging

- Logs are essential for detecting and responding to threats.

**Cloud-native tools**:
- AWS CloudTrail, GuardDuty
- Azure Monitor, Sentinel
- Google Cloud Logging, Security Command Center

---

### 9.6 Compliance and Certifications

Cloud providers adhere to strict compliance frameworks:

- **ISO 27001**, **SOC 1/2/3**
- **HIPAA**, **GDPR**, **FedRAMP**
- **PCI-DSS**, **FIPS**

Customers can inherit compliance posture by building on compliant platforms but must also configure workloads appropriately.

---

### 9.7 Threat Detection and Incident Response

- Use threat intelligence and AI to detect anomalies.
- **SIEM tools**: Centralize logs and generate alerts.
- Define **incident response plans** with roles and playbooks.

---

### 9.8 Data Loss Prevention (DLP)

- Prevent accidental or malicious leaks of sensitive data (e.g., PII, credit card numbers).
- Tools analyze content and apply rules to block or alert on violations.

---

### 9.9 Secure Software Supply Chain

- Verify software sources and use **signed container images**.
- Scan images for **vulnerabilities** before deployment.
- Use **policy enforcement** in CI/CD pipelines (e.g., OPA, Kyverno).

---

### 9.10 Zero Trust Architecture

- **"Never trust, always verify"** approach.
- Every access request is authenticated, authorized, and encrypted.
- Applies to users, devices, apps, and services—internal or external.

---

### 9.11 Cloud Security Best Practices

- Use IAM roles, not access keys.
- Enforce MFA and role-based access control.
- Regularly patch systems and rotate secrets.
- Encrypt all sensitive data.
- Monitor continuously and set up alerts.
- Conduct security reviews and penetration testing.

---

> ✅ Cloud security is **not automatic**. It requires intentional design, constant vigilance, and a culture of security awareness.
