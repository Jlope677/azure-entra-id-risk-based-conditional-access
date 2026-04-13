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
![condition1](https://github.com/user-attachments/assets/7c317bfd-834a-4119-ae80-1164ecc80c71)
![condition2](https://github.com/user-attachments/assets/e2e3cdb0-4a2e-42cb-bdef-0de722b14468)


---

### Step 2 – Create New Policy
- Click: **New Policy**
- Name: `Medium or High require MFA Entra ID`
![condition3](https://github.com/user-attachments/assets/80d6b285-66d8-4d00-81a5-395042bb09a7)
![condition17](https://github.com/user-attachments/assets/9f5979fa-9958-4d05-b46e-1acf4c93823a)


---

### Step 3 – Assign Users
- Select: **Users or workload identities**
- Choose: **All Users**

> ⚠️ In production, this should be tested with a pilot group first.
![condition15](https://github.com/user-attachments/assets/1ddb52cc-c12e-48f1-b1bf-86742dd0d56a)
![condition16](https://github.com/user-attachments/assets/66734e7b-5bbb-4cd0-9ded-5d6e5cc9662a)


---

### Step 4 – Configure User Risk
- Select: **User Risk**
- Set to: Configure → Yes
- Include:
  - Medium
  - High
![condition3](https://github.com/user-attachments/assets/765192db-5546-45eb-8d44-64483037c79f)
![condition5](https://github.com/user-attachments/assets/bce7cbcf-5bdb-45c8-9c42-2dcd57eb5875)
![condition6](https://github.com/user-attachments/assets/1a905ee4-c739-4f3e-a327-b223137cad1b)
![condition7](https://github.com/user-attachments/assets/ff113431-fa56-41bb-a081-fd3c99891134)
![condition8](https://github.com/user-attachments/assets/89cf9c84-f879-43ab-b420-502db3dd42c1)
![condition9](https://github.com/user-attachments/assets/78d7b685-25cc-4833-9d1f-2d0be13021d2)

---

### Step 5 – Configure Sign-In Risk
- Select: **Sign-In Risk**
- Set to: Configure → Yes
- Include:
  - Medium
  - High
![condition10](https://github.com/user-attachments/assets/1d2e859e-0c11-4e0c-8eac-044a65a3a8f5)
![condition11](https://github.com/user-attachments/assets/dacee215-3c11-49e4-ba69-c0a91168ba75)
![condition12](https://github.com/user-attachments/assets/9227e8e3-0791-4962-be11-9b57db7d62a4)
![condition13](https://github.com/user-attachments/assets/d7696b73-cac0-4acb-ad7d-680725778cbc)
![condition14](https://github.com/user-attachments/assets/fd5bd7ee-1ff9-4d29-ac6e-f4f51a48d366)







---

### Step 6 – Configure Access Controls
- Select: **Grant**
- Choose:
  - Require Multi-Factor Authentication (MFA)
![condition18](https://github.com/user-attachments/assets/6d2332dc-9964-47ad-8538-229c4ff5f33b)
![condition19](https://github.com/user-attachments/assets/ec7c5f33-4d9f-4151-a87a-1fd0233361dc)
![condition20](https://github.com/user-attachments/assets/2a4ecf46-a4ea-45a2-9f2d-1cb2db3cf3cc)



---

### Step 7 – Enable Policy
- Set to: **Report-only** (testing phase)
- Then switch to: **On**
![condition21](https://github.com/user-attachments/assets/4b095c25-52e1-48ea-952b-757dbf31cf6f)


---

### Step 8 – Create Policy
- Click: **Create**
- Confirm policy appears in Conditional Access list
![condition22](https://github.com/user-attachments/assets/5e3b3f79-a507-4d16-af00-3b01047d5887)

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
