# Cover Letter Generator

This Python script uses Tkinter to generate customized cover letters based on a template document. Below are the fields required by the program:

## Fields:

1. **Aspiration:** Your career aspiration or goal.
2. **Role:** The specific role or position you are applying for.
3. **Company:** The name of the company you are applying to.
4. **Top Skill:** Your most prominent or relevant skill.
5. **Databases:** List of databases you are familiar with.
6. **Skills:** Relevant programming languages or technical skills.
7. **Concept:** Fundamental concepts you are proficient in.
8. **Industry:** The industry or sector you are targeting.

## Placeholders in Template (cv.docx):

Ensure that your template document (cv.docx) contains the following placeholders. The script will replace these placeholders with the user-provided information.

1. **Aspiration Placeholder:** `{Aspiration}`
2. **Role Placeholder:** `{ROLE}`
3. **Company Placeholder:** `{COMPANY}`
4. **Top Skill Placeholder:** `{TOP_SKILL}`
5. **Databases Placeholder:** `{DB}`
6. **Skills Placeholder:** `{SKILL}`
7. **Concept Placeholder:** `{CONCEPT}`
8. **Industry Placeholder:** `{INDUSTRY}`

## How It Works:

- The script reads the template document and replaces the placeholders with the user-provided information.
- The customized cover letter is saved with a filename based on the company and role, following the format: `{COMPANY}_{ROLE}_CV.docx`.

## Requirements:

- Python
- Tkinter (comes with Python)
- python-docx library (install using `pip install python-docx`)

**Note:** The placeholders in the template document must match the specified format for successful execution. Adjust the template accordingly to ensure proper functionality.

## Updating Code:

To reproduce and run the code, please make the following changes:

1. Open the script (main.py) in a text editor.

2. Locate the line where the template document is loaded:
    ```python
    doc = docx.Document('<PATH TO TEMPLATE>/cv.docx')
    ```
    Change `<PATH TO TEMPLATE>` to the actual path where your template document (cv.docx) is located.

3. Locate the line where the generated cover letter is saved:
    ```python
    doc.save('<PATH TO SAVE GENERATED COVER LETTER>'+filename)
    ```
    Change `<PATH TO SAVE GENERATED COVER LETTER>` to the desired path where you want to save the generated cover letters.

## Reference:

For a sample cover letter, please refer to [cus.docx](./cus.docx).

Sure! Here is the updated installation guide that includes instructions for installing dependencies using `requirements.txt`:

## Installation Guide:

To create a clickable application, follow these steps:

1. Create a bash script (e.g., `run_cover_letter.sh`) with the following content:
    ```bash
    #!/bin/bash
    python3 "<PATH TO SCRIPT>/cus.py"
    ```
    Change `<PATH TO SCRIPT>` to the actual path where your `cus.py` script is located.

2. Save and close the script.

3. Open a terminal and navigate to the directory where `run_cover_letter.sh` is located.

4. Make the script executable:
    ```bash
    chmod +x run_cover_letter.sh
    ```

5. Install the required dependencies using the following command:
    ```bash
    pip install -r requirements.txt
    ```
    This will ensure that the necessary libraries, such as `python-docx`, are installed.

6. You can now run the script by double-clicking on it or executing it in the terminal:
    ```bash
    ./run_cover_letter.sh
    ```

This script will launch the Cover Letter Generator application.