# Markdown to Google Docs Converter

## Project Description
This Python-based tool is designed to automate the conversion of Markdown meeting notes into professionally formatted Google Documents. It utilizes the Google Docs API to handle hierarchical headings, nested bullet points, assignee mentions, and interactive checkboxes.

## Requirements
To run this project, you need:
* A Google account with access to Google Drive and Google Docs.
* The `google-api-python-client` library.
* The `google-auth-oauthlib` library.

## Setup Instructions
1.  **Repository**: Clone this repository or download the `.ipynb` notebook.
2.  **Environment**: Open the notebook in [Google Colab](https://colab.research.google.com/).
3.  **Dependencies**: Run the installation cell:
    `!pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib`

## How to Run in Colab
1.  **Authentication**: Execute the authentication cell. A browser pop-up will appear; log in with your Google credentials to grant the script permission to create documents.
2.  **Input Data**: Provide the Markdown content in the `markdown_content` string variable.
3.  **Execution**: Call the `convert_markdown_to_google_doc` function.
4.  **Output**: The script will print a direct link to the newly created and formatted Google Doc.

## Code Features
* [cite_start]**API Integration**: Programmatic creation and batch updating of Google Docs[cite: 12].
* [cite_start]**Automatic Formatting**: Converts `#` to H1, `##` to H2, and `###` to H3 styles[cite: 14, 15, 16].
* [cite_start]**Interactive Elements**: Transforms `- [ ]` into functional Google Doc checkboxes[cite: 18].
* [cite_start]**Mention Styling**: Automatically bolds and colors `@name` mentions for visibility[cite: 19].
