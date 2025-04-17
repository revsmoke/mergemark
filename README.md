# MergeMark

![MergeMark Logo](mergemark_logo.svg)

## Introduction

MergeMark is a powerful web application that simplifies document management by combining multiple text (.txt) or markdown (.md) files into a single, cohesive document. Perfect for project documentation, research notes, content compilation, and more, MergeMark enables seamless organization and export of your text-based content.

**Key Benefits:**
- No installation required - runs in your browser
- No data leaves your computer - 100% client-side processing
- Intuitive interface with drag-and-drop support
- Multiple export options to suit your needs
- Dark mode support for comfortable viewing

## Description

MergeMark processes uploaded files in real-time, displaying markdown content with proper rendering and plain text content with clear formatting. Each file becomes a distinct section in the combined document view, which can be easily rearranged through a user-friendly interface.

The application provides comprehensive tools to manage your combined document:

* **Uploading:** Select files through a file picker or simply drag and drop them onto the designated area.
* **Reordering:** Change the order of file sections using an intuitive drag-and-drop interface.
* **Deletion:** Remove individual sections (files) from the combined view as needed.
* **Output Options:**
  * **Print Document:** Use your browser's built-in print functionality to print or save as PDF with full formatting.
  * **Generate PDF (Text Only):** Create a downloadable PDF containing the plain text content.
  * **Export Combined HTML:** Save the entire document as a standalone HTML file with styling preserved.
  * **Export Combined Markdown:** Export all content as a single markdown file for further editing.

## Features

* Support for `.txt` and `.md` file formats
* Advanced drag-and-drop file input with visual feedback
* Real-time preview of rendered Markdown content
* Image support for markdown files (displayed in preview and preserved in HTML export)
* Intuitive drag-and-drop reordering of document sections
* One-click deletion of individual sections
* Four export options (Print, PDF, HTML, Markdown)
* Dark mode toggle with preference saving
* Toast notifications for user feedback
* Confirmation modals for critical actions
* Responsive design for desktop and mobile use
* Back-to-top navigation for long documents

## Technology Stack

* **Frontend:** HTML5, CSS3, Vanilla JavaScript
* **Libraries:**
  * [marked.js](https://marked.js.org/): For parsing and rendering Markdown
  * [jsPDF](https://github.com/parallax/jsPDF): For generating PDFs client-side
  * [html2canvas](https://html2canvas.hertzen.com/): For canvas-based captures
  * [Font Awesome](https://fontawesome.com/): For iconography

## How to Use

1. Open `mergemark.html` in your web browser
2. Click "Select Files" or drag and drop `.txt` or `.md` files onto the designated area
3. View the combined content with proper markdown rendering
4. Use the "Document Sections" list to drag and drop sections into your desired order
5. Click the arrow button next to any section to quickly navigate to it in the preview
6. Click the trash button next to any section to remove it
7. Use the export options at the bottom of the controls panel:
   - "Print Document" for browser's print/save-to-PDF feature (preserves formatting)
   - "Generate PDF (Text Only)" for a downloadable text-only PDF
   - "Export Combined HTML" for a standalone HTML file
   - "Export Combined Markdown" for a single markdown file
8. Toggle dark mode using the moon/sun icon in the navigation bar
9. Click "Clear All" to remove all loaded files and start over

## Development Roadmap

### Completed Enhancements
* ✅ Dark mode implementation with preference saving
* ✅ Enhanced export options (HTML and Markdown)
* ✅ Image support in preview and HTML export
* ✅ Improved UI with toast notifications
* ✅ Back-to-top navigation

### Current Priorities
* **Enhance PDF Generation:** Improve the PDF export to better handle markdown formatting and images
* **Local Persistence:** Save document state to localStorage to prevent work loss
* **Batch Processing:** Optimize handling of larger document collections

### Future Goals
* **Customizable Themes:** Allow users to personalize the interface beyond dark/light mode
* **Section Editing:** In-app editing of document sections
* **Cloud Integration:** Optional connectivity with cloud storage services
* **Collaborative Features:** Real-time collaboration capabilities
* **Syntax Highlighting:** Enhanced code block display in markdown sections
* **Advanced Image Handling:** Better control over image placement and sizing
* **Accessibility Improvements:** Ensure full compliance with accessibility standards

## Contributing

Contributions to MergeMark are welcome! Whether you're fixing bugs, improving the documentation, or proposing new features, your help is appreciated.

## License

[MIT License](LICENSE)