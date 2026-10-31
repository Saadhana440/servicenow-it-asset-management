\# IT Asset Management System – Project Documentation



\## 1. Introduction



The IT Asset Management System is developed using the ServiceNow platform to manage IT assets and automate asset-related activities.



It provides a centralized way to maintain asset information, monitor warranty periods, and automate important operations using Business Rules and Flow Designer.



\## 2. Problem Statement



Managing IT assets manually can result in duplicate records, inaccurate asset information, and missed warranty expiration dates.



This project provides an automated solution to improve asset tracking, data accuracy, and warranty monitoring.



\## 3. Project Objectives



\- Develop a centralized IT asset management application.

\- Maintain asset details in a custom table.

\- Prevent duplicate serial numbers.

\- Automate default asset status assignment.

\- Track warranty expiration dates.

\- Automate warranty status updates.

\- Notify the IT team about upcoming warranty expirations.



\## 4. Technologies Used



\- ServiceNow Platform

\- Custom Tables

\- Business Rules

\- Flow Designer

\- Scheduled Triggers

\- Update Sets

\- XML

\- GitHub



\## 5. Database Design



\*\*Custom Table:\*\* `u\_it\_asset`



\### Fields



1\. Asset Name

2\. Asset Type

3\. Asset Status

4\. Assigned To

5\. Location

6\. Purchase Cost

7\. Purchase Date

8\. Warranty Expiry

9\. Serial Number

10\. Manufacturer

11\. Asset Description

12\. Warranty Status



\## 6. Business Rules



\### Rule 1: Prevent Duplicate Serial Number

Prevents duplicate serial number entries to maintain data accuracy.



\### Rule 2: Set Default Asset Status

Automatically assigns a default asset status when a new asset record is created.



\### Rule 3: Update Warranty Status

Automatically checks the warranty expiry date and updates the warranty status.



\- Future expiry date: Under Warranty

\- Past expiry date: Expired



\## 7. Flow Designer



\*\*Flow Name:\*\* IT Asset Warranty Expiry Alert



\*\*Trigger:\*\* Daily at 9:00 AM.



The workflow is designed to retrieve IT asset records, identify upcoming warranty expirations, process matching records, and send email notifications to the IT team.



\## 8. Expected Email Details



\- Asset Name

\- Serial Number

\- Asset Type

\- Assigned To

\- Warranty Expiry Date



\## 9. Testing



The following tests were performed:



| Test | Result |

|---|---|

| Future warranty date | Under Warranty |

| Past warranty date | Expired |

| Duplicate serial number | Duplicate prevention |

| Default asset status | Automatic assignment |



\## 10. Benefits



\- Better asset tracking.

\- Reduced manual work.

\- Improved data accuracy.

\- Automated warranty monitoring.

\- Better visibility of IT assets.



\## 11. Future Enhancements



\- Asset allocation management.

\- Asset maintenance reminders.

\- Advanced reporting dashboards.

\- Warranty renewal management.

\- Asset lifecycle tracking.



\## 12. Conclusion



The IT Asset Management System demonstrates how ServiceNow can be used to manage IT assets and automate business processes. It combines custom tables, Business Rules, and Flow Designer to improve operational efficiency.

