Java Junior-level technical task

Description:
Application for scraping jobs from jobs.techstars.com by specific job function


User story:
As a user, I want to have an application that can scrape job listings from jobs.techstars.com based on specific job functions. The application should allow me to input the desired work functions or job categories I am interested in, and then it should automatically crawl the website to gather relevant job postings for those functions. The scraped data should be presented in a user-friendly format, showing key details. Additionally, I would like the application to have an option to filter or sort the results based on different criteria, such as job location or posting date. This will help me efficiently find and explore job opportunities tailored to my preferences, ultimately simplifying the job search process and improving my overall experience on the jobs.techstars.com platform.


List page:
Url to page - https://jobs.techstars.com/jobs
Use the “Job function” dropdown menu to choose a specific job function.
Collect all jobs filtered by specific job function

job function dropdown menu
number of filtered jobs results
job item
tags


Item:
For every job, you need to gather next points:

position name
url to organization
logo
organization title
labor function
address
posted date
description

Data to collect (Data points):
(If some data is not provided, the field should be 'NOT_FOUND')
job page url on jobs.techstars.com
position name
url to organization
logo (save only link to image)
organization title
labor function
location (can be one line string)
posted date (can be one line string, preferer - parse and save in Unix Timestamp)
description (can be as text content, preferee - save with html formatting)
tags names (can be one line string separated by coma)


Technical requirements:
For sending requests to the website, you can use any of the following:
okhttp
jsoup
As framework you can use - Spring Boot
If you decide to render page to get information from site pages, use any of the following:
Selenium
Playwright
Database for storing data - any of sql (PostgreSQL, MySQL)
Datasource interaction through ORM
Build tools preference use the Maven

Must have:
All your source code should be uploaded to VCS. (GitHub, GitLab, Bitbucket)
Enforcement of Object-Oriented Programming (OOP) principles and adherence to clean code practices
Scraping results - only first page of one of any job function
Scraping results can be dump to SQL file, with database creation schema or in CSV format
INSTALL.md - instructions on how to configure and run the project
README.md - with short description


As plus:
Use docker
Use multithreaded
Upload results into Google Sheet (through google api by application)

Result of task:
Fully working code with additional files (INSTALL.md, README.md) uploaded on any VCS
Scraping results in SQL database dump uploaded on google drive or CSV file
