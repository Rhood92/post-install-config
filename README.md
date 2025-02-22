# osTicket Installation and Configuration

## Overview
This repository documents my step-by-step installation and configuration of the **osTicket** ticketing system. osTicket is an open-source help desk solution that allows for efficient ticket management.

## Table of Contents
- [System Requirements](#system-requirements)
- [Installation Steps](#installation-steps)
  - [1. Setting Up osTicket](#1-setting-up-osticket)
  - [2. Installing HeidiSQL](#2-installing-heidisql)
  - [3. Connecting to MySQL](#3-connecting-to-mysql)
  - [4. Creating the Database](#4-creating-the-database)
  - [5. Completing osTicket Setup](#5-completing-osticket-setup)
  - [6. Accessing the Admin and User Portals](#6-accessing-the-admin-and-user-portals)
  - [7. Creating User Roles](#7-creating-user-roles)
  - [8. Setting Up Help Topics](#8-setting-up-help-topics)
  - [9. Configuring SLA Plans](#9-configuring-sla-plans)
  - [10. Creating End Users](#10-creating-end-users)
  - [11. Adding Agents](#11-adding-agents)
  - [12. Creating Teams](#12-creating-teams)
  - [13. Creating Departments](#13-creating-departments)
- [Conclusion](#conclusion)

---

## System Requirements
Before setting up osTicket, ensure you have the following:
- A web server (IIS)
- PHP
- MySQL Database
- HeidiSQL (for database management)

---

## Installation Steps

### 1. Setting Up osTicket
First, I began the installation process by setting up the osTicket system. I configured the **Helpdesk Name, Default Email, and Admin User Account**.

![image](https://github.com/user-attachments/assets/bbf9813a-1066-422f-b9a2-097529f72a13)



---

### 2. Installing HeidiSQL
To manage the MySQL database efficiently, I installed **HeidiSQL**. This tool provides an easy-to-use interface for connecting to MySQL databases.

![image](https://github.com/user-attachments/assets/185b5dbf-199e-4011-bc70-e56597421c31)


---

### 3. Connecting to MySQL
After installing HeidiSQL, I created a connection to the MySQL database. The hostname was set to `127.0.0.1`, and the root user was used for database authentication.

![image](https://github.com/user-attachments/assets/0fdba1f1-c862-45e0-ba9f-b7b0fe47d149)


---

### 4. Creating the Database
Next, I created a **new MySQL database** for osTicket using HeidiSQL. The database was named `osTicket`.

![image](https://github.com/user-attachments/assets/811f79d1-5a41-46b8-a24a-6a65f35bc44f)


---

### 5. Completing osTicket Setup
Once the database was created, I linked it to osTicket by providing the MySQL **hostname, database name, username, and password** in the osTicket setup page.

![image](https://github.com/user-attachments/assets/23012c31-7152-4097-8ebc-83cec754060c)


---

### 6. Accessing the Admin and User Portals
After completing the installation, osTicket was fully set up, and I accessed the admin and user portals.

#### Admin Login Page
This is where administrators and support agents log in to manage tickets.

![image](https://github.com/user-attachments/assets/9c860ed3-b9d6-4785-931c-425735747629)


#### End-User Support Page
Users can create new support tickets and check the status of their existing tickets.

![image](https://github.com/user-attachments/assets/b60c0377-0243-4a88-8be9-551c75d70ad9)


#### Admin Dashboard
From the admin panel, I can manage users, tickets, and system configurations.

![image](https://github.com/user-attachments/assets/cd31276b-202a-4f91-b5a6-edf2b72dda82)


#### Roles & Permissions
Different levels of access are assigned to various agents.

![image](https://github.com/user-attachments/assets/e66f1000-e0e8-4e43-8246-4397b352432c)


---

### 7. Creating User Roles
I created a **SupremeAdmin** role and assigned it full permissions to perform all actions within osTicket.

![image](https://github.com/user-attachments/assets/5b179e7e-8538-46ac-ba8d-1dcd3641c4ad)

![image](https://github.com/user-attachments/assets/2ac81beb-462a-4b7d-a8e8-3b4f0c85f508)

![image](https://github.com/user-attachments/assets/0d7767f6-b1ad-47ac-b7ae-ea563fc3e917)


---

### 8. Setting Up Help Topics
I added multiple **help topics** for end-users to choose from when submitting a ticket. These include:
- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
- Other

![image](https://github.com/user-attachments/assets/a1959e61-1464-4dff-8bae-29ed0470dde5)


---

### 9. Configuring SLA Plans
I created **Service Level Agreements (SLA)** to prioritize ticket resolution:
- **Sev-A**: 1-hour grace period, 24/7 support
- **Sev-B**: 4-hour grace period, 24/7 support
- **Sev-C**: 8-hour grace period, business hours only

![image](https://github.com/user-attachments/assets/83bc893b-777e-44f1-9819-7d4291d08a34)


---

### 10. Creating End Users
I created two **end users** who will submit tickets to the support team for resolution.

![image](https://github.com/user-attachments/assets/eb8ab531-690b-44b7-a0e6-fe3d45146442)


---

### 11. Adding Agents
I added **two agents** (employees) and assigned them to a department. Each agent was given appropriate permissions based on their role.

![image](https://github.com/user-attachments/assets/26351b38-60c0-4cfd-9265-608849f88a53)


---

### 12. Creating Teams
I created an **Online Banking Team**, which will be responsible for handling specific types of support requests.

![image](https://github.com/user-attachments/assets/17f918fa-8267-40b6-8236-8836036c298a)


---

### 13. Creating Departments
A **SysAdmins Department** was created to manage IT-related issues within the organization.

![image](https://github.com/user-attachments/assets/47dfd52f-5e8b-451e-9b4e-49c37afdb6ba)

---

## Conclusion
This project showcases the complete installation and configuration of osTicket on a local server. With osTicket successfully set up, I can now manage support tickets efficiently. If you're interested in setting up your own osTicket system, feel free to follow this guide! **Check out the last section of my project entitled "Ticket Lifecycle Examples".**




