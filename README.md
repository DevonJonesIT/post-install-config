# osTicket - Post-Install Configuration

This tutorial outlines the post-install configuration of the open-source help desk ticketing system **osTicket**.

---

## **Video Demonstration**

- ### [YouTube: How To Configure osTicket, Post-Installation](https://www.youtube.com/results?search_query=how+to+configure+osticket+post+installation)

---

## **Environments and Technologies Used**

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

---

## **Operating Systems Used**

- Windows 10 (21H2)

---

## **Post-Install Configuration Objectives**

1. Configure Roles and Departments
2. Add New Agents and Assign Permissions
3. Configure User Authentication and Settings
4. Create Help Topics
5. Configure SLA (Service Level Agreement) Plans

---

## **Configuration Steps**

### **Step 1: Configure Roles and Departments**

1. Log in to the osTicket admin panel (`http://localhost/scp`).
2. Navigate to **Admin Panel** -> **Agents** -> **Roles**.
3. Add a new role and define its permissions (e.g., view tickets, close tickets).
4. Next, navigate to **Departments** and create a new department (e.g., "IT Support" or "Customer Service").
5. Assign the appropriate roles to the new department.

---

### **Step 2: Add New Agents and Assign Permissions**

1. In the osTicket admin panel, go to **Agents** -> **Add New Agent**.
2. Fill in the required fields:
   - **Name**: Enter the agent’s full name.
   - **Email**: Enter their work email (used for ticket notifications).
   - **Username**: Create a unique username for the agent.
3. Assign the agent to the appropriate **department** and **role**.
4. Save the new agent and confirm their account.

---

### **Step 3: Configure User Authentication and Settings**

1. Navigate to **Admin Panel** -> **Settings** -> **Users**.
2. Enable or disable user registration based on your organization’s needs.
3. Enable **"Require registration and login to create tickets"** if you want only registered users to submit tickets.
4. Optionally, configure **LDAP/Active Directory integration** for centralized user management.

---

### **Step 4: Create Help Topics**

1. Go to **Admin Panel** -> **Manage** -> **Help Topics**.
2. Add categories for common support issues (e.g., "Password Reset," "Network Issues," "Software Requests").
3. For each help topic, specify:
   - **Name**: The title of the help topic.
   - **Description**: A brief explanation of the issue.
   - **Assigned Department**: The department responsible for handling the request.

---

### **Step 5: Configure SLA (Service Level Agreement) Plans**

1. Navigate to **Admin Panel** -> **Manage** -> **SLA Plans**.
2. Create new SLA plans based on priority levels (e.g., "High Priority," "Standard Support").
3. For each SLA plan, configure:
   - **Grace Period**: The amount of time allowed before the ticket becomes overdue.
   - **Schedule**: The business hours during which tickets are addressed.
   - **Notification Settings**: Set reminders and overdue alerts for pending tickets.

---

## **Final Configuration Checks**

1. Ensure your **email settings** (SMTP and IMAP) are properly configured to send and receive email notifications.
2. Perform a test by submitting a ticket through the client portal and verifying that agents receive notifications.
3. Adjust **auto-responses** and **escalation rules** as needed to align with your team’s workflow.

---

## **Additional Resources**

- [osTicket Official Documentation](https://docs.osticket.com/)
- [osTicket Community Forums](https://forum.osticket.com/)
