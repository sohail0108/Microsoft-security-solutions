# Introduction

To allow employees, partners, and customers to collaborate securely, organizations need to shift to an approach whereby identity becomes the new security perimeter.

Using an identity provider helps organizations manage that shift and all the aspects of identity security.

**What is Microsoft Entra ID?**

It is a cloud-based identity & access management (IAM) service
Helps organizations:

1. Manage user logins

2. Control who can access what

3. Secure apps, data, and resources

**Types of Identities**

Microsoft Entra ID supports:

1. User identities → Employees, students, admins

2. External identities → Partners, customers (B2B/B2C)

3. Application identities → Apps/services accessing resources

4. Managed identities → Secure identity for Azure services (no passwords)


**Final Understanding**

Security is no longer about networks, It’s about who is accessing (identity)

**Microsoft Entra ID helps:**
1. Authenticate users
2. Authorize access
3. Secure collaboration (internal + external)

---

# Describe Microsoft Entra ID

Microsoft Entra ID, formerly Azure Active Directory, is Microsoft’s cloud-based identity and access management service. 
Organizations use Microsoft Entra ID to enable their employees, guests, and others to sign in and access the resources they need, including:

1. Internal resources, such as apps on your corporate network and intranet, and cloud apps developed by your own organization.
2. External services, such as Microsoft Office 365, the Azure portal, and any SaaS applications used by your organization.


Instead of managing logins in many places, everything is managed in one place (Entra ID),Users can use one account to access all systems
Works with:
1. Cloud
2. On-premises
3. External users

<img width="2146" height="1463" alt="image" src="https://github.com/user-attachments/assets/fe3e00be-103d-4da1-9f13-131e0b435c76" />

What this diagram shows
Microsoft Entra ID is the central system (brain) for identity and access.
It connects everything:

📱 Devices (laptops, mobiles)

☁️ Cloud apps (like Office 365 / Azure)

🏢 On-premises apps & Active Directory

🤝 Business partners & customers

#  Identity Secure Score

🛡️ Identity Secure Score (Very Important)

Microsoft Entra ID gives an Identity Secure Score

🔢 What is it?

A percentage (%) score

Shows how secure your organization’s identity setup is

Based on Microsoft security best practices

👉 Example:

Your score = 16%

Typical company = 53%

➡️ Means your security needs improvement

**🧠 Why it is useful?**

📊 Measure security level

🛠️ Get improvement suggestions




<img width="1013" height="801" alt="image" src="https://github.com/user-attachments/assets/11aca8d5-c060-4cbb-ae47-101709486a70" />


**⚙️ How it works**

It gives Improvement Actions, like:

Use least privilege access

Enable risk policies

Add more global admins

**Each action shows:**

⭐ Score impact

👤 User impact

💰 Implementation cost

📈 Track progress over time

# Basic Terminology (Simple Understanding)

1️⃣ **Tenant (Most Important Concept)**

👉 **Tenant** = Your Organization in Entra ID

A separate instance of Entra ID for your company Contains:

1. Users 👤

2. Groups 👥

3. Devices 💻

4. Apps 📱

5. Policies 🔐

Has:

Unique Tenant ID & Domain name (e.g., contoso.onmicrosoft.com)

✅ Think:
👉 Tenant = Full company environment + security boundary

#

**2️⃣ Directory**

👉 **Directory** = Data inside the tenant

Stores all identity info:

1. Users

2. Apps

3. Devices

Like a database/catalog

✅ **Important:** 1 Tenant = 1 Directory

#

**3️⃣ Multi-Tenant**

👉 Multi-tenant = Multiple Entra tenants

Used when:

1. Company has multiple branches/subsidiaries
2. Mergers & acquisitions
3. Different countries (compliance rules)

✅ Think:

1 tenant → single company
Multi-tenant → multiple company environments

# 👥 Who uses Microsoft Entra ID?

🛠️**1. IT Administrators**

**They use it to:**

1. 🔐 Control who can access what
2. 🔑 Enable MFA (Multi-Factor Authentication)
3. 📊 Manage users, roles, and policies
4. 🛡️ Protect identities & credentials
5. 📋 Handle access governance (rules, permissions)
   
**✅ Example:**

**Admin sets rule** → “Office login ke liye OTP mandatory”

# 

