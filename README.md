# A CRM Application For Wholesale Rice Mill

The SmartBridge Salesforce project is a customized CRM application tailored for the wholesale rice mill industry. The application enables seamless management of rice production, sales, and customer interactions. It offers features such as daily tracking of rice production, sales, customer data, and real-time reporting, improving efficiency and decision-making for rice mill owners.

## Key Features

1. **Custom Object Design:**
   - Custom objects for Supplier, Rice Mill, Consumer, and Rice Details were created to capture essential data related to rice production, sales, and distribution.
   
2. **Workflow Automation:**
   - Automated workflows for key processes like order processing, inventory management, and customer communication, reducing manual efforts and enhancing accuracy.

3. **Enhanced User Experience:**
   - Custom page layouts and fields for an intuitive user experience aligned with the operational needs of the rice mill business.

4. **Role-Based Access Control:**
   - Role hierarchies were defined, ensuring data visibility and access permissions were aligned with user roles (Owner, Employer, Worker).

5. **Analytics and Reporting:**
   - Multiple report types (Tabular, Summary, Matrix) were utilized to gain actionable insights into sales trends, inventory levels, and customer preferences.

6. **Visual Dashboards for Insights:**
   - Dynamic dashboards provide visual representations of critical metrics such as daily sales, production quantities, and customer feedback.

7. **Collaborative Efficiency:**
   - Sharing reports and subscribing to automated updates enabled team collaboration with access to real-time information essential for various roles.

8. **Continuous Improvement:**
   - Continuous refinement and enhancements based on user feedback ensure the CRM adapts to evolving business needs and maintains operational excellence.

## Milestones and Activities

### Milestone 1: Salesforce Introduction

**What is Salesforce?**
Salesforce is a customer success platform designed to help you sell, service, market, and connect with your customers. It provides a comprehensive suite for managing relationships, collaborating with employees and partners, and securely storing data.

#### Activity 1: Creating Developer Account
Sign up at [Salesforce Developer Signup](https://developer.salesforce.com/signup).

#### Activity 2: Account Activation
Verify email, set a password, and access the Salesforce setup page.

### Milestone 2: Object Creation

- **What is an Object?**  
  Objects in Salesforce are database tables that store data specific to an organization.

  - **Standard Objects:** Predefined by Salesforce.
  - **Custom Objects:** Created by users for specific business requirements.

#### Activities:
1. **Supplier Object:**  
   - Label Name: Supplier  
   - Record Name: Supplier Name (Text)  
   - Enable: Reports, Track Field History
2. **Rice Mill Object:**  
   - Label Name: Rice Mill  
   - Record Name: Auto Number (rice-{000})
3. **Consumer Object:**  
   - Label Name: Consumer  
   - Record Name: Auto Number (consumer-{000})
4. **Rice Details Object:**  
   - Label Name: Rice Details  
   - Record Name: Auto Number (rice-{000})

### Milestone 3: Tabs

- **What is a Tab?**  
  A tab in Salesforce allows users to build and view records for objects.

#### Activities:
1. **Creating a Custom Tab (Supplier):**
   - Setup → Tabs → Custom Object Tabs → New  
   - Select Object (Supplier) → Tab Style → Save.

2. **Creating Tabs for Rice Mill, Consumer, and Rice Details:**
   - Repeat the above steps for other objects.

### Milestone 4: The Lightning App

- **What is a Lightning App?**  
  A collection of items that work together to serve a specific function, accessible via a navigation bar.

#### Activity 1: Creating a Lightning App
- Setup → App Manager → New Lightning App  
- App Name: `MY RICE` → Add navigation items (Supplier, Rice Mill, Consumer, Rice Details).

### Milestone 5: Fields

- **What are Fields?**  
  Data stored in the columns of a relational database.

#### Activity 1: Creating Number Field in Rice Details Object
- Setup → Object Manager → Rice Details Object → Fields & Relationships → New  
- Data Type: Number → Field Label: `Rice Distributed`.

#### Activity 2: Creating Junction Object
- Setup → Object Manager → Rice Details Object → Fields & Relationships → New  
- Data Type: Master-Detail → Related Object: Supplier.

### Milestone 6: Page Layouts

Page layouts allow you to customize detail and edit pages.

#### Activity 1: Creating a Page Layout
- Setup → Object Manager → Select Object (e.g., Consumer) → Page Layouts → New  
- Create sections like "Personal Details", "Rice Details", and "Receipt Details".

### Milestone 7: Profiles

Profiles define user permissions and access settings.

#### Activities:
1. **Owner Profile:**
   - Clone the Standard User profile, set permissions for Consumers, Rice Details, Rice Mill, and Suppliers.
   
2. **Employer and Worker Profiles:**
   - Create profiles with customized access.

### Milestone 8: Role & Role Hierarchy

Roles define record-level visibility for users.

#### Activities:
1. **Creating Owner Role:**
   - Setup → Roles → Add role labeled `Owner`.

2. **Employer and Worker Roles:**
   - Add roles under the Owner role.

### Milestone 9: Users

#### Activity 1: Creating Users
- Setup → Users → New User → Assign roles (Owner, Employer, Worker).

### Milestone 10: Permission Sets

#### Activity 1: Adjusting Organization-Wide Defaults (OWD)
- Setup → Sharing Settings → Set "Public Read-Only" for Rice Mill and Supplier objects.

### Milestone 11: Reports

Reports provide insights into data.

#### Activity 1: Create Report
- Reports tab → New Report → Select "Rice Mill with Consumers".

#### Activity 2: Sharing Reports
- Edit the report → Subscribe → Configure email notifications.

### Milestone 12: Dashboards

Dashboards visualize data from reports.

#### Activity 1: Create Dashboard
- Dashboards tab → New Dashboard → Add components like bar and donut charts.

## Conclusion

The CRM application developed for our wholesale rice mill revolutionized our operations, customer relationships, and data insights. It enabled automation, enhanced user experience, and improved decision-making through powerful reporting and analytics features.

### Result Image:
![CRM Application Result](result.jpg)
