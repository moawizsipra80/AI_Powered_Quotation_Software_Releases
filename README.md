# AI-Powered-Quotation-Software-Releases


## Overview
This is a professional Quotation management software designed to streamline the process of generating financial documents and managing client relationships. It includes a modern dashboard, comprehensive document generation tools, and integrated marketing bots.

## Features
- **Document Generation**: Easily create and export:
  - Quotations
  - Tax Invoices
  - Commercial Invoices
  - Delivery Challans (with auto-generated signature notes)
- **Dashboard & Analytics**: 
  - Real-time sales performance graphs.
  - Monthly sales summaries.
  - Recent activity tracking.
- **Client Management**:
  - Detailed client history and ledgers.
  - Quick access to client summaries.
- **Marketing Automation**:
  - **WhatsApp Bot**: Send bulk messages with attachments for marketing campaigns.
  - **Instagram Lead Miner**: Automated DM bot to reach potential clients.
- **Security & User Management**:
  - Secure Login System with "Remember Me" functionality.
  - **Enhanced**: Full-screen login and setup interface.
  - **New**: Profile picture upload for user accounts.
  - Password recovery via security question.
  - Role-based access (Admin/User).
- **Customization**:
  - Custom header/footer and logo alignment.
- **PDF Generation**: High-quality PDF output using ReportLab.
- **Offline AI assistant** : An offline ai assistant.Your personal ai assistant to assist you. You can ask anything from that like gpt and grmini.
- **AI Agent**:An ai agent that simply takes command from you and a sample template and items (either you give hand written or printed document or write manually ) and then takes a sample of that doocument you want to generate and then analyze it's format and at the end generate it.
- **Invite team**:You can invite a team and give access to your team mates 
  
## Technology Used:-

### 1. User Interface (UI) & Theme Styling

* **tkinter** – Builds the desktop graphical user interface (GUI), including windows, buttons, input fields, canvas grids, and scrollable frames.
* **ttkbootstrap** – Applies modern themes and styling to `tkinter` widgets, replacing the default appearance with a clean, professional design.
* **Pillow (PIL)** – Loads, resizes, crops, and processes images (PNG, JPG, ICO) for logos, icons, and document headers.

### 2. Document Generation & Export

* **reportlab** – Generates professionally formatted PDF documents such as Quotations, Invoices, and Delivery Challans.
* **python-docx** – Creates and exports Microsoft Word (`.docx`) documents.
* **openpyxl** – Generates and formats Microsoft Excel (`.xlsx`) spreadsheets.

### 3. Database, Networking & Utilities

* **sqlite3** – Stores and manages application data locally using SQLite databases.
* **requests** – Sends HTTP requests, such as communicating with local Ollama AI endpoints.
* **json** – Reads and writes structured JSON data for settings, configurations, and AI responses.
* **re** – Performs regular expression (regex) operations for text parsing and data extraction.
* **qrcode** – Generates QR codes for invoices and other printable documents.

### 4. System & Process Management

* **os / sys** – Handles file paths, directories, and system-level operations.
* **shutil** – Copies and moves generated files between directories.
* **webbrowser / subprocess** – Opens document previews and executes external programs or print commands.
* **time / datetime** – Manages dates, timestamps, document creation times, and validity periods.

## How to Use
1. **Installation**: Ensure Python is installed along with the required libraries (selenium, pandas, reportlab, ttkbootstrap, etc.).
2. **Launch**: Run the `quotation.py` file to start the application.
   ```bash
   python quotation.py
   ```
3. **Setup**: On the first run, you will be prompted to set up an Admin profile.
4. **Operation**: Use the dashboard to navigate between creating quotations, invoices, and managing marketing tools.

--
<img width="1919" height="1109" alt="image" src="https://github.com/user-attachments/assets/52b448cb-1e66-4a64-8a50-73a19ebf0d48" />


<img width="1911" height="1110" alt="image" src="https://github.com/user-attachments/assets/d00768fe-3663-48f6-adb8-af9edb7b8ce2" />



<img width="1910" height="1093" alt="image" src="https://github.com/user-attachments/assets/e4f6020c-6d44-4d9f-b7c6-96e9136a48c8" />

<img width="1919" height="1133" alt="image" src="https://github.com/user-attachments/assets/cab0cf59-f36a-4502-99d2-75dfe334c91a" />


## Public Downloads While Source Stays Private
Use this repository as private source code, and publish installers to a separate public repository:

1. Create a public repository (example: `your-org/Quotation-Software-Downloads`).
2. In this private repository, add:
   - Repository variable: `PUBLIC_DOWNLOADS_REPO` = `owner/public-download-repo`
   - Repository secret: `PUBLIC_REPO_TOKEN` = GitHub PAT with `repo` access to the public downloads repository
3. Push a version tag (for example `v5.3.0`) to trigger the release workflow.
4. The workflow uploads Windows and macOS binaries to the public repository release with the same tag.
5. Use website button links in this format:
   - `https://github.com/<owner>/<public-download-repo>/releases/latest/download/QuotationGenerator_Setup_v5.2.exe`
   - `https://github.com/<owner>/<public-download-repo>/releases/latest/download/QuotationGenerator-macOS.zip`

Do not use GitHub Actions artifact URLs for end-user downloads, because they require authenticated access.

---
We will improve it further.
