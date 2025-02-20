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

![Setting up osTicket](https://imgur.com/a/7phIdPu)


---

### 2. Installing HeidiSQL
To manage the MySQL database efficiently, I installed **HeidiSQL**. This tool provides an easy-to-use interface for connecting to MySQL databases.

![Installing HeidiSQL](images/Screenshot-2.png)

---

### 3. Connecting to MySQL
After installing HeidiSQL, I created a connection to the MySQL database. The hostname was set to `127.0.0.1`, and the root user was used for database authentication.

![Connecting to MySQL](images/Screenshot-3.png)

---

### 4. Creating the Database
Next, I created a **new MySQL database** for osTicket using HeidiSQL. The database was named `osTicket`.

![Creating the Database](images/Screenshot-4.png)

---

### 5. Completing osTicket Setup
Once the database was created, I linked it to osTicket by providing the MySQL **hostname, database name, username, and password** in the osTicket setup page.

![Completing osTicket Setup](images/Screenshot-5.png)

---

### 6. Accessing the Admin and User Portals
After completing the installation, osTicket was fully set up, and I accessed the admin and user portals.

#### Admin Login Page
This is where administrators and support agents log in to manage tickets.

![Admin Login Page](images/Screenshot-6.png)

#### End-User Support Page
Users can create new support tickets and check the status of their existing tickets.

![End-User Support Page](images/Screenshot-7.png)

#### Admin Dashboard
From the admin panel, I can manage users, tickets, and system configurations.

![Admin Dashboard](images/Screenshot-8.png)

#### Roles & Permissions
Different levels of access are assigned to various agents.

![Roles and Permissions](images/Screenshot-9.png)

---

### 7. Creating User Roles
I created a **SupremeAdmin** role and assigned it full permissions to perform all actions within osTicket.

![Creating User Roles](images/Screenshot-10.png)

---

### 8. Setting Up Help Topics
I added multiple **help topics** for end-users to choose from when submitting a ticket. These include:
- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
- Other

![Setting Up Help Topics](images/Screenshot-11.png)

---

### 9. Configuring SLA Plans
I created **Service Level Agreements (SLA)** to prioritize ticket resolution:
- **Sev-A**: 1-hour grace period, 24/7 support
- **Sev-B**: 4-hour grace period, 24/7 support
- **Sev-C**: 8-hour grace period, business hours only

![Configuring SLA Plans](images/Screenshot-12.png)

---

### 10. Creating End Users
I created two **end users** who will submit tickets to the support team for resolution.

![Creating End Users](images/Screenshot-13.png)

---

### 11. Adding Agents
I added **two agents** (employees) and assigned them to a department. Each agent was given appropriate permissions based on their role.

![Adding Agents](images/Screenshot-14.png)

---

### 12. Creating Teams
I created an **Online Banking Team**, which will be responsible for handling specific types of support requests.

![Creating Teams](images/Screenshot-15.png)

---

### 13. Creating Departments
A **SysAdmins Department** was created to manage IT-related issues within the organization.

![Creating Departments](images/Screenshot-16.png)

---

## Conclusion
This project showcases the complete installation and configuration of osTicket on a local server. With osTicket successfully set up, I can now manage support tickets efficiently. 

If you're interested in setting up your own osTicket system, feel free to follow this guide. Contributions and suggestions are welcome!

---
## Contact
For any questions, feel free to reach out via GitHub Issues.

