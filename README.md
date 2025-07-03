## Project: PDF Annotator Application

### Problem Statement:

The goal of this project is to build a React-based PDF annotator that allows a user to upload a PDF file, highlight any selected text in the document, and have those highlights saved for later viewing. When the same PDF is opened again in the app, the previously highlighted sections should be automatically re-rendered as highlighted.

---

### Objective:

You are required to build a React application that provides the following functionality:

1. **Upload and view a PDF document**
   The user should be able to upload any PDF file from their local machine and view it in the browser. The viewer should support basic features such as page navigation and zoom.

2. **Highlight selected text**
   The user should be able to select and highlight any portion of text in the PDF. This should work across multiple pages.

3. **Save highlight metadata**
   The application should save the metadata related to each highlight. This may include the page number, the selected text, the bounding box or position of the highlight, and any other information necessary to re-render the highlight later. You are free to choose the data structure and format (e.g., JSON), as well as how and where this data is stored (e.g., localStorage, IndexedDB, or a backend if you wish to add one).

4. **Restore highlights on file reopen**
   When the user uploads the same PDF again, the application should detect this (using filename, checksum, or any identifier you decide) and automatically render the previously saved highlights on the correct pages and positions.

You may consider using libraries such as `pdfjs-dist` (for rendering the PDF), `react-pdf` (for integration in React), or `pdf-lib` (for working with PDF coordinates and text content). These are suggestions only — you are free to explore and choose other libraries if they better suit your implementation.

---

### Requirements:

* Use React for the application.
* Maintain highlight persistence across sessions for each unique PDF.
* Ensure that highlights appear only on the correct PDF and in the correct positions.
* Provide a clean and usable interface for viewing and highlighting PDFs.
* Metadata storage should be reliable and efficient — choose an appropriate strategy based on your app architecture.

---

### Deliverables:

* A fully working React application with:

  * PDF upload and viewing capability
  * Text selection and highlighting
  * Persistent and restorable highlight metadata
* A README that explains:

  * The overall structure and approach of your solution
  * How to run the project locally
  * Any additional notes (e.g., decisions made, edge cases handled, limitations)

---

### Success Criteria:

* The app functions reliably for multiple PDFs.
* Highlights persist across reloads and accurately reappear on re-opening the same document.
* The codebase is organized and understandable.
* UI is responsive and intuitive.

---

You are encouraged to make your own decisions around UX, highlight logic, data format, and storage strategy. Treat this as a real-world scenario where you're solving a problem end-to-end.
