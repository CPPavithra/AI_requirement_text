# AI_requirement_text

Run this on Google COLAB. Google Colab inherently provides us with a UI for displaying the code. I am using that.
Use this link. 
It is active for 72 hours only. Starting from 1/04/2025 23:40
[!] https://f42eb22935d116fc1e.gradio.live


## Tech Stack and Frameworks Used

This AI-powered Requirement Extraction System is built using the following technologies and frameworks:

**1. Core Programming Language:**

* **Python:** The primary language used for the entire application development.

**2. User Interface Framework:**

* **Gradio:**
    * **Purpose:** Used to create the interactive web user interface for easy interaction with the requirement extraction functionalities.
    * **Key Features Used:**
        * `gr.Blocks`: For structuring the UI layout.
        * `gr.Markdown`: For displaying formatted text (title, description).
        * `gr.Row`: For arranging components horizontally.
        * `gr.File`: For handling file uploads.
        * `gr.Textbox`: For displaying the processing status.
        * `.upload()`: To trigger the processing function upon file upload.

**3. File Processing Libraries:**

* **`pdfplumber`:** Used for extracting text content from PDF (`.pdf`) files.
* **`python-docx`:** Used for creating and manipulating Microsoft Word (`.docx`) files (for generating the requirements document).
* **`openpyxl`:** Used for working with Excel (`.xlsx`) files (for generating the user stories spreadsheet).
* **`email` (Python Standard Library):** Used for parsing and extracting content from email (`.eml`) files.

**4. Data Manipulation Library:**

* **`pandas`:** Used for creating and managing structured data (DataFrames) for generating the user stories in Excel format.

**5. External Connectivity (for Public Access in Development):**

* **`pyngrok`:** A Python wrapper for `ngrok`, used to create secure public URLs for the locally running Gradio interface (primarily for development and sharing in environments like Google Colab).

**6. Standard Python Libraries:**

* **`os`:** Used for interacting with the operating system, such as handling file paths and removing temporary files.

**Summary:**

The system leverages Python as its core language, utilizing Gradio for the user interface, specialized libraries for processing various document formats (`pdfplumber`, `python-docx`, `openpyxl`, `email`), and `pandas` for data structuring. `pyngrok` is employed during development in environments like Google Colab to provide public accessibility for testing and sharing.
