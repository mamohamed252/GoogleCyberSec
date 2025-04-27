# Principle of Least Privilege

## What is Least Privilege?

- The principle of least privilege is a security concept where a user is only given the minimum level of access needed to do their job.
- This approach minimizes risks associated with data breaches, accidental modifications, and unauthorized access.

## Implementing Least Privilege

- It involves identifying each user (person, device, or software) and determining the specific resources they need.
- Different account types (guest, user, service, privileged) have varying baseline access levels.

## Auditing Account Privileges

- Regular audits are crucial to maintain security and prevent privilege creep (users accumulating unnecessary access over time).
- **Usage audits** examine how accounts utilize resources.
- **Privilege audits** ensure user roles align with their access levels.
- **Account change audits** track modifications for suspicious activity.

---

# Data Governance and the Data Lifecycle

This document summarizes key concepts about data governance and the data lifecycle, emphasizing the importance of protecting sensitive information.

## Data Governance

- **Definition:** Data governance encompasses a set of processes that organizations use to manage information effectively. The primary goal is to ensure data privacy, accuracy, availability, and security throughout its lifecycle.

- **Key Roles:**
  - **Data Owner:** Determines who can access, modify, use, or delete their data.
  - **Data Custodian:** Responsible for the secure handling, transfer, and storage of data.
  - **Data Steward:** Implements and maintains data governance policies established by the organization.

## Data Lifecycle

- **Definition:** The data lifecycle is a crucial model in data security that outlines the different stages data goes through within an organization. Understanding these stages is essential for implementing appropriate security controls.

- **Stages:**
  - **Collect:** Gathering data from various sources.
  - **Store:** Securely storing data in appropriate systems.
  - **Use:** Accessing and utilizing data for business purposes.
  - **Archive:** Retaining data for compliance or historical purposes.
  - **Destroy:** Securely disposing of data that is no longer needed.

## Protecting Sensitive Information

- **Data Privacy:** Individuals have the right to control how their personal information is collected, used, and shared. Protecting data privacy is a fundamental ethical and legal obligation.

- **Regulations:** Various regulations and laws, such as HIPAA in the U.S. and GDPR in the EU, provide guidelines and mandates for protecting sensitive personal information.

- **Types of Sensitive Information:**
  - **PII (Personally Identifiable Information):** Information that can be used to identify an individual.
  - **PHI (Protected Health Information):** Data related to an individual's health or medical history.
  - **SPII (Sensitive Personally Identifiable Information):** A subset of PII that requires stricter security measures due to its sensitive nature (e.g., financial data, login credentials).

By adhering to data governance principles and understanding the data lifecycle, organizations can establish robust security measures to protect sensitive information and comply with relevant regulations.

---

# Information Privacy and Security

## Acronyms:

- **GDPR (General Data Protection Regulation):** A set of regulations by the European Union ensuring data owners have control over their personal information.
- **PCI DSS (Payment Card Industry Data Security Standard):** Security standards ensuring credit and debit card transactions are secure from data theft and fraud.
- **HIPAA (Health Insurance Portability and Accountability Act):** A U.S. law requiring the protection of sensitive patient health information.

## Summary:

This reading emphasizes the connection between information privacy and security, highlighting their distinct roles.

- **Privacy** focuses on user control over personal information.
- **Security** aims to safeguard that information.

The reading underscores the importance of both for building customer trust. Additionally, it introduces key regulations like GDPR, PCI DSS, and HIPAA, which provide guidelines for businesses to handle data responsibly. Organizations often use security audits and assessments to ensure compliance with these regulations and identify vulnerabilities.

---

# Introduction to Encryption

Previously, you learned these terms:

- **Encryption**: the process of converting data from a readable format to an encoded format
- **Public Key Infrastructure (PKI)**: an encryption framework that secures the exchange of online information
- **Cipher**: an algorithm that encrypts information

All digital information deserves to be kept private, safe, and secure. Encryption is one key to doing that! It is useful for transforming information into a form that unintended recipients cannot understand. In this reading, you’ll compare symmetric and asymmetric encryption and learn about some well-known algorithms for each.

---

## Types of Encryption

There are two main types of encryption:

### Symmetric Encryption

- Uses a **single secret key** to exchange information.
- The same key is used for both encryption and decryption.
- Both the sender and the receiver must have access to the secret key.

### Asymmetric Encryption

- Uses a **public and private key pair** for encryption and decryption.
- The **public key** encrypts data, and the **private key** decrypts it.
- The private key is only shared with authorized users.

---

## The Importance of Key Length

Ciphers are vulnerable to **brute force attacks**, which use trial and error to discover private information.

- **Longer key lengths** are more secure because they increase the number of possible combinations.
- However, **longer keys** can slow down processing times.
- **Short keys** are faster but less secure.

---

## Approved Algorithms

Many web applications combine symmetric and asymmetric encryption to balance security with user experience.

### Symmetric Algorithms

- **Triple DES (3DES)**:
  A block cipher that applies the DES algorithm three times using three different 56-bit keys, resulting in a 168-bit key. It is still used for backward compatibility but is being phased out.

- **Advanced Encryption Standard (AES)**:
  One of the most secure symmetric algorithms, using 128, 192, or 256-bit keys. Brute-forcing an AES 128-bit key could take billions of years.

### Asymmetric Algorithms

- **Rivest Shamir Adleman (RSA)**:
  One of the first asymmetric algorithms. Produces key sizes of 1,024, 2,048, or 4,096 bits. Used for protecting highly sensitive data.

- **Digital Signature Algorithm (DSA)**:
  Introduced by NIST in the 1990s. Commonly used with RSA in PKI, generating 2,048-bit keys.

---

## Generating Keys

