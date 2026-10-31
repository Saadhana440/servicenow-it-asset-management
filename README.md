\# 🚀 IT Asset Management System | ServiceNow



\## 📌 Project Overview



The \*\*IT Asset Management System\*\* is a ServiceNow-based application developed to manage, monitor, and maintain IT assets efficiently.



The system provides centralized asset information, automated status updates, duplicate serial number prevention, and warranty tracking using ServiceNow Business Rules and Flow Designer.



It aims to reduce manual work, improve data accuracy, and simplify IT asset management.



\## 🎯 Problem Statement



Organizations manage multiple IT assets such as laptops, desktops, printers, and other devices. Tracking asset details, warranty periods, and asset status manually can lead to duplicate records, outdated information, and missed warranty expiry dates.



This project addresses these challenges by implementing an automated IT Asset Management solution using ServiceNow.



\## 🎯 Project Objectives



\- Create a centralized platform to manage IT assets.

\- Maintain complete asset information.

\- Prevent duplicate serial number entries.

\- Automatically assign default asset status.

\- Track warranty expiry dates.

\- Automatically update warranty status.

\- Automate upcoming warranty expiry notifications.

\- Improve asset management efficiency.



\## 🛠️ Technologies Used



| Technology | Purpose |

|---|---|

| ServiceNow | Application development platform |

| Custom Tables | Store IT asset information |

| Business Rules | Automate record operations |

| Flow Designer | Workflow automation |

| Update Sets | Capture configuration changes |

| XML | Configuration export |

| GitHub | Project version control and documentation |



\## 📦 Project Modules



\### 1. IT Asset Management Table



Created a custom table:



`u\_it\_asset`



The table stores the following information:



| Field | Description |

|---|---|

| Asset Name | Name of the IT asset |

| Asset Type | Category of the asset |

| Asset Status | Current asset status |

| Assigned To | Employee using the asset |

| Location | Asset location |

| Purchase Cost | Cost of the asset |

| Purchase Date | Purchase date |

| Warranty Expiry | Warranty expiration date |

| Serial Number | Unique asset serial number |

| Manufacturer | Asset manufacturer |

| Asset Description | Additional asset details |

| Warranty Status | Current warranty condition |



\### 2. Business Rules Automation



Implemented three Business Rules.



\*\*A. Prevent Duplicate Serial Number\*\*

\- Checks whether a serial number already exists.

\- Prevents duplicate serial number entries.



\*\*B. Set Default Asset Status\*\*

\- Automatically assigns a default status when a new asset is created.



\*\*C. Update Warranty Status\*\*

\- Checks the warranty expiry date.

\- Sets the status to Under Warranty when the expiry date is in the future.

\- Sets the status to Expired when the expiry date has passed.



\### 3. Flow Designer – Warranty Expiry Alert



Created a scheduled workflow named:



`IT Asset Warranty Expiry Alert`



\*\*Workflow components:\*\*

1\. Scheduled Trigger – Daily at 9:00 AM.

2\. Look Up Records – Retrieves IT asset records.

3\. For Each – Processes matching asset records.

4\. Condition – Identifies upcoming warranty expiry.

5\. Send Email – Intended to notify the IT team.



The intended notification includes:

\- Asset Name

\- Serial Number

\- Warranty Expiry Date

\- Asset Type

\- Assigned To



\*Document the email notification as completed only after successfully configuring and testing the action.\*



\## 🔄 System Workflow



```text

&#x20;      Start

&#x20;        |

&#x20;        v

&#x20; Create IT Asset

&#x20;        |

&#x20;        v

&#x20; Store Asset Details

&#x20;        |

&#x20;        v

&#x20;  Business Rules

&#x20;        |

&#x20;   +----+-----+

&#x20;   |          |

&#x20;   v          v

Duplicate    Default

Validation   Status

&#x20;   |          |

&#x20;   +----+-----+

&#x20;        |

&#x20;        v

&#x20; Warranty Status

&#x20;   Automation

&#x20;        |

&#x20;        v

&#x20;Scheduled Flow

&#x20; (Daily 9 AM)

&#x20;        |

&#x20;        v

&#x20; Find Upcoming

&#x20; Warranty Expiry

&#x20;        |

&#x20;        v

&#x20; Process Each Asset

&#x20;        |

&#x20;        v

&#x20; Email Notification

&#x20;        |

&#x20;        v

&#x20;       End

```



\## 🧪 Testing and Validation



The following functionalities were tested:



| Test Case | Expected Result |

|---|---|

| Future warranty expiry date | Under Warranty |

| Past warranty expiry date | Expired |

| Duplicate serial number | Duplicate entry prevented |

| New asset creation | Default status assigned |



\## 🌟 Key Benefits



\- Centralized IT asset management.

\- Reduced manual data entry.

\- Improved data accuracy.

\- Automated warranty tracking.

\- Better visibility of asset information.

\- Reduced risk of missing warranty expiry dates.

\- Improved IT asset management efficiency.



\## 🔮 Future Enhancements



\- Asset allocation and return management.

\- Dashboard for asset statistics.

\- Automated email reminders.

\- Warranty renewal tracking.

\- Asset maintenance scheduling.

\- Advanced reporting and analytics.



\## 📁 Project Folder Structure



```text

servicenow-it-asset-management/

│

├── README.md

│

├── Update-Set/

│   └── IT\_Asset\_Management\_Project.xml

│

├── Screenshots/

│   ├── Table/

│   ├── Business-Rules/

│   ├── Flow-Designer/

│   └── Testing/

│

└── Documentation/

&#x20;   └── Project-Description.md

```



\## 👩‍💻 Skills Demonstrated



\- ServiceNow Administration

\- Custom Table Creation

\- Field Configuration

\- Business Rules

\- Flow Designer

\- Scheduled Automation

\- Update Set Management

\- XML Export

\- Technical Documentation

\- GitHub



\## 👩‍🎓 Project Information



\*\*Project Name:\*\* IT Asset Management System



\*\*Platform:\*\* ServiceNow



\*\*Project Type:\*\* Application Development and Workflow Automation



\*\*Domain:\*\* IT Service Management (ITSM)



\*\*Author:\*\* R. Sakthishwari Saadhana



\---



⭐ \*Developed as a hands-on ServiceNow project to demonstrate IT asset management and automation capabilities.\*

