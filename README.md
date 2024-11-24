# **NAAN MUDHALVAN - SALESFORCE REPORT**  
### **A CRM Application To Manage The Services Offered by an Institution**  

---

## **Project Team**  
| **Name**               | **Roll Number**    |
|------------------------|--------------------|
| Arunkumar V           | 421622243003       |
| Keerthi K             | 421622243026       |
| Yashwanth Kumar A     | 421622243057       |
| Pugazhendhi N         | 421622243041       |
| Hariharan S           | 421622243020       |

---

## **Abstract**  
The Salesforce-based **Garage Management System (GMS)** is a comprehensive solution for automotive repair businesses. It leverages Salesforce's CRM capabilities to automate processes like appointment scheduling, inventory management, billing, and customer communication. GMS ensures streamlined operations, top-notch service, and competitive advantage for repair facilities.  


## **Detailed Tasks**

### **Task 1: Creating Developer Account**  
1. Visit [Salesforce Developer Signup](https://developer.salesforce.com/).
2. Fill the signup form:
   - **First Name, Last Name, Email, Role**: Developer  
   - **Company**: College Name  
   - **Country**: India  
   - **Postal Code**: PIN code  
   - **Username**: Format `username@organization.com`  
3. Activate your account by verifying the email.

---

### **Task 2: Creating Custom Objects**
#### **Objects Created:**
1. **Customer Details**  
   - Record Name: `Customer Name`  
   - Data Type: `Text`
2. **Appointment**  
   - Record Name: `Appointment Name`  
   - Auto Number: `app-{000}`
3. **Service Records**  
   - Record Name: `Service Records Name`  
   - Auto Number: `ser-{000}`
4. **Billing Details and Feedback**  
   - Record Name: `Billing Details and Feedback Name`  
   - Auto Number: `bill-{000}`

---

### **Task 3: Creating Custom Tabs**  
Custom tabs were created for:  
- Customer Details  
- Appointments  
- Service Records  
- Billing Details and Feedback  

---

### **Task 4: Building Lightning App**  
Created a **Garage Management Application** with:  
- Navigation items: Customer Details, Appointments, Service Records, Reports, Dashboards.  
- User Profiles: System Administrator.  

---

### **Task 5: Creating Fields**  
| **Object**                  | **Field**                  | **Type**    | **Notes**                       |
|-----------------------------|----------------------------|-------------|----------------------------------|
| Customer Details            | Phone Number              | Phone       | Captures customer contact info. |
| Appointment                 | Vehicle Number Plate      | Text        | Unique, Required (10 chars).    |
| Service Records             | Service Status            | Picklist    | Values: `Started`, `Completed`. |
| Billing Details and Feedback| Payment Status            | Picklist    | Values: `Pending`, `Completed`. |

---

### **Task 6: Validation Rules**  
1. **Appointment Object**  
   - Vehicle Number Plate format: `[A-Z]{2}[0-9]{2}[A-Z]{2}[0-9]{4}`  
2. **Service Records Object**  
   - Service Status must be `Completed`.  
3. **Billing Details and Feedback**  
   - Rating should be between `1` and `5`.  

---

### **Task 7: Duplicate Rules**  
- Created matching and duplicate rules for **Customer Details** based on **Email** and **Phone Number**.

---

### **Task 8: Profiles**  
1. **Manager Profile**  
   - Default app: Garage Management Application  
   - Permissions: All custom objects.  
2. **Sales Person Profile**  
   - Permissions: Limited to relevant custom objects.

---

### **Task 9: Roles**  
- **Manager** role created under CEO.  
- **Sales Person** role created under Manager.

---

### **Task 10: Users**  
- Manager and Sales Person users created with appropriate roles and profiles.

---

### **Task 11: Public Groups**  
Created a public group named **Sales Team** with the **Sales Person** role.

---

### **Task 12: Sharing Settings**  
- **Service Records Object**:  
   - OWD: Private  
   - Sharing Rule: Sales Person → Manager (Read/Write).

---

### **Task 13: Flows**  
Built a **Record-Triggered Flow** for **Billing Details and Feedback**:  
- Triggers email alerts upon payment completion.

---

### **Task 14: Apex Triggers**  
- **Trigger**: AmountDistribution  
   - Calculates service amount based on selected services.  

---

### **Task 15: Reports**  
- Created **Garage Management Folder**.  
- Generated a **Service Information Report** with fields:  
   - Customer Name, Appointment Date, Service Status, Payment Paid.

---

### **Task 16: Dashboards**  
- Built **Service Rating Dashboard** with line charts and shared with appropriate roles.

---

## **Conclusion**  
The **Garage Management System** on Salesforce streamlines operations, enhances service quality, and ensures a competitive edge for automotive repair facilities. With its comprehensive CRM capabilities, it simplifies daily operations and provides actionable business insights.

---
