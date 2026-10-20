# Assignment 9: n8n Automation – Google Sheets to Gmail

## 📌 Project Overview

This project demonstrates an automation workflow built using **n8n** that reads data from Google Sheets, formats it into a structured email, and sends it through Gmail automatically.

The workflow reduces manual work by retrieving spreadsheet records and converting them into a readable email summary.

## 🎯 Objectives

- Read records from Google Sheets.
- Format spreadsheet data into a clear email subject and body.
- Send the email using Gmail.
- Handle empty sheets without sending blank emails.
- Log the empty-sheet condition.
- Export and maintain the workflow as a JSON file.

## 🛠️ Tools & Technologies

- **n8n** – Workflow automation
- **Google Sheets** – Data source
- **Gmail** – Email delivery
- **JavaScript** – Email formatting using the Code node
- **GitHub** – Workflow version control and project submission

## 🔄 Workflow Overview

The automation follows these steps:

1. **Manual Trigger** – Starts the workflow.
2. **Google Sheets** – Retrieves rows from the spreadsheet.
3. **IF Node** – Checks whether data is available.
4. **Code Node** – Formats the records into a structured email.
5. **Gmail** – Sends the formatted email to the chosen recipient.
6. **Logging Node** – Records a message when no data is available.

### Workflow Logic

- If data is available, the workflow formats the records and sends an email.
- If the sheet is empty, the workflow follows the logging branch and avoids sending a blank email.

## 📧 Sample Email

**Subject:** CAIE Course Program – Data Summary

**Body:**

Hi,

Here is the latest data from the Google Sheet.

- Name: Arun Kumar
- Course: CAIE Mathematics
- Status: Enrolled

Regards,  
Your Automation Bot

## 📂 Repository Contents

| File | Description |
|---|---|
| `CAIE Course Program.json` | Exported n8n workflow configuration |
| `Screenshot 2026-10-20 202628.png` | Workflow screenshot |
| `Screenshot 2026-10-20 202758.png` | Workflow screenshot |
| `▶️ CAIE Course Program - n8n - Google Chrome 2026-10-20 20-31-24.mov` | Workflow demonstration video |
| `.gitattributes` | Git file-handling configuration |
| `.gitignore` | Specifies files Git should ignore |

## 🧪 Testing

The workflow should be tested to verify that:

- Google Sheets data is retrieved correctly.
- The email subject and body are formatted properly.
- Gmail sends the email successfully.
- Multiple spreadsheet rows are included in the email.
- An empty sheet does not result in a blank email.
- The empty-sheet logging branch works as expected.

## 🔐 Credentials & Security

Google Sheets and Gmail credentials are configured within n8n.

**No passwords, OAuth tokens, or private credentials should be committed to this repository.**

When importing the workflow into another n8n instance, configure the required credentials before execution.

## 🚀 How to Use

1. Download `CAIE Course Program.json` from this repository.
2. Open your n8n instance.
3. Import the workflow JSON file.
4. Configure your Google Sheets and Gmail credentials.
5. Select the appropriate Google spreadsheet and worksheet.
6. Set the recipient email address.
7. Execute the workflow and verify the received email.

## 🎓 Learning Outcome

This project demonstrates practical knowledge of workflow automation, Google Sheets integration, Gmail automation, conditional logic, JavaScript data formatting, error handling, and GitHub version control.

---

**Assignment:** 9 – n8n Automation: Google Sheets to Gmail  
**Program:** Social Eagle · CAIE Course Program  
**Status:** Project completed and documented
