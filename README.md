# 🏡 Find Residences RPA Project

## 📖 Project Overview
The **Find Residences** project is an RPA (Robotic Process Automation) solution developed with **UiPath Studio 2025.0.157**. This automation assists users in finding available residences (apartments, houses, etc.) for sale or rent across multiple websites. The process is triggered upon receiving a payment invoice and an email with search details.

## ⚙️ How It Works

1. **User Email Request**
   - Users send an email to **findapartaments99@outlook.com**.
   - The email should include:
     - **Search criteria**: desired location, price range, property type, etc.
     - **PDF attachment**: A payment invoice for the search service.

2. **Invoice Verification**
   - The robot monitors incoming emails.
   - For each email, it extracts and validates the attached payment invoice.
   - If the invoice is invalid, the robot replies to the user, indicating the error.

3. **Residence Search**
   - Upon successful invoice validation, the robot uses the provided search criteria to explore various real estate websites.
   - Filters applied include location, price range, number of rooms, and other preferences.

4. **Results Compilation**
   - The bot compiles the found listings into an Excel file.
   - The file includes essential information such as property address, price, contact details, and website link.

5. **Response Email**
   - The robot sends an email back to the user with the results attached.

## 🛠️ Technologies Used

- **UiPath Studio 2025.0.157**
- **Outlook Email Integration**
- **PDF Processing**
- **Web Data Extraction**
- **Excel Automation**

## 🚀 Setup & Execution

1. Clone this repository.
2. Open the project in **UiPath Studio 2025.0.157**.
3. Configure email settings for the given address.
4. Run the process and test with sample emails and invoices. More examples can be found [here](./Files/InputModel).

## 📬 Email Template Example

```plaintext
Subject: [chirie / vanzare]

[chirie/vanzare]
locatie: [Oras]
[numar] camere
pret: [numar] euro
```

## ⚠️ Important Notes

- Ensure that invoices follow the predefined format for validation.
- The robot only processes new emails from the inbox.

Happy apartment hunting! 🏡🤖

