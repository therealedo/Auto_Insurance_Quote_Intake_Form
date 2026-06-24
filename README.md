# Acosta Insurance Group - Intake Form

A modern, fast, and fully client-side **Auto Insurance Quote Intake Form** built for Acosta Insurance Group. This tool helps clients input driver and vehicle information, upload necessary documents (like driver licenses and vehicle registrations), and compile everything into a ready-to-send package (PDF/ZIP) for their insurance agent.

## Features

- 🌐 **Bilingual Interface**: Support for both Spanish (default) and English with instant language toggling.
- 🚗 **Multi-Driver & Multi-Vehicle Support**: Add or remove multiple drivers and vehicles dynamically.
- 📁 **Document Uploads**: Attach photos or PDFs of driver's licenses, vehicle registrations, and existing declaration pages directly.
- 🔒 **Privacy-First (Client-Side Processing)**: All text compiling, PDF formatting, and ZIP file bundling happen entirely inside the browser. No data is sent to a backend server.
- 📄 **Automated PDF & ZIP Packaging**: 
  - Compiles manual input into a professional PDF summary using `jsPDF` and `jsPDF-autotable`.
  - Bundles the PDF summary along with all uploaded files into a single `.zip` file using `JSZip` and `FileSaver.js`.

## Tech Stack

- **Frontend**: HTML5, Vanilla JavaScript, and Tailwind CSS (via CDN).
- **Libraries**:
  - [jsPDF](https://github.com/parallax/jsPDF) for client-side PDF generation.
  - [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable) for structured PDF tables.
  - [JSZip](https://stuk.github.io/jszip/) for client-side file compression.
  - [FileSaver.js](https://github.com/eligrey/FileSaver.js/) for saving files locally.

## Getting Started

1. Clone or download this repository.
2. Open `acosta_insurance_intake_form.html` in any web browser.
3. Fill out the form, add any uploads, and click **Generar Paquete de Cotización (PDF/ZIP)** to save the bundle.

---

## How to Set Up and Push to GitHub

Here are the step-by-step instructions to push this project to a new repository on GitHub:

### 1. Initialize Git and Commit Files Locally
Run these commands in your project folder:
```bash
# Initialize the repository
git init -b main

# Add files to tracking
git add .

# Create the initial commit
git commit -m "Initial commit: Acosta Insurance Intake Form website"
```

### 2. Create a Repository on GitHub
1. Go to [GitHub](https://github.com/) and log in.
2. Click the **New** button (or go to `https://github.com/new`).
3. Set the repository name (e.g., `Auto_Insurance_Quote_Intake_Form`).
4. Keep it **Public** or **Private** as you prefer.
5. **Do not** check "Add a README file", "Add .gitignore", or "Choose a license" (we already have our own).
6. Click **Create repository**.

### 3. Link Local Repository and Push
On your terminal, copy the commands from your new GitHub repository's "or push an existing repository from the command line" section:
```bash
# Replace <username> and <repository-name> with yours:
git remote add origin https://github.com/<username>/<repository-name>.git

# Push your code to GitHub
git push -u origin main
```
