# Markdown to Word Converter 

## Overview

Simple and straight forward Python script that converts a Markdown file (`.md`) to a Microsoft Word document (`.docx`). It supports basic Markdown elements, including headings, bold and italic text, and both unordered and ordered lists.


## Features

- Converts Markdown headers (`#`, `##`, `###`) to Word document headings.
- Supports bold and italic text formatting.
- Converts unordered (`*`, `-`) and ordered (`1.`, `2.`) lists.
- Handles paragraphs with mixed content.

## Prerequisites

You need to have Python installed on your system along with the following libraries:

- `markdown` for converting Markdown to HTML.
- `python-docx` for creating and editing Word documents.
- `beautifulsoup4` for parsing HTML.

You can install the required libraries using pip:

```bash
pip install markdown python-docx beautifulsoup4
```
## Why repo and not others ?

Here are some reasons why this script might be considered better or more suitable for certain use cases compared to other scripts available on the internet:

### 1. **Comprehensive Markdown Support**
   - **Header Levels**: The script supports multiple header levels (`h1`, `h2`, `h3`), which is important for properly structuring the document.
   - **Bold and Italic Text**: It handles bold (`**`) and italic (`*`) text, providing more accurate formatting in the Word document.

### 2. **Proper List Formatting**
   - **Unordered and Ordered Lists**: The script correctly formats both unordered (`*`, `-`) and ordered lists (`1.`, `2.`) in the Word document. This ensures that lists appear as expected without additional line breaks or formatting issues.

### 3. **Use of Well-Supported Libraries**
   - **Markdown to HTML Conversion**: Utilizes the `markdown` library, which is a widely used and reliable tool for converting Markdown to HTML.
   - **HTML Parsing and Word Document Creation**: Employs `BeautifulSoup` for parsing HTML and `python-docx` for creating Word documents, both of which are robust and well-maintained libraries.

### 4. **Simplicity and Readability**
   - **Clear Code Structure**: The script is designed to be straightforward and easy to understand, making it accessible for users who may want to customize or extend it.
   - **Basic Markdown Elements**: Focuses on the most commonly used Markdown elements, ensuring compatibility with a wide range of Markdown files without unnecessary complexity.

### 5. **Customizability**
   - **Easy to Modify**: Users can easily adjust the script to handle additional Markdown features or customize the output format based on their specific needs.
   - **Example Usage**: Provides a clear example of how to use the script, making it easy for users to adapt it for their own files.

### 6. **Minimal Dependencies**
   - **Lightweight and Focused**: The script relies on only a few libraries, which reduces potential conflicts and keeps the script lightweight.

### 7. **Handles Basic HTML Tags**
   - **Text Formatting**: Properly handles bold and italic text by interpreting HTML tags (`strong`, `em`), ensuring that formatting is preserved when converting to Word.

### Comparison to Other Scripts
- **Feature Set**: Some scripts may lack comprehensive support for Markdown features or may not handle lists and text formatting well.
- **Performance**: Depending on the implementation, performance might vary. This script is designed to be efficient for typical Markdown files.
- **User-Friendliness**: The clear and concise code in this script may make it more user-friendly and easier to modify compared to more complex alternatives.

Overall, this script provides a balanced combination of functionality, simplicity, and ease of use, which can be advantageous for many users looking to convert Markdown files to Word documents.

