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

# 🔐 Multifactor Authentication (MFA) – Complete Revision Notes

## 📌 What is MFA?

- MFA = **Multiple layers of authentication during login**
- Instead of only password → user must provide **2 or more factors**

### ❗ Why MFA?
- Passwords can be:
  - Weak
  - Reused
  - Stolen (phishing, leaks)
- ✅ MFA adds **extra security layer**
- Makes it **hard for attackers to access accounts**

---

## 🔑 Authentication Factors (Core Concept)

Microsoft Entra MFA uses:

1. **Something you know**
   - Password / PIN  

2. **Something you have**
   - Phone  
   - Hardware key  
   - Authenticator app  

3. **Something you are**
   - Fingerprint  
   - Face recognition  

---

## ⚙️ How Microsoft Entra MFA Works

- MFA is triggered during **sign-in event**
- Microsoft Entra ID:
  - Automatically requests MFA
  - No app/service changes required  

### 🔄 Login Flow
1. User enters credentials  
2. MFA prompt appears  
3. User verifies identity using registered method  

---

### 👤 User Control
- Users can:
  - Add/edit methods via **MyAccount portal**
- Admin can:
  - Enforce specific MFA methods  

---

## 🔐 Available MFA Verification Methods

<img width="1075" height="787" alt="image" src="https://github.com/user-attachments/assets/34cb52bd-d633-4741-81f7-c1a8794d4063" />

### 📱 App-Based Methods
- Microsoft Authenticator  
- Authenticator Lite (Outlook)  

---

### 💻 Device-Based Methods
- Windows Hello for Business  
- Passkey (FIDO2)  
- Passkey in Microsoft Authenticator  

---

### 🪪 Certificate-Based
- Certificate-Based Authentication (CBA)  
  - Works as MFA when configured  

---

### 🔗 External Methods
- External authentication providers  

---

### ⏳ Temporary Access
- Temporary Access Pass (TAP)  

---

### 🔢 Token-Based Methods
- OATH Hardware Token  
- OATH Software Token  

---

### 📞 Traditional Methods (Less Secure)
- SMS (OTP)  
- Voice Call  

---

## 🛡️ Security Defaults (VERY IMPORTANT)

### 📌 What are Security Defaults?
- Pre-configured **basic security settings**
- Enabled by default in new tenants  
- Free security baseline  

---

### 🔥 Key Features
- Require MFA registration for all users  
- Require MFA for admins  
- Enforce MFA when needed  
- Block legacy authentication  
- Protect privileged operations (Azure portal)  

---

### 📊 Important Fact
- ✅ **99.9% of identity attacks stopped using MFA + blocking legacy auth**

---

### 🔢 Number Matching (Anti MFA Fatigue)
- During login:
  - User sees a number  
  - Must enter same number in Authenticator app  
- ✅ Prevents:
  - MFA fatigue attacks  
  - Random approval attacks  

---

## ⚡ Conditional Access + MFA

### 📌 What is Conditional Access?
- Advanced policy-based control  
- Requires **Entra ID P1/P2 license**  

---

### 🎯 Purpose
- Apply MFA based on conditions:
  - Location  
  - Device  
  - Risk level  
  - Application sensitivity  

---

### 📍 Real Example

- ✅ Inside office network:
  - Only password required  

- ❗ Outside network:
  - MFA required  

---

## 🧠 Quick Revision Points

- MFA = **2 or more factors**
- Types:
  - Know (password)
  - Have (device)
  - Are (biometric)

---

### ✅ Most Secure Methods
- Passkeys (FIDO2)  
- Windows Hello  
- Authenticator app  

---

### ❌ Less Secure
- SMS OTP  
- Voice call  

---

### 🔥 Important Concepts
- MFA stops **credential theft attacks**
- Security defaults = **basic protection**
- Conditional Access = **advanced control**
- Number matching = **anti MFA fatigue**

---

## 🧑‍💻 SOC Analyst Perspective

- Enforce MFA for all users  
- Prefer phishing-resistant methods  
- Monitor:
  - MFA bypass attempts  
  - Unusual login activity  
- Block legacy authentication  

---

## 🚀 Final Real-Life Flow

1. User enters username + password  
2. Gets MFA prompt  
3. Approves via Authenticator / OTP  

👉 Access granted securely  

---
# 🔐 Self-Service Password Reset (SSPR) – Full Detailed Notes

## 📌 What is SSPR?

