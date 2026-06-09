# Okta-Workforce-IAM-LAB
Enterprise IAM sandbox detailing user lifecycle automation, SAML 2.0 application federation, and adaptive authentication policies
# Enterprise Workforce Identity Architecture Lab
An end-to-end Identity and Access Management (IAM) deployment simulating real-world corporate lifecycle management, federated Single Sign-On (SSO), and access security controls using the **Okta Identity Engine** platform.

---

## Project Overview
This project demonstrates the design and execution of a secure corporate workforce environment. The primary objective was to move away from legacy static access models to a modern, automated, and secure identity perimeter. 

The lab successfully implements Role-Based Access Control (RBAC), federates a third-party application using enterprise industry standards, and builds a strict access intercept policy to protect sensitive corporate endpoints.

### Key IAM Domains Demonstrated:
* **Directory Operations:** User Lifecycle Management (Joiner-Mover-Leaver framework).
* **Federated Identity:** IDP-Initiated Single Sign-On (SSO) utilizing the **SAML 2.0 standard**.
* **Access Defense:** Contextual, policy-driven step-up Authentication mapping.

---

## Architecture & Implementation Phase

### Phase 1: User Lifecycle & Role-Based Access Control (RBAC)
* Created a structured corporate directory topology from scratch.
* Established a dedicated department group (`Finance-Department`) designed to isolate financial users and apply zero-standing-privilege tracking.
* Provisioned multi-user templates with day-one onboarding parameters (enforced credential resetting upon initial authentication).

### Phase 2: Federated Single Sign-On (SAML 2.0)
* Integrated an external enterprise Service Provider (RSA SAML Test platform) into the Okta Identity Engine.
* Performed a federated cryptographic handshake, parsing directory attributes securely across cloud tenants.
* Assigned applications to entire security groups simultaneously, demonstrating efficient role-based deployment.

---

## Verification & Proof of Concept

### 1. The Provisioned Workforce Perimeter
Once users are assigned to their respective organizational units, Okta’s engine automatically maps resource accessibility rules to the individual dashboards.

### 2. Successful Federation Handshake
By authenticating as a mock finance specialist (`Jane Doe`), the identity token successfully handles the assertion validation, securely transmitting the profile payload and logging the user in seamlessly without password exposure.

*(Insert successful login screenshot here)*
