# 🤖 Job Application Bot – UiPath RPA Automation with Gmail

An automated **Job and Internship Application Email System** built using UiPath Studio and Gmail SMTP. This project automates repetitive application emails by reading company details from Excel, generating personalized email content, attaching resumes, sending emails through Gmail, handling failures with retry logic, and maintaining execution logs.

## 📌 Project Overview

Applying for internships and jobs often involves sending similar emails to multiple companies. Performing this process manually is repetitive and time-consuming.

The Job Application Bot automates this process using Robotic Process Automation (RPA).

The bot:
- Reads company information from an Excel spreadsheet.
- Loads email and SMTP configurations from a separate Excel file.
- Personalizes email subjects and messages using placeholders.
- Attaches the appropriate resume or CV.
- Sends application emails using Gmail SMTP.
- Implements retry mechanisms for failed email attempts.
- Records execution results in an Excel log file.

## 🎯 Objectives

- Reduce manual effort in sending job and internship applications.
- Automate repetitive email communication.
- Generate personalized emails for multiple companies.
- Improve consistency and reduce manual errors.
- Maintain an organized record of application attempts.

## ⚙️ Workflow Architecture

![Job Application Bot Workflow](workflow-diagram.png)

### Process Flow

1. **Initialize:** Start the bot and load configuration settings.
2. **Load Data:** Read `Config.xlsx` and `Companies.xlsx`.
3. **Process Companies:** Iterate through each company record.
4. **Personalize Email:** Replace placeholders such as `{CompanyName}` with company-specific values.
5. **Send Email:** Send the personalized application using Gmail SMTP.
6. **Retry Handling:** Retry failed email attempts according to the configured retry settings.
7. **Log Results:** Record timestamps,
