# 🔐 Identity Lifecycle Automation using Microsoft Entra ID + n8n

## 📌 Overview
This project demonstrates a real-world **Identity and Access Management (IAM)** workflow that automates the complete user lifecycle:

- User provisioning (account creation)
- Role-based access assignment (RBAC)
- Group membership enforcement
- Time-based deprovisioning (auto-disable)

The system integrates **Microsoft Entra ID** with **n8n** to simulate enterprise-grade identity orchestration.

---

## 🧠 Problem Statement
In most organizations, user onboarding and offboarding are:

- Manual and time-consuming  
- Prone to human error  
- Security risks (delayed access removal)  

This project solves that by automating identity lifecycle events using APIs and workflow orchestration.

---

## 🚀 Features

- ✅ Automated user provisioning via Microsoft Graph API  
- ✅ Role-Based Access Control (RBAC) using conditional logic  
- ✅ Dynamic group assignment based on department  
- ✅ Time-based access control (auto disable after duration)  
- ✅ End-to-end identity lifecycle automation  
- ✅ API-driven architecture (no manual intervention)  

---

## 🛠️ Tech Stack

- Microsoft Entra ID (Azure AD)  
- Microsoft Graph API  
- n8n (Workflow Automation)  
- OAuth2 (Client Credentials Flow)  
- JSON / REST APIs  

---

## 🔄 Workflow Explanation

### 1. Trigger
A webhook receives user data (name, email, department)

### 2. Normalization
Incoming data is cleaned and structured

### 3. Decision Engine
Conditional logic assigns:
- IT → IT Group  
- HR → HR Group  
- Others → Default Group  

### 4. User Provisioning
User is created in Microsoft Entra ID using Graph API

### 5. Access Assignment
User is added to the appropriate group

### 6. Lifecycle Control
After a defined time:
- User account is automatically disabled

---

## 🔐 Security Concepts Implemented

- Least Privilege Access  
- Role-Based Access Control (RBAC)  
- Identity Lifecycle Management  
- Automated Deprovisioning  
- API-based Identity Governance  

---

## 📂 Project Structure


IAM-Identity-Orchestration-Entra-n8n/
│
├── README.md
├── workflow.json
├── screenshots/
└── architecture.png



---

## 💼 Use Cases

- Employee onboarding automation  
- Contractor temporary access management  
- IAM process automation  
- Security compliance workflows  
- Zero Trust identity lifecycle enforcement  

---

## 📈 Future Enhancements

- SCIM-based provisioning integration  
- Slack / Email notifications  
- Approval workflows (manager approval before access)  
- Logging & audit trail integration  
- Multi-tenant support  

---



---

## 🧠 Key Takeaway

This project demonstrates how modern IAM systems can be automated using APIs and workflow engines to improve security, efficiency, and scalability.

---

## 📬 Contact

Feel free to connect for discussions on IAM, automation, and security engineering.

