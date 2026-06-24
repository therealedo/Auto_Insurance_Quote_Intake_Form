# Universal Auto Insurance Quote Intake Form

A modern, fast, and fully client-side **Auto Insurance Quote Intake Form**. This tool allows insurance agencies to gather client information, request supporting documents (like driver licenses, vehicle registrations, and declaration pages), and generate a consolidated quote package (PDF or ZIP file) ready for the agent to review.

## Features

- 🌐 **Bilingual Interface**: Seamless translation support for Spanish (default) and English with instant language toggling.
- 🎨 **Custom Agency Branding**: A branding settings panel (accessible via the gear icon in the header) allows agencies to specify their own name and subtitle. Custom branding is saved locally in the browser's `localStorage` and automatically prints in the header of generated PDFs.
- 🚗 **Combined Manual & Document Inputs**: Supports entering driver and vehicle details alongside file uploads for corroboration, allowing agents to copy-paste data and verify documents in one place.
- 🔒 **Privacy-First (100% Client-Side)**: All PDF compiling, file compression, and ZIP bundling happen inside the browser. No data is transmitted to an external server.
- ✉️ **Send via Gmail Integration**: Clicking "Enviar por Gmail" downloads the package, copies a text summary of the form to the user's clipboard, and opens a new Gmail Compose tab so they can paste and drag-and-drop the attachment instantly.

## Tech Stack

- **Frontend**: HTML5, Vanilla JavaScript, and Tailwind CSS (via CDN).
- **Libraries**:
  - [jsPDF](https://github.com/parallax/jsPDF) for client-side PDF generation.
  - [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable) for rendering PDF tables.
  - [JSZip](https://stuk.github.io/jszip/) for client-side compression.
  - [FileSaver.js](https://github.com/eligrey/FileSaver.js/) for saving local files.

---

## How to Use It

### Option A: Use it Offline / Desktop App
Because the entire application is contained in a single self-contained HTML file, you can run it completely offline:
1. Clone or download this repository.
2. Locate the [insurance_intake_form.html](insurance_intake_form.html) file.
3. Double-click the file to open it in Google Chrome or any modern web browser.
4. Customize your agency details by clicking the **Gear Icon** in the top right.

### Option B: Embed It in an Existing Website
You can embed this form into your agency's website using an `iframe`. Keeping the JavaScript, styles, and markup inside a single file makes hosting and embedding extremely convenient:

1. Upload `insurance_intake_form.html` to your website's server (e.g. into a directory like `/forms/`).
2. Add the following `iframe` tag to your website's HTML code:
   ```html
   <iframe 
       src="https://yourdomain.com/forms/insurance_intake_form.html" 
       width="100%" 
       height="850px" 
       style="border: 0; border-radius: 12px; box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);"
       allow="clipboard-write">
   </iframe>
   ```
   > [!IMPORTANT]  
   > The `allow="clipboard-write"` attribute is required in the `iframe` to allow the "Send via Gmail" button to successfully copy the form summary to the client's clipboard.

---

## Collaboration & Contributing

This project is open-source and customizable! If you have suggestions for improvements, styling tweaks, or new features (such as adding more insurance options or new email templates):

- **Fork this repository** to adapt it for your specific agency's tools and layout.
- **Open an issue** to report bugs, suggest features, or request improvements.
- **Submit a pull request (PR)** with your enhancements to share them back with the community!
