# 🎯 **NAAN MUDHALVAN - SALESFORCE REPORT**  
## 🚀 **A CRM Application To Manage Services Offered by an Institution**  

---

## 🌟 **Project Team**  
| **👨‍💻 Name**           | **📋 Roll Number**  |
|------------------------|--------------------|
| **Arunkumar V**       | 421622243003       |
| **Keerthi K**         | 421622243026       |
| **Yashwanth Kumar A** | 421622243057       |
| **Pugazhendhi N**     | 421622243041       |
| **Hariharan S**       | 421622243020       |

---

## 📝 **Abstract**  
The **Garage Management System (GMS)** is a modern, Salesforce-powered CRM application tailored for automotive repair businesses. It automates key processes like **appointment scheduling**, **inventory management**, **billing**, and **customer feedback**. With GMS, businesses can deliver exceptional services while gaining a competitive edge in the market.

---

## 🛠️ **Detailed Tasks**

### ✨ **Task 1: Creating Developer Account**  
1. Go to [Salesforce Developer Signup](https://developer.salesforce.com/).  
2. Complete the form:  
   - **First Name, Last Name, Email, Role:** *Developer*  
   - **Company:** *College Name*  
   - **Country:** *India*  
   - **Postal Code:** *PIN Code*  
   - **Username:** *Format `username@organization.com`*  
3. Activate your account via email verification.  

---

### 🛠️ **Task 2: Custom Objects**  
**Objects Created:**  
1. **Customer Details**  
   - *Record Name:* `Customer Name`  
   - *Type:* Text  
2. **Appointment**  
   - *Record Name:* `Appointment Name`  
   - *Auto Number:* `app-{000}`  
3. **Service Records**  
   - *Record Name:* `Service Records Name`  
   - *Auto Number:* `ser-{000}`  
4. **Billing Details & Feedback**  
   - *Record Name:* `Billing Details Name`  
   - *Auto Number:* `bill-{000}`  

---

### 🔖 **Task 3: Custom Tabs**  
Custom tabs for:  
- 🟢 **Customer Details**  
- 🟡 **Appointments**  
- 🔵 **Service Records**  
- 🔴 **Billing Details and Feedback**

---

### ⚡ **Task 4: Building Lightning App**  
Created a **Garage Management Application**:  
- **Navigation Items:** Customer Details, Appointments, Service Records, Reports, Dashboards.  
- **User Profiles:** System Administrator.  

---

### 📊 **Task 5: Custom Fields**  
| **📂 Object**                 | **📋 Field**             | **🔍 Type**      | **💡 Notes**                   |
|-------------------------------|-------------------------|-----------------|--------------------------------|
| Customer Details              | Phone Number           | Phone           | Contact details of customers. |
| Appointment                   | Vehicle Number Plate   | Text            | Required, unique (10 chars).  |
| Service Records               | Service Status         | Picklist        | Values: `Started`, `Completed`.|
| Billing Details & Feedback    | Payment Status         | Picklist        | Values: `Pending`, `Completed`.|

---

### ✅ **Task 6: Validation Rules**  
- **Appointment:**  
  - Vehicle Number Plate format: `[A-Z]{2}[0-9]{2}[A-Z]{2}[0-9]{4}`  
- **Service Records:**  
  - Service Status must equal `Completed`.  
- **Billing Feedback:**  
  - Rating must be between `1` and `5`.  

---

### 👥 **Task 7: Duplicate Rules**  
- Duplicate rules for **Customer Details** (using **Email** and **Phone Number**).  

---

### 🔒 **Task 8: Roles & Sharing**  
- **Roles:** Manager and Sales Person.  
- **Sharing:**  
  - *Service Records Object* → Private OWD, sharing rule grants Manager read/write access to Sales Person data.

---

### 📧 **Task 9: Automation**  
- Created a **Record-Triggered Flow**:  
  - Sends email alerts upon **payment completion**.  

---

### ✍️ **Task 10: Apex Trigger**  
- Trigger **AmountDistribution:** Calculates total billing amount based on selected services.

---

### 📈 **Task 11: Reports**  
- Generated a **Service Information Report** in the **Garage Management Folder**, including:  
  - Customer Name, Appointment Date, Service Status, Payment Status.  

---

### 📊 **Task 12: Dashboards**  
- Built a **Service Rating Dashboard** using visually rich **line charts**, **bar graphs**, and **performance summaries**.  

---

## 🌟 **Conclusion**  
The **Garage Management System (GMS)** empowers automotive businesses by simplifying complex processes, improving efficiency, and enhancing customer satisfaction. Built with Salesforce, GMS delivers **real-time insights** and **streamlined workflows**, ensuring businesses stay ahead of the competition. 🚘💡

---
#**PRACTICAL VIDEO**
https://github.com/user-attachments/assets/56fa0956-d77d-4281-8e93-a2a41dad15fb
---