- SSPR = Users can **reset/change password without admin/helpdesk**
- Works when:
  - User forgets password  
  - Account is locked  

### 🎯 Benefits
- Reduces helpdesk calls  
- Improves productivity  
- Faster account recovery  

### 📊 Logging
- Provides **audit logs**
- Logs can be integrated with:
  - SIEM systems  

---

## ⚙️ How SSPR Works

When user opens SSPR portal, Microsoft Entra performs checks:

1. ✅ User account is valid  
2. ✅ SSPR is enabled  
3. ✅ User has registered authentication methods  
4. ✅ Password location is identified (cloud/on-prem)  

👉 If all pass → user can reset/change password  

---

## 👤 Requirements to Use SSPR

User must:

- Have **Microsoft Entra ID license**
- Be **enabled for SSPR by admin**
- Be **registered with authentication methods**

📌 Recommendation:
- Use **2 or more authentication methods** (backup safety)

---

## 🔐 Authentication Methods for SSPR

Users must register at least **1 method (2 recommended)**

### 📱 Supported Methods
- Microsoft Authenticator (push notification)  
- Software OATH tokens  
- Hardware OATH tokens (preview)  
- SMS (OTP)  
- Voice call  
- Email OTP  
- Security questions ⚠️  

---

### ⚠️ Important Update
- ❌ Security Questions will be **retired in March 2027**
- ✅ Organizations must switch to other methods  

---

## ⚙️ Admin Configuration

Admins can:

- Choose **required methods (1 or 2)**
- Control authentication options  
- Enable/disable SSPR  

---

### 🔑 Special Case (Admins)

- Admin accounts:
  - Always enabled for SSPR  
  - Require **2 authentication methods**  
  - ❌ Cannot use security questions  

---

## 🔄 Registration & Reconfirmation

### 📌 Registration
- Users must register methods before using SSPR  
- Prompt shown during login if not registered  

---

### 🔁 Reconfirmation
- Admin can force users to re-verify info  
- Time range: **0–730 days**

👉 Ensures methods stay updated  

---

## 🔔 Notifications

### 📧 User Notifications
- Email sent when password is reset  
- Sent to:
  - Primary email  
  - Alternate email  

---

### 👨‍💼 Admin Notifications
- Global admins get alert when:
  - Another admin resets password  

👉 Adds security for privileged accounts  

---

## 🔄 On-Prem Integration (Password Writeback)

### 📌 What is Password Writeback?

- Syncs password from:
  - Microsoft Entra ID → On-prem AD  

---

### 🔄 Supported Scenarios
- Password Hash Sync  
- Pass-through Authentication  
- Federation  

---

### 🔓 Extra Feature
- Users can:
  - Unlock account without resetting password  

---

### ⚠️ Important
- Custom password filters must support SSPR  
- Microsoft Entra password protection works by default  

---

## 🚨 Account Recovery (VERY IMPORTANT DIFFERENCE)

### 📌 Problem Scenario
- User loses ALL authentication methods  

👉 SSPR cannot help  

---

### 🔐 Solution → Account Recovery

- Uses **identity verification process**
- Powered by:
  - Microsoft Entra Verified ID  
  - Face Check (Azure AI)  

---

### 📊 SSPR vs Account Recovery

| Aspect | SSPR | Account Recovery |
|------|------|----------------|
| Use case | Forgot password | Lost all methods |
| Requirement | At least 1 method | Identity verification |
| Scope | Password reset only | Full account recovery |
| Security | Medium | High |

---

### 🔥 Key Advantage
- No human involvement → reduces social engineering risk  

---

## 🧠 Exam Important Points

- SSPR = **Self password reset without admin**
- Requires:
  - License  
  - Enablement  
  - Registration  
- Methods:
  - Authenticator, OTP, Email, etc.  
- Security questions → ❌ Removed by 2027  
- Admins:
  - Require 2 methods  
- Password writeback:
  - Sync to on-prem AD  
- Account recovery:
  - Used when **all methods lost**  

---

## 🧑‍💻 Real-Life Example

### 🏢 Scenario

1. User forgets password  
2. Opens SSPR portal  
3. Gets OTP on phone  
4. Verifies identity  
5. Sets new password  
6. Logs in  

👉 No helpdesk needed  

---

## 🛡️ SOC Analyst Perspective

- Monitor:
  - Multiple reset attempts  
  - Suspicious reset patterns  
- Ensure:
  - Strong authentication methods  
