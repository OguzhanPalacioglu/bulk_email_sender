# bulk_email_sender
-----------------------
This program is designed to automate bulk email sending by reading recipient information from an Excel file and creating personalized emails using Python.

# Features
------------------------
Read recipient information from an Excel file and insert it into the email template.
Send emails using an SMTP server.
Add a delay during email sending to avoid potential spam issues.

# Usage
-----------------------
Edit the smtp_server, smtp_port, sender_email, and sender_password variables in the mailler.py file to match your email provider and authentication details.
Customize the template in email_template and replace the placeholders ({{name}}, {{surname}}, {{age}}, {{city}}, etc.) with appropriate recipient information.
Create an Excel file containing recipient information. The column headers in your Excel file should be name, surname, age, city, etc., and each recipient should be placed in a separate row.
Run the Python script to start the email sending process: python3 mailler.py

# Warnings
-----------------------
Be sure to adjust the email sending rate according to your email provider's policies. Sending emails too quickly may result in emails being marked as spam.
When sending bulk emails, ensure that you have obtained permission from recipients and comply with permission-based email marketing laws.