**💻 2. Developers**

👉 App banane wale log

**They use it to:**

1. 🔑 Add SSO (Single Sign-On) in apps
2. 👤 Let users login with existing accounts
3. 🔗 Use APIs to access organization data

**✅ Example:**
Ek app banayi → user directly company account se login kar sakta hai

#

**🧑‍💼 3. End Users (Indirectly)**

👉 Employees / users

**They benefit from:**

1. 🔓 Single login (SSO)
2. 📱 Secure access from anywhere
3. 🔐 Extra security (MFA)

#

**☁️ 4. Service Subscribers**

**Users of:**

1. Microsoft Azure
2. Microsoft 365
3. Dynamics 365

👉 Automatically get access to Entra ID

**✅ They can:**

Use basic features
Upgrade to Premium for advanced security

#
**⚡ One-Line Summary**

👉 Admins manage security, developers integrate login, users access apps, and cloud subscribers automatically use Entra ID.

---

# Microsoft Entra ID - Identity Types

## 🔐 Introduction
Microsoft Entra ID supports different types of identities.  
Main question: **"Kisko identity assign kar sakte ho?"**

👉 Answer: 3 main categories

---

<img width="637" height="226" alt="image" src="https://github.com/user-attachments/assets/ac9df7f4-42d6-47e5-b2f5-d87386b9f605" />


## 👤 1. User Identities (Humans)
These are identities assigned to people.

### Examples:
- Employees (internal users)
- Customers
- Partners
- Vendors
- Consultants

### Use:
- Login to applications
- Access organizational resources

---

## 💻 2. Device Identities
These are identities assigned to physical devices.

### Examples:
- Mobile phones
- Laptops / Desktops
- IoT devices

### Use:
- Ensure only trusted devices can access resources
- Apply device-based security policies

---

## ⚙️ 3. Workload Identities (Software)
These are identities assigned to software-based objects.

### Examples:
- Applications
- Virtual Machines (VMs)
- Services
- Containers

### Use:
- Secure communication between services
- Avoid hardcoded credentials (passwords)

---

## 🌐 Other Important Identity Types

### External Identities
- Users outside the organization
- Examples: partners, customers
- Used for secure collaboration

---

### 🔗 Hybrid Identities
- Combination of:
  - On-premises Active Directory
  - Cloud (Entra ID)

### Benefit:
- Same login for both environments

---

## ⚡ Final Summary of Identity Types
Microsoft Entra ID assigns identities to:
- 👤 Humans (Users)
- 💻 Devices
- ⚙️ Software (Workloads)

👉 Purpose: Secure and controlled access to resources


# Microsoft Entra ID - User & Workload Identities

---

## 👤 User Identities

User identities represent **people**:
- Employees
- Customers
- Partners
- Vendors
- Consultants

---

## 🔐 Two Key Concepts

### 1. How User Authenticates

#### Internal Authentication
- User has account in **your organization’s Entra ID**
- Uses same account to login

#### External Authentication
- User logs in using:
  - Another organization’s Entra ID
  - Social account (Google, Facebook, etc.)
  - Other identity providers

---

### 2. UserType Property

Defines **relationship with organization**

- **Member** → Full access (employees)
- **Guest** → Limited access (external users)

---

## 👥 User Types Explained

### 🏢 Internal Member
- Employees of organization
- Login: Internal Entra ID
- Access: Full (Member-level)

---

### 🌐 External Guest
- Partners, vendors, consultants
- Login: External account
- Access: Limited (Guest-level)

---

### 🔄 External Member
- Used in **multi-tenant organizations**

#### Example:
- Contoso user accessing Fabrikam resources
- Login: External (Contoso account)
- Access: Member-level in Fabrikam

---

### ⚠️ Internal Guest (Legacy)
- Internal account but limited access
- Used earlier before B2B
- Now mostly replaced by **B2B collaboration**

---

## 🤝 B2B Collaboration
- External users use **their own credentials**
- Organization doesn’t manage their passwords
- Falls under **External Identities**

---

## ⚙️ Workload Identities

### 📌 What is it?
Identity for **software (not humans)**

Used by:
- Applications
- Services
- Virtual Machines
- Containers

---

### 🎯 Purpose
- Authenticate apps securely
- Access resources without human login

---