- Combine with:
  - MFA  
  - Conditional Access  

---

## ⚡ Quick Revision

- SSPR = Reset password yourself  
- Needs registered authentication methods  
- Supports password writeback  
- Security questions retiring (2027)  
- Account recovery = backup for full lockout

---
# 🔐 Password Protection & Management – Microsoft Entra ID

## 📌 What is Password Protection?

- Feature that **prevents weak passwords**
- Detects & blocks:
  - Common passwords  
  - Weak patterns  
  - Organization-specific terms  

### 🎯 Goal
- Reduce risk of:
  - Password attacks  
  - Credential compromise  

---

## ⚠️ Important Concept

- Strong passwords alone ❌ not enough  
- ✅ Must combine with:
  - MFA  
  - Conditional Access  

---

## 🌍 Global Banned Password List

### 📌 What is it?
- Default list of **weak/compromised passwords**
- Created using:
  - Real-world attack data  
  - Password spray analysis  

---

### 🔑 Key Features

- ✅ Automatically enabled  
- ❌ Cannot be disabled  
- ❌ No configuration needed  
- Applied to:
  - All users in tenant  

---

### 🧠 Smart Detection

- Uses:
  - Fuzzy matching  
  - Pattern detection  
- Blocks:
  - Millions of password variations  

---

## 🏢 Custom Banned Password List

### 📌 What is it?
- Organization-defined weak terms  

---

### 📝 Examples to Add

- Company name  
- Product names  
- Office location  
- Internal abbreviations  

---

### ⚙️ Key Points

- Max limit: **1000 terms**  
- Works with:
  - Global banned list (combined)  
- Focus:
  - Base words (system blocks variations automatically)  

---

## ⚙️ How Password Evaluation Works

When user sets/resets password:

### 1️⃣ Normalization
- Converts:
  - Uppercase → lowercase  
- Replaces:
  - @ → a  
  - $ → s  
  - 0 → o  

---

### 2️⃣ Fuzzy Matching
- Detects:
  - 1-character differences  
- Example:
  - "Password" → "Passw0rd" ❌ blocked  

---

### 3️⃣ Substring Matching
- Blocks:
  - User name  
  - Company name  

📌 Condition:
- Term must be **≥ 4 characters**

---

### 4️⃣ Score Calculation (IMPORTANT)

- +1 point → each banned term  
- +1 point → each remaining character  

👉 Password must score **≥ 5 points**

---

### 📌 Key Insight
- Long passwords ✅ allowed even if slightly weak  
- Short passwords ❌ rejected  

---

## 🚨 Password Spray Attack Protection

### 📌 What is Password Spray?

- Attacker tries:
  - Few common passwords  
  - Across many accounts  

---

### ⚠️ Why Dangerous?
- Avoids:
  - Account lockouts  
- Targets:
  - Weak passwords  

---

### 🛡️ Protection

- Global banned list blocks:
  - Most used attack passwords  
- Based on:
  - Real attack telemetry  

---

## 🔄 On-Premises Integration (Hybrid)

### 📌 Supported via Microsoft Entra Password Protection

---

### 🧩 Components

#### 1️⃣ Proxy Service
- Runs on domain-joined machine  
- Connects:
  - On-prem → Entra ID  

---

#### 2️⃣ DC Agent
- Installed on domain controllers  
- Validates:
  - Password changes  

---

### 🔄 How It Works

1. User changes password (on-prem)  
2. DC Agent checks policy  
3. Proxy connects to Entra  
4. Policy applied  
5. Password accepted/rejected  

---

### 🔑 Key Points

- Same:
  - Global + Custom lists used  
- No:
  - Direct internet access needed  
- No:
  - Schema changes required  

---

### 🔄 Policy Updates

- Policy downloaded:
  - At startup  
  - Every hour (if outdated)  

---

### ⚠️ Important

- Works as:
  - Supplement (not replacement)  
- Both must pass:
  - AD DS policy  
  - Entra policy  

---

## 🧠 Exam Important Points

- Global banned list:
  - Auto-enabled  
  - Cannot disable  
- Custom list:
  - Max 1000 terms  
- Password evaluation:
  - Normalization  
  - Fuzzy matching  
  - Substring check  
  - Score ≥ 5  
- Protects against:
  - Password spray attacks  
- Hybrid support:
  - Proxy + DC Agent  

---
# 🔐 Conditional Access – Microsoft Entra ID (Zero Trust Engine)