Organizations use tools like **OpenSSL** to implement encryption algorithms and generate public/private key pairs.

- OpenSSL is an open-source command-line tool.
- Used for verifying digital certificates in PKI.
- In 2014, OpenSSL had a vulnerability known as the **Heartbleed bug**, which has since been patched.
- Secure, updated versions are widely used today.

---

## Obscurity is Not Security

According to **Kerckhoff’s Principle**, an encryption system should be secure even if everything about it (except the private key) is public.

- Transparency ensures systems can be independently verified.
- Secret or custom encryption algorithms are generally not secure and can be easily broken.

---

## Encryption is Everywhere

Organizations often use both symmetric and asymmetric encryption together:

- **Asymmetric encryption** secures small, sensitive data (e.g., login credentials).
- **Symmetric encryption** is used for the rest of a session due to its speed.

Encryption is increasingly mandated by law through regulations like:

- **Federal Information Processing Standards (FIPS 140-3)**
- **General Data Protection Regulation (GDPR)**

---

## Key Takeaways

- Symmetric encryption uses **one secret key**.
- Asymmetric encryption uses a **key pair** (public and private).
- Different encryption algorithms have different key lengths and strengths.
- Encryption helps meet **compliance regulations** and protect online data.

---

# Authentication Technologies: SSO and MFA

Most companies help keep their data safely locked up behind authentication systems. **Usernames and passwords** are the keys that unlock information for most organizations. But are those credentials enough? Information security often focuses on managing a user's **access** to, and **authorization** for, information.

Previously, you learned about the **three factors of authentication**:

- **Knowledge** (something you know)
- **Ownership** (something you have)
- **Characteristic** (something you are)

Two technologies that implement these authentication factors are:

- **Single Sign-On (SSO)**
- **Multi-Factor Authentication (MFA)**

---

## A Better Approach to Authentication

### What is SSO?

**Single Sign-On (SSO)** is a technology that combines several different logins into one. Companies are adopting SSO for several reasons:

- ✅ **Improves user experience**: Fewer passwords to remember
- 💰 **Lowers costs**: Streamlines management of connected services
- 🔒 **Improves security**: Reduces the number of access points for attackers

SSO emerged in the **mid-1990s** as a response to **password fatigue**, where users reuse the same passwords across services—a significant security risk.

---

## How SSO Works

SSO automates trust between a user and a service provider. Instead of each application verifying the user directly, a **trusted third-party** (identity provider) does the job.

- **Encrypted access tokens** are exchanged between the **identity provider** and the **service provider**.
- This process uses protocols like:
  - **LDAP (Lightweight Directory Access Protocol)**: Used on-premises
  - **SAML (Security Assertion Markup Language)**: Used off-premises (e.g., cloud environments)

> Note: LDAP and SAML are often used together.

**Example**: One access token can connect a user to multiple applications.

---

## Limitations of SSO

While SSO offers many benefits, it still relies on **usernames and passwords**—which are not always secure.

- If an SSO password is stolen, **multiple services** could be exposed.

---

## MFA to the Rescue

**Multi-Factor Authentication (MFA)** requires users to **verify their identity in two or more ways**.

Think of it like using an **ATM**:

1. Insert your debit card (something you have)
2. Enter your PIN (something you know)

Only then can you access your account.

---

## Strengthening Authentication

MFA strengthens security by requiring:

- **2FA** (Two-Factor Authentication)
- **3FA** (Three-Factor Authentication)

### The Three Factors:

1. 🔐 **Something you know** – e.g., username and password
2. 📱 **Something you have** – e.g., one-time passcode (OTP) sent via SMS
3. 🧬 **Something you are** – e.g., fingerprints, facial recognition

MFA is especially useful in **cloud environments** where it’s difficult to verify remote users. It adds a layer of protection that is **hard to imitate** or **brute force**.

---

## Key Takeaways

- **Passwords alone are not secure enough**
- **SSO** simplifies access by reducing login points
- **MFA** adds additional verification to ensure identity
- **Together**, SSO + MFA provide a strong, user-friendly security solution

## By combining SSO and MFA, organizations can ensure that access is both **secure** and **convenient**.

# Managing User Access for Digital Asset Security

This document summarizes key concepts related to managing user access for digital asset security.

## Key Security Principles

- **Principle of Least Privilege:** Grant users the minimum level of access necessary to perform their job duties.
- **Separation of Duties:** Divide responsibilities among multiple users to prevent any single individual from having excessive control or the ability to misuse the system.

## Identity and Access Management (IAM)

- **Definition:** IAM encompasses processes and technologies that help organizations manage digital identities within their environment.
- **Goal:** Ensure the right user is granted access to the right resources at the right time and for the right reasons.
- **Key Components:**
  - **Authentication:** Verifying user identities (e.g., using passwords, multi-factor authentication).
  - **Authorization:** Determining what resources a user is allowed to access.
  - **User Provisioning:** Creating, managing, and deactivating user accounts and their associated access privileges.

## Authorization Frameworks

- **Mandatory Access Control (MAC):** Strictest framework where access is granted based on a need-to-know basis, typically by a central authority.
- **Discretionary Access Control (DAC):** Data owners have the discretion to determine and grant access levels to others.
- **Role-Based Access Control (RBAC):** Access is granted based on a user's role within the organization, simplifying access management for large groups.

## Access Control Technologies

- Organizations often use a combination of access control technologies to enforce authentication, authorization, and auditing.
- These technologies can be custom-built or third-party solutions.

## Key Takeaways

- Controlling access to digital assets is crucial for maintaining security.
- IAM and AAA (Authentication, Authorization, and Accounting) are common frameworks for implementing least privilege and separation of duties.
- Security analysts play a vital role in user provisioning and collaborating with IAM teams.