## ⚠️ Security Challenges
- Credentials need secure storage
- Hard to track:
  - When created
  - When to revoke
- Risk of:
  - Data breach
  - Unauthorized access

---

## 🛡️ Solution: Microsoft Entra Workload ID
Helps secure and manage workload identities

---

## 🔧 Types of Workload Identities

### 1. Applications
- App registered in Entra ID
- Enables integration

---

### 2. Service Principals
- Identity of an application in a tenant

#### Key Points:
- Created after app registration
- Used for:
  - Authentication
  - Authorization

---

### 3. Managed Identities
- No need to manage credentials manually
- Azure handles:
  - Passwords
  - Secrets

✅ More secure than service principals

---

## ⚡ Final Summary of User & Workload Identities

### User Identities:
- 👤 Internal Member → Employee (full access)
- 🌐 External Guest → Limited access
- 🔄 External Member → External login + full access
- ⚠️ Internal Guest → Legacy

### Workload Identities:
- ⚙️ Apps, Services, VMs
- 🔐 Used for secure app-to-app communication
- 🛡️ Managed Identities = safest option

---
# Microsoft Entra ID - Managed Identities, Devices & Groups

---

## 🔐 Managed Identities

### 📌 What is it?
- Special type of **service principal**
- Automatically managed by Microsoft Entra ID
- No need to store/manage credentials (passwords, secrets)

### 🎯 Benefits:
- 🔒 More secure (no hardcoded credentials)
- ⚙️ Easy to use with Azure services
- 💰 No extra cost
---

## 🔄 Types of Managed Identities

### 1️⃣ System-Assigned Managed Identity

#### 🔹 Key Points:
- Created **automatically** when enabled on a resource
- Tied to **one Azure resource**
- Lifecycle depends on resource

#### ⚡ Behavior:
- Resource deleted → Identity also deleted

#### ✅ Example:
- App running on a **single Virtual Machine (VM)**

---
### 2️⃣ User-Assigned Managed Identity

#### 🔹 Key Points:
- Created as a **separate Azure resource**
- Can be assigned to **multiple resources**

#### ⚡ Behavior:
- Resource deleted → Identity remains
- Must be deleted **manually**

#### ✅ Example:
- Same identity used across **multiple VMs**

---

## ⚖️ Quick Difference

| Feature | System-Assigned | User-Assigned |
|--------|---------------|--------------|
| Lifecycle | Tied to resource | Independent |
| Reusability | ❌ No | ✅ Yes |
| Deletion | Auto | Manual |

---

## 💻 Device Identities

### 📌 What is a Device?
- Hardware like:
  - Mobile 📱
  - Laptop 💻
  - Server 🖥️
  - Printer 🖨️

### 🎯 Purpose:
- Help admins control:
  - Access
  - Configuration
  - Security policies

---

## 🔄 Types of Device Identities

### 1️⃣ Microsoft Entra Registered
- For **personal devices (BYOD)**
- No need for org account login on device

#### ✅ Use Case:
- Employee using **personal mobile**

---

### 2️⃣ Microsoft Entra Joined
- Device is **owned by organization**
- Login using **org account**

#### ✅ Use Case:
- Company laptop

---
### 3️⃣ Microsoft Entra Hybrid Joined
- Connected to:
  - On-prem Active Directory
  - Entra ID

#### ✅ Use Case:
- Organizations using **both on-prem + cloud**

---

## 🔑 Key Benefit of Devices
- ✅ Single Sign-On (SSO)
- ✅ Secure access to cloud + on-prem apps

---
## 📱 Device Management

### 🛠️ Tool: Microsoft Intune
- Cloud-based service
- Handles:
  - MDM (Mobile Device Management)
  - MAM (Mobile Application Management)

---
## 👥 Groups in Microsoft Entra ID

### 📌 What is a Group?
- Collection of identities (users/devices)
- Used to assign permissions **in bulk**

### 🎯 Benefit:
- No need to assign access individually
- Follows **Zero Trust principle** (least access)

---
## 🔄 Types of Groups

### 1️⃣ Security Groups

#### 🔹 Purpose:
- Manage access to resources

#### 👥 Members:
- Users (internal + external)
- Devices
- Other groups
- Service principals

#### ✅ Example:
- Enforce MFA using Conditional Access

