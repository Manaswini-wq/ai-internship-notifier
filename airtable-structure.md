# 📊 Airtable Structure – AI Internship Matcher

This Airtable base contains two main tables:

---

## 🔹 1. Internships Table

Used to store internship listings.

| Field Name       | Field Type        | Description                              |
|------------------|-------------------|------------------------------------------|
| Title            | Single line text  | Name of the internship                   |
| Company          | Single line text  | Company offering the role                |
| Location         | Single line text  | City/Remote                              |
| Description      | Long text         | Detailed description of the role         |
| Skills Required  | Single line text  | Comma-separated required skills          |

---

## 🔹 2. Applicants Table

Used to store form submissions from Replit.

| Field Name         | Field Type        | Description                             |
|--------------------|-------------------|-----------------------------------------|
| Name               | Single line text  | Applicant name                          |
| Email              | Email             | Applicant email                         |
| College            | Single line text  | College or university name              |
| Skills             | Long text         | Skills (entered by user)                |
| Career Interests   | Long text         | Preferred fields or roles               |
| Submitted At       | Created time      | Automatically added timestamp           |

---

📌 These table names and field types are referenced inside the `n8n` workflow.
