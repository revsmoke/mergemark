# MergeMark

MergeMark is a client-side web application designed to combine multiple text (.txt) or markdown (.md) files into a single view for easy reading, organization, and output.

## Description

Users can upload or drag-and-drop their files into the application. MergeMark processes these files, displaying markdown content rendered as HTML and plain text content within preformatted blocks. Each file becomes a distinct section in a combined document view.

The application provides tools to manage the combined document:

* **Reordering:** Users can easily change the order of the file sections using a drag-and-drop interface.
* **Deletion:** Individual sections (files) can be removed from the combined view.
* **Output Options:**
  * **Print Document:** Leverages the browser's built-in print functionality, allowing users to print the combined document or save it as a PDF while preserving the on-screen formatting (including rendered markdown styles).
  * **Generate PDF (Text Only):** Creates a downloadable PDF containing only the plain text extracted from the source files. This option prioritizes content extraction over visual formatting and does not retain markdown styles.

## Features

* Supports `.txt` and `.md` file uploads.
* Drag-and-drop file input.
* Live preview of rendered Markdown content.
* Displays plain text content clearly.
* Intuitive drag-and-drop reordering of document sections.
* Ability to delete individual sections.
* Browser-native printing/saving as PDF (preserves formatting).
* Direct generation of a text-only PDF.
* Confirmation modals for critical actions (delete, clear all).
* Responsive design elements.

## Technology Stack

* **Frontend:** HTML5, CSS3, Vanilla JavaScript
* **Libraries:**
  * [marked.js](https://marked.js.org/): For parsing and rendering Markdown.
  * [jsPDF](https://github.com/parallax/jsPDF): For generating the text-only PDF client-side.

## How to Use

1. Open `mergemark.html` in your web browser.
2. Click "Select Files" or drag and drop `.txt` or `.md` files onto the designated area.
3. View the combined content. Markdown files will be rendered.
4. (Optional) Use the "Document Sections" list to drag and drop sections into your desired order.
5. (Optional) Click the "Delete" button next to any section to remove it.
6. Click "Print Document" to use your browser's print/save-to-PDF feature (preserves formatting).
7. Click "Generate PDF (Text Only)" to download a PDF containing only the plain text content.
8. Click "Clear All" to remove all loaded files and start over.

## Development Goals & Potential Enhancements

* **[High Priority] Preserve Formatting in Generated PDF:** Modify the "Generate PDF" function (potentially using jsPDF's `html()` method or exploring other libraries/approaches) to create a PDF that accurately reflects the on-screen rendered markdown formatting (styles, lists, etc.).
* **Implement Contact Form:** Add functionality to the contact modal (currently a placeholder) to allow users to send messages (would likely require a backend component).
* **More Export Options:**
  * Export as a single combined HTML file.
  * Export as a single combined Markdown file.
* **Syntax Highlighting:** Add syntax highlighting for code blocks within markdown sections, both in the preview and potentially in the formatted PDF output.
* **User Themes/Styling:** Allow customization of the visual appearance.
* **Local Persistence:** Use `localStorage` to save the current file list and order, allowing users to close and reopen the browser without losing their work.
* **Enhanced Error Handling:** Provide more specific feedback if files fail to load or parse.
* **Image Handling:** Add support for images embedded in Markdown (consider challenges for PDF generation).
* **Backend Processing Option:** For very large files or complex PDF generation tasks, consider adding an optional backend component (e.g., using Node.js or ColdFusion) to handle processing.
* **Unit/Integration Tests:** Develop a test suite to ensure reliability.