#### ⚠️ Requirement:
- Admin role needed to create

---
### 2️⃣ Microsoft 365 Groups

#### 🔹 Purpose:
- Collaboration

#### 👥 Members:
- Only users (including external)

#### ✅ Features:
- Shared mailbox 📧
- Calendar 📅
- SharePoint files 📂

#### ⚡ Note:
- Users can create (no admin needed)

---
## 🔄 Group Membership Types

### 1️⃣ Assigned (Manual)
- Admin manually adds/removes users

---

### 2️⃣ Dynamic Membership
- Rules-based automatic membership

#### ✅ Example Rule:
- Department = "IT" → auto added to group

---
## ⚡ Final Summary

### Managed Identities:
- 🔐 Auto-managed identities for apps
- 2 types:
  - System-assigned (tied to resource)
  - User-assigned (reusable)

---

### Devices:
- 💻 Registered → Personal
- 🏢 Joined → Organization
- 🔄 Hybrid → On-prem + Cloud

---

### Groups:
- 👥 Security → Access control
- 🤝 Microsoft 365 → Collaboration
- ⚙️ Dynamic → Auto membership

---
# Microsoft Entra Agent ID (AI Agent Identities)

---

## 🤖 What is Microsoft Entra Agent ID?

Microsoft Entra Agent ID is a **security and identity framework** designed for **AI agents**.

👉 Just like:
- 👤 Users need identity
- ⚙️ Apps need identity  

➡️ Same way, **AI agents also need identity** to:
- Authenticate
- Access resources securely

---

## ❓ Why AI Agents Need Separate Identity?

AI agents are different from normal apps:

- 🧠 Make **dynamic decisions**
- 🔄 Adapt based on context
- 🤖 Work **autonomously**

---

## ⚠️ Security Challenges with AI Agents

### 1️⃣ Expanded Attack Surface
- Interact with external systems
- Vulnerable to:
  - Prompt injection attacks
  - External threats

---

### 2️⃣ Permission Risks
- Often given **broad permissions**
- May:
  - Access unnecessary data
  - Perform unintended actions

---

### 3️⃣ Agent Sprawl
- Too many agents created
- Problems:
  - No visibility
  - No lifecycle control
  - Old agents remain active

---

## 🎯 Goal
👉 Treat AI agents **separately** from:
- User identities
- Workload identities

➡️ Apply proper **security & governance**

---

## ⚙️ How Microsoft Entra Agent ID Works

Built on top of:
- Microsoft Entra ID platform

---

## 🔑 Key Concepts

### 1️⃣ Agent Identity Blueprints

#### 📌 What is it?
- Template for creating agents

#### 🔹 Contains:
- Agent type/classification
- Credentials (used indirectly)
- Policies

#### ✅ Example:
- "Sales Assistant Agent"
  - Defines permissions for all sales agents

---

### 2️⃣ Agent Identities

#### 📌 What is it?
- Individual AI agent instance

#### 🔹 Features:
- Unique ID
- Display name
- Sponsor (human/group responsible)

#### ⚠️ Important:
- No direct credentials
- Uses **blueprint** for authentication

---

## 🔄 Blueprint → Identity Model

- Blueprint = Template 🧩  
- Agent Identity = Instance 🤖  

👉 Benefits:
- Centralized control
- Easy management at scale

---

## 🛡️ Security & Management Benefits

Admins can:
- 🔐 Apply Conditional Access policies
- 🚫 Disable permissions
- 📊 Audit agents
- ⚙️ Manage multiple agents easily

---

## ⚡ Final Summary

- 🤖 AI agents need **separate identity system**
- 🔐 Microsoft Entra Agent ID provides secure framework
- 🧩 Blueprints = Templates
- 🤖 Agent Identities = Instances
- 🛡️ Enables centralized control & security

---

# Microsoft Entra ID - External Identities

---

## 🌐 What are External Identities?

External identities allow **people outside your organization** to access:
- Applications
- Resources
- Data

👉 Used for collaboration with:
- Partners 🤝
- Customers 🧑‍💼
- Business clients 🏢

---

## 🔐 Microsoft Entra External ID

Microsoft Entra External ID is a solution that helps:
- Securely manage **external users**
- Allow users to **bring their own identity**

---

