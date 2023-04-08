## JOB PORTAL
## 1.0. Introduction
### 1.1. Purpose
+ The purpose of the job site would be to provide a centralized platform where Kenyan job seekers can easily access and apply to recently posted job listings.

### 1.2. Product Scope
+ The job site will display recently posted jobs for Kenyan job seekers. The site will utilize web scraping to gather data about these jobs from various sources. The site will require users to log in to access the job listings.

### 1.3 Definitions, Accronyms and Abbreviations
+ None
## 2.0. Overall Solution Description
###  2.1. Overall Perspective
+ The diagram below shows the context diagram of the solution to be developed in the first sprint (the diagram will be modified as we add more features according to road map).

        +-----------------------+
        |                       |
        |  Web Application      |
        |                       |
        +-----------------------+
                   |
                   |
        +----------v-----------+
        |                      |
        |  Web Scraping Server |
        |                      |
        +----------+-----------+
                   |
                   | HTTP requests/responses
                   |
        +----------v-----------+
        |                      |
        |  External Websites   |
        |  and APIs            |
        |                      |
        +----------+-----------+
                   |
                   | Data extraction
                   |
        +----------v-----------+
        |                      |
        |  Data Storage        |
        |  (e.g. database)     |
        |                      |
        +----------+-----------+
                   |
                   | Data retrieval
                   |
        +----------v-----------+
        |                      |
        |  Web Application      |
        |                      |
        +-----------------------+

Summary of the external actors and systems:

+ Actors:

+ + Job seeker - user
+ + Admin - user

+ Interfacing Systems:

+ + SMS Gateway - send SMS using Tiara Connect API or standard SMPP v3.4
+ + Email Server - send email API, SMTP server
+ + Auth Server - authenticate user using Google Auth Server
Note: * - may not be included in the first sprint.

### 2.2. Product Functions
Below is a list of the main product functions in the system:

+ Job Seeker management
+ Job management
+ Authentication and authorization

### 2.3. System Users & their Characteristics
+ User 1: Job Seeker:

+ + main channels: Web via mobile or laptop
    other channels:
+ + SMS - notifications
+ + Email - notifications
+ characteristics:
+ + will mainly access service via a smart phone
+ + will be using this system on a day to day basis

+ + User 2: Admin

+ + main channel: Web via laptop
+ + other channels:
+ + Email - notifications
+ characteristics:
+ + does admin functions - mainly managing job seekers profiles and other system configurations
### 2.4. Operting Environment
The solution should be built to run on the cloud
### 2.5. Design and implementation considerations
+ None
### 2.6. User Documentation
+ + Requirements document
+ + Architecture document
+ + User guide*
+ + Technical operations guide
### 2.7. Assumptions and Dependancies
+ None
### 2.8. Assumptions and Dependancies
+ None
## 3.0 External Interface Requirements
### 3.1. User Interfaces
+ Web:

+ + Job seekers and admins will access the web
+ + It is the main user interface
It should be mobile friendly to Job seekers
+ SMS:

+ + Notifications to Job seekers
+ Email:

+ + Notifications to Job seekers
### 3.2. Hardware Interfaces
+ None
### 3.3. Software Interfaces
+ SMS Gateway API -
+ Email Server API - SMTP
+ Auth Servers - Google API
### 3.4. Communication Interfaces