# MergeMark

## Overview

MergeMark is a web application that allows users to combine multiple text (.txt) or markdown (.md) files into a single document for easy reading, organization, and export. It provides a streamlined interface for uploading, arranging, and exporting document collections.

## Features

- **File Upload**: Upload multiple text or markdown files via file selector or drag-and-drop interface
- **Content Preview**: View formatted content with proper markdown rendering
- **Document Organization**: Drag and reorder document sections to customize the sequence
- **Multiple Export Options**:
  - Print document with full formatting
  - Generate text-only PDF
  - Export as combined HTML (with CSS styling preserved)
  - Export as combined markdown
- **Dark Mode Support**: Toggle between light and dark interface themes
- **Responsive Design**: Works on desktop and mobile devices
- **Image Support**: Displays and processes images in markdown files
- **User Notifications**: Toast notifications for operation feedback

## Technical Implementation

### Frontend Components

- **HTML/CSS/JavaScript**: Pure frontend implementation with no backend requirements
- **Libraries**:
  - Marked.js for markdown parsing
  - jsPDF for PDF generation
  - html2canvas for canvas-based captures
  - Font Awesome for icons

### CSS Architecture

- Comprehensive CSS with variables for theming
- Responsive design using media queries
- Dark mode implementation
- Print-specific styling

### JavaScript Features

- Asynchronous file processing
- Drag-and-drop API implementation
- Error handling with user feedback
- Image processing (converts to base64 for portability)
- Dialog management for modals
- LocalStorage for theme preference persistence

## Current Status

The application is fully functional with a clean, responsive interface. Recent updates include:

- Merged CSS from separate files into a single comprehensive stylesheet
- Enhanced error handling and user feedback
- Improved file handling with asynchronous processing
- Support for image embedding in exported HTML
- Implementation of toast notifications
- Dark mode toggle with persistent preferences
- Back-to-top button for better navigation
- Improved drag-and-drop experience

## Planned Improvements

- Enhanced PDF generation with better image support
- Additional export format options
- Save/load document collections
- Cloud storage integration

## Usage

1. **Upload Files**: Click "Select Files" or drag & drop files onto the dropzone
2. **Reorder Content**: Drag sections in the list to change their order
3. **Remove Content**: Delete individual sections as needed
4. **Export**: Choose from multiple export options based on your needs

## Browser Compatibility

MergeMark works in all modern browsers (Chrome, Firefox, Safari, Edge). It uses standard web APIs and should maintain compatibility across updates.