<img width="1120" height="531" alt="image" src="https://github.com/user-attachments/assets/2a57ca32-628e-45c8-b21e-02ce67b3b22c" />

## 👤 Types of External Identities

Users can sign in using:

- 🏢 Corporate accounts (other organizations)
- 🏛️ Government-issued accounts
- 🌐 Social accounts:
  - Google
  - Facebook

---


## 🎯 Key Use Cases

### 1️⃣ Collaborate with Business Guests
- Partners, vendors, consultants
- Secure access to internal resources

---

### 2️⃣ Apps for Consumers & Customers
- Public apps (web/mobile)
- Used by:
  - Customers
  - Business clients

---

## 🏢 Tenant Configuration Types

Microsoft Entra supports **2 configurations**

---

### 1️⃣ Workforce Tenant

#### 📌 Used for:
- Employees
- Internal apps
- Organizational resources

#### 🔹 Feature:
- Can invite **external users (guests)**

---

### 2️⃣ External Tenant

#### 📌 Used for:
- External users only
- Consumers / customers

#### 🔹 Feature:
- Apps published for public or business users

<img width="1018" height="641" alt="image" src="https://github.com/user-attachments/assets/23d46a81-424c-4c93-b947-35c2440a260d" />

---

## ⚡ Quick Difference

| Feature | Workforce Tenant | External Tenant |
|--------|----------------|----------------|
| Users | Employees + Guests | Only external users |
| Purpose | Internal work | Customer-facing apps |
| Access | Internal resources | Public/business apps |

---

## ⚡ Final Summary

- 🌐 External Identities = Outside users
- 🔐 Entra External ID secures access
- 👤 Users can bring their own accounts
- 🏢 Workforce tenant → Internal + guests
- 🌍 External tenant → Only external users

---


# Microsoft Entra ID - B2B, CIAM & Direct Connect

---

## 🤝 B2B Collaboration (Business Guests)

<img width="659" height="521" alt="image" src="https://github.com/user-attachments/assets/ea8e1c25-6699-49cf-b676-a426b2463d2f" />


### 📌 What is it?
- Allows employees to **collaborate with external partners**
- Uses **External ID for B2B collaboration**

---

### 🔐 How it works:
- External users (guests):
  - Use **their own credentials**
  - No need to create new passwords

- Your organization:
  - Controls access to apps & data
  - Verifies user eligibility

---

### 🎯 Use Cases:
- Office 365 apps 📧
- SaaS applications ☁️
- Internal business apps 🏢

---

### ⚡ Key Point:
- Guests are added as **Guest users in your tenant**

---

## 🌐 CIAM (Customer Identity & Access Management)

### 📌 What is it?
- Used for **customers & business users**
- Helps secure **public/consumer applications**
  
<img width="654" height="521" alt="image" src="https://github.com/user-attachments/assets/9ac480cc-5537-4ecf-9d47-4e83b6c8024c" />

---

### 🔹 Features:
- 📝 Self-service registration (signup/login)
- 🔑 Single Sign-On (SSO)
- 🌍 Login using:
  - Social accounts (Google, Facebook)
  - Enterprise accounts

- 👤 Customer account management

---

### 🎯 Benefits:
- 🔐 Strong security
- 📊 Scalable
- 📋 Compliance ready

---

## 🔗 B2B Direct Connect

### 📌 What is it?
- Direct connection between **two Entra organizations**

---

### 🔹 Key Features:
- No guest accounts created ❌
- Users stay in **their home tenant**
- Access shared resources directly

---

### 🎯 Example:
- Microsoft Teams shared channels:
  - Chat 💬
  - Calls 📞
  - File sharing 📂

---

## ⚖️ B2B vs Direct Connect

| Feature | B2B Collaboration | B2B Direct Connect |
|--------|------------------|-------------------|
| User Type | Guest user | No guest |
| Identity | Stored in your tenant | Stays in home tenant |
| Use Case | App/resource access | Teams collaboration |

---

## ⚡ Final Summary

- 🤝 B2B → External users as guests (access apps)
- 🌐 CIAM → Customers use apps (login/signup)
- 🔗 Direct Connect → Org-to-org direct access (no guest)

---
# 🔐 Authentication Methods (Microsoft Entra ID)

