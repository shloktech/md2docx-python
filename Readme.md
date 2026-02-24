# Word to Markdown and Markdown to Word Converter 

## Overview

Simple and straight forward Python utility that converts Microsoft Word documents (`.docx`) to Markdown files (`.md`) and vice versa. It supports multiple Markdown elements, including headings, bold and italic text, both unordered and ordered lists, and many more.

## Word to Markdown Conversion Example:
#### Input .docx file:
![image](https://github.com/user-attachments/assets/2891ebdf-ff36-4fd5-af2f-b35413264b06)

#### Output .md file:
![image](https://github.com/user-attachments/assets/e46c096b-762e-4f0c-a0ab-f81c3069a533)


## Markdown to Word Conversion Example:
#### Input .md file:
![image](https://github.com/user-attachments/assets/c2325e52-05a7-4e11-8f28-4eeb3d8c06f5)

#### Output .docx file:
![image](https://github.com/user-attachments/assets/3e48a9dd-8fe3-43cc-8246-164c58e95179)


## Features

- Bi-directional conversion between Markdown and Word documents
- Handles various programming languages code given in word doc like python, ruby and more.
- Converts Markdown headers (`#`, `##`, `###`) to Word document headings and back
- Supports bold and italic text formatting
- Converts unordered (`*`, `-`) and ordered (`1.`, `2.`) lists
- Handles paragraphs with mixed content
- Preserves document structure during conversion

## Prerequisites

You need to have Python installed on your system along with the following libraries:

- `markdown` for converting Markdown to HTML
- `python-docx` for creating and editing Word documents
- `beautifulsoup4` for parsing HTML
- `mammoth` for converting Word to HTML

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

#### For Converting Word to Markdown
Use the `word_to_markdown()` function to convert your Word document to Markdown:

```python
word_to_markdown(word_file, markdown_file)
```

- `word_file`: The path to the Word document you want to convert
- `markdown_file`: The desired path and name for the output Markdown file


Here's a complete example:

```python
from md2docx_python.src.docx2md_python import word_to_markdown

# Define the paths to your files
word_file = "sample_files/test_document.docx"
markdown_file = "sample_files/test_document_output.md"

# Convert the Word document to a Markdown file
word_to_markdown(word_file, markdown_file)
```

This code will create a file named `test_document_output.md`, which is the conversion of `test_document.docx` to the Markdown format.

---

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

### 9. **Bi-directional Conversion**
   - **Complete Workflow**: Convert documents in both directions, allowing for round-trip document processing
   - **Format Preservation**: Maintains formatting and structure when converting between formats
   - **Flexibility**: Easily switch between Markdown and Word formats based on your needs


### 10. **Handles Code Blocks in Word or Markdown**
   - If you have code written in Word or Markdown, this utility seamlessly handles it.
   - **For Word**: Code blocks written in Word will be converted and added in proper code formatting for Markdown.
   - **For Markdown**: Code blocks written in Markdown will be formatted and integrated neatly into Word documents.
   - Refer to the images above for a visual reference.

     
### Comparison to Other Scripts
- **Feature Set**: Some scripts may lack comprehensive support for Markdown features or may not handle lists and text formatting well.
- **Performance**: Depending on the implementation, performance might vary. This script is designed to be efficient for typical Markdown files.
- **User-Friendliness**: The clear and concise code in this script may make it more user-friendly and easier to modify compared to more complex alternatives.

Overall, this script provides a balanced combination of functionality, simplicity, and ease of use, which can be advantageous for many users looking to convert Markdown files to Word documents.

For any queries please start a discussion I will be happy to answer your queries :)