## 📌 What is Conditional Access?

- Conditional Access = **Policy-based access control**
- Adds **extra security layer AFTER login (first-factor authentication)**

👉 Works like:

IF condition → THEN action


### 📍 Example
- IF user logs in from outside network  
- THEN require MFA  

---

## 🎯 Purpose

- Enforce **Zero Trust security**
- Control:
  - Who can access  
  - What they access  
  - From where  
  - Under what conditions  

---

## ⚠️ Important Point

- Applied **after authentication**
- ❌ Not used for:
  - DoS attack prevention  
- ✅ Uses risk signals from attacks  

---

## 🧩 Conditional Access Policy Components

Each policy has **2 main parts**:

### 1️⃣ Assignments (WHEN policy applies)
### 2️⃣ Access Controls (WHAT action to take)

---

# 🟢 1. Assignments (Who, What, Where, When)

👉 All conditions are **ANDed (must be true)**

---

## 👤 Users

Target:
- All users  
- Specific users/groups  
- Admin roles  
- Guests  
- Workload identities (AI, apps)  

---

## 🎯 Target Resources

Applies to:
- Cloud apps (M365, Azure apps)  
- User actions (register device, security info)  
- Authentication context  
- AI services  

---

## 🌍 Network (Location-based)

Control access based on:
- IP address  
- Location  
- Trusted networks  
- Named locations  

---

## ⚙️ Conditions (Advanced Control)

### 🔐 Risk-Based
- Sign-in risk (suspicious login)  
- User risk (compromised account)  

---

### 🧠 Insider Risk
- Based on Microsoft Purview signals  

---

### 💻 Device Platform
- Windows / Android / iOS / macOS  

---

### 🌐 Client Apps
- Browser  
- Mobile apps  
- Desktop apps  

---

### 🖥️ Device Filters
- Target specific devices  
- Example:
  - Privileged access workstation  

---

# 🔵 2. Access Controls (What happens)

---

## 🚫 Block Access
- Completely deny access  

---

## ✅ Grant Access (with conditions)

Can require:

- MFA  
- Authentication strength  
- Compliant device  
- Hybrid joined device  
- Approved app  
- Password change  
- Terms of use  

---

## 🧪 Session Controls

Limit user actions after login:

- Block download/copy/print  
- Require file labeling  
- Control session time  

---

# 🔑 Authentication Strengths (VERY IMPORTANT)

Defines **how strong authentication must be**

---

## 1️⃣ Multifactor Authentication Strength
- Password + OTP / push / token  

---

## 2️⃣ Passwordless MFA Strength
- No password required  
- Methods:
  - Authenticator (phone sign-in)  
  - FIDO2  
  - Windows Hello  

---

## 3️⃣ Phishing-Resistant MFA (MOST SECURE)

- Strongest security  
- Methods:
  - FIDO2  
  - Windows Hello  
  - Certificate-based auth  

---

## 🔧 Custom Authentication Strength
- Admin defines allowed methods  

---

# 🤖 Protecting AI Services

Conditional Access can secure:

- Microsoft 365 Copilot  
- Security Copilot  

---

### 🔐 Example Policies

- Require phishing-resistant MFA  
- Allow access only from compliant device  
- Block access if insider risk is high  

---

# 💳 Licensing

- Requires:
  - Microsoft Entra ID P1 or P2  

---

### 🆓 Free Tier Alternative
- Use **Security Defaults**
  - Basic MFA enforcement  

---

# 🧠 Exam Important Points

- Conditional Access = **IF → THEN policy**
- Applied:
  - After authentication  
- Components:
  - Assignments + Access Controls  
- Assignments:
  - Who, what, where, when  
- Access controls:
  - Grant / Block / Session control  

---

## 🔥 High-Value Points

- MFA can be enforced via Conditional Access  
- Risk-based access (VERY IMPORTANT)  
- Authentication strengths define security level  
- Phishing-resistant MFA = most secure  

---

# 🧑‍💻 Real-Life Example

### 🏢 Scenario

1. User logs in from home  
2. Condition triggered:
   - Unknown location  
3. Policy applied:
   - Require MFA  

👉 Access granted after verification  

---

# 🛡️ SOC Analyst Perspective

- Monitor:
  - Risky sign-ins  
  - Policy violations  
- Enforce:
  - MFA for sensitive apps  
- Use:
  - Risk-based Conditional Access  
- Protect:
  - Admin accounts  
  - AI services  

---
