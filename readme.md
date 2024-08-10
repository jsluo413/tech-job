# Job Seeker Automation Website

## Goal
Create a website for job seekers that automates job applications by integrating features such as job listings from various job boards, user account management, application tracking, keyword extraction from job descriptions, and resume matching.

## Features and Functionalities
- **Job Listing**: Automatically pull job listings from various job boards.
- **User Registration and Login**: Enable users to sign up and log in securely.
- **User Dashboard**: Provide a dashboard for users to track their job applications.
- **Keyword Extraction**: Extract key information from job descriptions using NLP.
- **Resume Matching**: Offer suggestions for resume improvements and match resumes with job listings.

## Tech Stack
- **Operating System**: Ubuntu
- **Frontend**: React
- **Backend**: Node.js (Nest Framework)
- **Database**: AWS RDS or GCP SQL (MySQL or PostgreSQL)
- **Cloud Service**: AWS

## Development Process

### 1. Web Crawling
- **Framework**: BeautifulSoup
- **Data Collected**: Job title, Company name, Job description, Post time, Location
- **Storage**: Data stored in the database
- **Execution Frequency**: Every four hours

### 2. Database Design
- **Parallel Development**: Design the database schema based on the data structure needed for web crawling.
- **Integration**: Ensure seamless integration with the backend API.

### 3. Keyword Extraction and Resume Matching
- **Approach Options**:
  - **BERT**: Requires dataset and training.
  - **GPT**: Simple but might be costly in terms of tokens and money.
  - **Fine-tuning LLaMa**:
    - Requires paired datasets of job descriptions and resumes.
    - Involves pre-processing and fine-tuning the model.
    
### 4. Backend API Development
- Start after the database design and web crawling tasks are completed.

### 5. Frontend Development
- Develop simultaneously with backend API development once crawling and database setup are done.

## Additional Features
- **Job Alerts**: Send the latest job listings to users using SMTP (Python library).
