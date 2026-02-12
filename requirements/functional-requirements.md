#Functional Requirements

## 1.User Management
The user will be able to register an account, log in to the account and log out of it.
1.1 The system shall allow users to register, log in, manage their accounts, and update personal information through an interface.
1.2 The system shall support registration, authentication, and access control for four distinct roles: Owner, Tenant, Supervisor, and Maintenance Provider.
1.3 The system shall support account creation using either mobile number or email, and shall verify identity using a One-Time Password (OTP).
1.4 The system shall provide secure login/logout functionality and allow users to reset their password through OTP-based verification.
1.5 The system shall allow users to update their personal information, including name, contact details, and profile picture.
1.6 The system shall enforce Role-Based Access Control (RBAC) to ensure each role only accesses data and functionalities permitted to them. 


## 2.Linking Users to Units
The user shall be linked to the unit.
2.1 The system shall link residents accounts to their respective units only after validating building and unit information.
2.2 The system shall prevent residents from viewing or modifying any unit information not associated with their account.

## 3.Profile Visibility & Privacy
The system shall allow the user to control the visibility of their profile information.
3.1 The system shall allow residents to control the visibility of their profile information to other residents.
3.2 The system shall allow only residents of the same building to view each other’s profiles, subject to individual visibility settings.
3.3 The system shall allow residents to hide their profile picture so that it is not visible to any other resident.
3.4 The system shall log all changes made to profile visibility and privacy settings for auditing purposes.

## 4.Maintenance Requests 
The user shall be able to create Personal or Community Maintenance Requests, describe the issue, attach media, track maintenance progress and view their maintenance history, and choose from verified providers, submit feedback on maintenance requests. 
4.1 The system shall allow residents to submit Personal or Community Maintenance Requests with attachments, notes, and preferred visit times including entry instructions. 
4.2 The system shall include an AI Agent that analyzes the issue type and recommends top-rated verified providers.
4.3 The system shall display verified providers ranked by rating, response time, price, and relevance.
4.4 The system shall display only verified providers to residents.
4.5 The system shall allow supervisors to add and remove verified providers.
4.6 The system shall send the full request details to the selected maintenance provider through the internal interface.
4.7 The system shall allow residents to track maintenance progress and view their maintenance history.
4.8 The system shall allow residents to submit feedback on maintenance requests, whether Personal or Community, including ratings and comments, which shall be visible to supervisors and used for provider evaluation.

## 5.Maintenance Provider Actions
The user will receive notification about maintenance requests, accept or reject requests. 
5.1 The system shall notify maintenance providers when new requests are assigned to them. 
5.2 The system shall allow providers to accept or reject requests and shall notify residents of the decision. 
5.3 The system shall prevent providers from canceling accepted requests without Supervisor approval. 
5.4 The system shall log all provider actions for auditing. 

## 6.Community Maintenance 
The user will be able to vote on community maintenance and receive notification about it.
6.1 The system shall allow residents to vote on Community Maintenance requests and approve providers.
6.2 The system shall schedule approved Community Maintenance requests based on the agreed-upon date and time selected by the residents, after verifying that the required payment has been successfully processed. 6.3 The system shall allow supervisors to monitor request progress and generate performance and maintenance reports.
6.4 The system shall send notifications regarding shared expenses and payment deadlines.

## 7.Notification Management 
The user will receive notification, and will be able to manage it.
7.1 The system shall send push notifications via mobile and email for all important updates, including maintenance request status changes, visit scheduling and completion, payment confirmations, document expirations or approvals, community voting results.
7.2 The system shall allow residents to manage and customize their notification preferences. 
7.3 The system shall log all notifications for auditing purposes.

## 8.Payment & Billing 
The user will be able to view bills, pay electronically, receive remainders, and view payment status
8.1 The system shall allow residents to view bills, pay electronically, or upload manual payment receipts.
8.2 The system shall generate billing reminders and issue digital payment receipts.
8.3 The system shall maintain a complete payment history for each resident and unit. 
8.4 The system shall provide providers with a dashboard to view payment status for each request, including pending, completed, and failed payments.

## 9.Community & Interaction 
The user shall be able to join groups chats. 
9.1 The system shall allow residents to join group chats and participate in announcements and voting activities. 
9.2 The system shall securely store chat logs for auditing.

## 10.Document & Data Management (Digital Passport) 
The user can upload documents, and search and filter documents. 
10.1 The system shall allow residents to upload documents such as contracts, invoices, warranties, and photos, and automatically categorize them.
10.2 The system shall allow residents to search and filter documents by type or date.
10.3 The system shall enforce role-based access for all documents (Owner, Tenant, Supervisor, Provider). 
10.4 The system shall track document expiry dates and send automated reminders.
10.5 The system shall maintain document versions and log all modifications for auditing.

## 11.Visit Management 
The user can review and approve visit date and time, update visit status, and supervisors can access all visit logs
11.1 The system shall allow residents to review and approve scheduled visit dates and times. 
11.2 The system shall allow providers to update visit status: On the Way, Arrived, Work Started, and Completed. 
11.3 The system shall send notifications to residents upon technician arrival and completion of work. 
11.4 The system shall store visit logs including start/end time, technician name, and notes. 
11.5 The system shall allow supervisors to access all visit logs for auditing and performance tracking. 

## 12.Chatbot Assistant 
The user can interact with the chatbot. 
12.1 The system shall support both Arabic and English languages in chatbot interactions. 
12.2 The system shall integrate the chatbot with resident, Maintenance, Payment, and Document modules. 
12.3 The system shall provide role-based chatbot responses and require confirmation before performing sensitive actions. 
12.4 The system shall securely log all chatbot interactions.

## 13.Predictive Maintenance 
The user can request predictive maintenance.
13.1 The system shall collect historical maintenance data including issue type, frequency, resolution details, and equipment involved.
13.2 The system shall analyze collected data to detect recurring issues or operational risks. 
13.3 The system shall generate predictions for potential equipment failures.
13.4 The system shall create recommended maintenance tasks generated from predictions. 
13.5 The system shall notify supervisors based on risk level (low, medium, high).
13.6 The system shall categorize predicted issues by severity and urgency. 
13.7 The system shall allow supervisors to review prediction details and convert them into scheduled visits. 
13.8 The system shall continuously update predictions as new data becomes available. 
13.9 The system shall maintain a log of all predictive alerts for auditing.
