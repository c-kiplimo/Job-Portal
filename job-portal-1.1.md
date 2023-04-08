### JOB PORTAL
## 1.0. Introduction
# 1.1. Purpose
+ The purpose of the job site would be to provide a centralized platform where Kenyan job seekers can easily access and apply to recently posted job listings.
# 1.2. Product Scope
+ The job site will display recently posted jobs for Kenyan job seekers. The site will utilize web scraping to gather data about these jobs from various sources. The site will require users to log in to access the job listings.

# 1.3 Definitions, Accronyms and Abbreviations
+ None
## 2.0. Overall Solution Description
#  2.1. Overall Perspective
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
