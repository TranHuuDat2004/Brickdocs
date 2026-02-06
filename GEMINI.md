# Gemini Session Log
Date: 06/02/2026

## Summary of Work
We have completed a comprehensive update to the UniDocs application and are now initiating the "BrickDocs" project - a clone of UniDocs customized for Lego/Brick instruction manuals.

### 1. New Content Added (UniDocs)
-   **Lab Subjects**: Calculus Python, Methodology C, Computer Org Lab, Linear Algebra Python, OOP Lab, OS Lab, DSA Lab, SQL Lab.
-   **Internship Subjects**: TSNN, KTCN.
-   **English Certificates**: Aptis ESOL.
-   **Skill Review**: KNTHCM.

### 2. UI/UX Improvements (UniDocs)
-   **Responsive Design**: Adjusted sidebar breakpoints, added Responsive Preview Modal.
-   **Mobile Enhancements**: Fixed Master-Detail layout, Clickable File List.
-   **Notification Feature**: Added external link notifications.

### 3. Technical Enhancements (UniDocs)
-   **File Processing**: Scripts for DOCX to PDF and renaming files.
-   **PDF Rendering**: Integrated PDF.js.
-   **DOCX Preview**: Integrated docx-preview.

### 4. Project Cloning (BrickDocs)
-   **Initialization**: Cloned UniDocs structure to `BrickDocs`.
-   **Branding**: Renamed `Subjects` to `Sets`, `Categories` to `Brands`.
-   **Target Brands**: Lego, Qman, Keeppley, Sluban.
-   **Core Files**:
    -   `set.html` (adapted from `subject.html`).
    -   `data/brands.json` (new structure).

### 5. Data Refactoring (BrickDocs)
-   **Organization**: Switched from Theme-based (Lego City) to Set-based (e.g., 60343).
-   **New Files**: Created `data/sets/lego/60343.json` and `data/sets/lego/60312.json`.
-   **Updates**: Updated `brands.json` to map IDs like `lego/60343` directly to the new file paths.

