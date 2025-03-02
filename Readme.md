# Markdown to Word Converter 

## Overview

Simple and straight forward Python utility that converts a Markdown file (`.md`) to a Microsoft Word document (`.docx`). It supports multiple Markdown elements, including headings, bold and italic text, both unordered and ordered lists, and many more.

#### Input .md file:
![image](https://github.com/user-attachments/assets/c2325e52-05a7-4e11-8f28-4eeb3d8c06f5)

#### Output .docx file:
![image](https://github.com/user-attachments/assets/3e48a9dd-8fe3-43cc-8246-164c58e95179)

## Word to Markdown Conversion Example:
#### Input .docx file:
![image](https://github.com/user-attachments/assets/2891ebdf-ff36-4fd5-af2f-b35413264b06)

#### Output .md file:
![image](https://github.com/user-attachments/assets/e46c096b-762e-4f0c-a0ab-f81c3069a533)



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

Sure, let's enhance your instructions for clarity and completeness:

---

### How to Convert Markdown to Word Using `md2docx-python`

#### Step 1: Install the Required Library
First, you need to install the `md2docx-python` library using pip. Open your terminal and run the following command:

```bash
pip install md2docx-python
```

#### Step 2: Import the Library in Your Code
To use the library, import it into your Python code with the following line:

```python
from md2docx_python.src.md2docx_python import markdown_to_word
```

#### Step 3: Convert Markdown to Word
Call the `markdown_to_word()` function to convert your Markdown file to a Word document. Here's the syntax:

```python
markdown_to_word(markdown_file, word_file)
```

- `markdown_file`: The path to the Markdown file you want to convert.
- `word_file`: The desired path and name for the output Word document.

#### Step 4: Sample Code
Here's a complete example to illustrate how it works:

```python
from md2docx_python.src.md2docx_python import markdown_to_word

# Define the paths to your files
markdown_file = "sample_files/amazon_case_study.md"
word_file = "sample_files/amazon_case_study.docx"

# Convert the Markdown file to a Word document
markdown_to_word(markdown_file, word_file)
```

This code will create a file named `amazon_case_study.docx`, which is the conversion of `amazon_case_study.md` to the Word format.

---

This should make it easier to understand and follow the steps. Let me know if you need any more help or further enhancements!

## Why this repo and not others ?

Here are some reasons why this repo might be considered better or more suitable for certain use cases compared to other scripts available on the internet:

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

### 8. **Privacy**
   - If you are working in a corporate firm and you want to convert your markdown files to word and you use a online tool to do it then there are chances that they will store your file which can cause to a vital information leak of your company. With use of this repo you can easily do the conversion in your own system.

### Comparison to Other Scripts
- **Feature Set**: Some scripts may lack comprehensive support for Markdown features or may not handle lists and text formatting well.
- **Performance**: Depending on the implementation, performance might vary. This script is designed to be efficient for typical Markdown files.
- **User-Friendliness**: The clear and concise code in this script may make it more user-friendly and easier to modify compared to more complex alternatives.

Overall, this script provides a balanced combination of functionality, simplicity, and ease of use, which can be advantageous for many users looking to convert Markdown files to Word documents.

For any queries please start a discussion I will be happy to answer your queries :)
