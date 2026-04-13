# 🔐 Azure Entra ID – Risk-Based Conditional Access (MFA Enforcement)

## 📌 Overview
This project demonstrates the implementation of **risk-based Conditional Access policies** in Microsoft Entra ID to enhance identity security. The solution enforces **Multi-Factor Authentication (MFA)** when elevated risk is detected during user sign-ins.

---

## 🎯 Objectives
- Implement risk-based access control using Microsoft Entra ID  
- Enforce MFA for medium and high-risk sign-in scenarios  
- Strengthen identity protection using built-in risk detections  

---

## 🏗️ Environment
- Microsoft Entra ID  
- Conditional Access Policies  
- Identity Protection (Risk-Based Policies)  

---

## ⚙️ Step-by-Step Implementation

### Step 1 – Navigate to Conditional Access
- Go to **Microsoft Entra Admin Center**
- Select: **Identity Protection**
- Click: **Risk-based Conditional Access**

---

### Step 2 – Create New Policy
- Click: **New Policy**
- Name: `Medium or High require MFA Entra ID`

---

### Step 3 – Assign Users
- Select: **Users or workload identities**
- Choose: **All Users**

> ⚠️ In production, this should be tested with a pilot group first.

---

### Step 4 – Configure User Risk
- Select: **User Risk**
- Set to: Configure → Yes
- Include:
  - Medium
  - High

---

### Step 5 – Configure Sign-In Risk
- Select: **Sign-In Risk**
- Set to: Configure → Yes
- Include:
  - Medium
  - High

---

### Step 6 – Configure Access Controls
- Select: **Grant**
- Choose:
  - Require Multi-Factor Authentication (MFA)

---

### Step 7 – Enable Policy
- Set to: **Report-only** (testing phase)
- Then switch to: **On**

---

### Step 8 – Create Policy
- Click: **Create**
- Confirm policy appears in Conditional Access list

---

## ✅ Validation
- Verified policy is active  
- Confirmed MFA triggers on risky sign-ins  
- Ensured policy applies correctly to users  

---

## 🔐 Security Impact
- Protects against compromised credentials  
- Enforces MFA dynamically based on risk  
- Supports Zero Trust security model  

---

## 🧠 Key Takeaways
- Risk-based policies strengthen identity security  
- MFA is critical for protecting user accounts  
- Identity Protection enables real-time access decisions  

---

## 🚀 Future Improvements
- Block legacy authentication  
- Add location-based policies  
- Implement Privileged Identity Management (PIM)  

---

## 📸 Screenshots
Place all screenshots in the **/screenshots** folder.

---

## 👩‍💻 Author
Josephine Lopez  
AZ-900 Certified | Studying SC-900  