<img width="1639" height="768" alt="image" src="https://github.com/user-attachments/assets/d71be8fa-ec92-4e1f-bfc9-fa68b582fdb1" />


## 1. Password-based Authentication
- Most common method (username + password)  
- ❌ Weak when used alone (phishing, brute-force attacks)  
- ✅ Should be combined with MFA or passwordless methods  

---

## 2. Phone-based Authentication
- **SMS OTP** → Code sent via text (primary/secondary)  
- **Voice Call** → User confirms via call (secondary only)  
- ⚠️ Less secure (SIM swap, phishing risks)  

---

## 3. OATH Tokens (TOTP)
- Generates time-based one-time passwords  
- Types:
  - **Software tokens** → Apps (Microsoft Authenticator)  
  - **Hardware tokens** → Physical devices (key fob)  
- Used as MFA / secondary authentication  

---

## 4. Other Authentication Methods
- **Temporary Access Pass (TAP)** → Temporary login for onboarding/recovery  
- **QR Code Authentication** → Fast login for shared/frontline devices  
- **Email OTP** → Used in SSPR and guest access  
- **Authenticator Lite** → MFA inside apps (e.g., Outlook mobile)  
- **External MFA Providers** → Duo, RSA integration  
- **Platform Credential (macOS)** → Secure device-based authentication  

---

## 5. Passwordless Authentication (Most Important)

### a) Windows Hello for Business
- Uses **PIN + biometrics + device key**
- Provides strong protection against credential theft  

### b) Passkeys (FIDO2)
- Uses **public-private key cryptography**
- Types:
  - **Device-bound** (stored on a single device)
  - **Synced** (across devices via cloud providers)
- ✅ Phishing-resistant  

### c) Microsoft Authenticator
- Supports:
  - Passwordless login  
  - Push notifications (MFA)  
  - OTP codes  
- Uses number matching for enhanced security
  
<img width="590" height="381" alt="image" src="https://github.com/user-attachments/assets/c4c22dd9-99d2-4904-ab7a-7e150f97fea4" />

---

# 🔐 Certificate-Based & Phishing-Resistant Authentication (Easy Notes)

## 📜 Certificate-Based Authentication (CBA)

- Uses **X.509 certificates** to verify user identity  
- Users sign in **without passwords**  
- Works directly with **Microsoft Entra ID (cloud-based)**  
- ❌ No need for AD FS (no extra infrastructure)  

### ✅ Key Points
- Passwordless authentication  
- Can be used as:
  - **Primary authentication**
  - **MFA (secondary authentication)**  
- More secure than passwords  

---

## 🎣 Phishing-Resistant Authentication

### ❗ Problem
- SMS OTP & Email OTP can be **phished (stolen)**  
- Attackers use **AI + social engineering**  

### ✅ Solution
Use **phishing-resistant methods**

### 🔐 How it works
- Uses **public-private key cryptography**  
- Credential is linked to a **specific website/domain**  
- ✔️ Works only on original site  
- ❌ Cannot be reused or stolen  

---

## 🚀 Phishing-Resistant Methods (IMPORTANT)

- **Windows Hello for Business**  
- **Platform Credential (macOS)**  
- **Passkeys (FIDO2)**  
- **Microsoft Authenticator (Passkeys)**  
- **Certificate-Based Authentication (CBA)**  

---

## 🔑 Primary vs Secondary Authentication

### 🟢 Primary Authentication
- First step during login  
- Examples:
  - Password  
  - Passkeys  
  - CBA  

---

### 🟡 Secondary Authentication (MFA)
- Second layer of security  
- Used after primary login  
- Examples:
  - OTP (SMS/Email)  
  - Authenticator app  
  - OATH tokens  

---

# 🔥 Key Points (Exam & Interview)

- **Best Security:** Passkeys (FIDO2), Windows Hello  
- **Weak Methods:** Passwords, SMS OTP  
- **MFA is essential**  
- **Phishing-resistant methods:** Passkeys, Authenticator  
- **TAP:** Used for onboarding and recovery  

---

# 🛡️ SOC Analyst Perspective

- Monitor for:
  - Multiple failed login attempts (brute force)  
  - MFA fatigue attacks (push spam)  
  - Suspicious OTP activity  

- Enforce:
  - MFA policies  
  - Passwordless authentication  
  - Conditional Access policies
 
---
