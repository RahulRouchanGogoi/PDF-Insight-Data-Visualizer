# PDF Insight & Data Visualizer

PDF Insight & Data Visualizer allows users to upload a PDF document to extract text, analyze content, and generate insights on age distribution. It identifies names and ages within the text, visualizes age-group distribution through a bar chart, and provides an option to download the chart as a PDF. This tool is particularly useful for extracting demographic insights from textual data quickly and efficiently.

## Features

- **PDF Text Extraction**: Upload a PDF and extract all text, including multi-page documents.
- **Age-Group Analysis**: Automatically identifies and counts ages, grouping them into predefined age ranges.
- **Visual Representation**: Displays age distribution as an interactive bar chart.
- **Download Options**: Export the text content or download the age-distribution chart as a PDF.

## Usage

- Open the application.
- Upload a PDF file (with optional password entry for protected files).
- The page range will automatically default to "All Pages" for text extraction, displaying the full text in the textbox.
- The age distribution chart will auto-generate based on the extracted data.
- Use the "Download Chart as PDF" button to save the visualization.

## Tech Stack

- **HTML/CSS/JavaScript**: Basic web application structure.
- **pdf.js**: PDF parsing and text extraction.
- **Chart.js**: Creating visual charts for age distribution.
- **jsPDF**: Exporting chart as PDF files.

## Library Workflow

1. **pdf.js**  
   - **Role**: Responsible for parsing and extracting text from PDF files.
   - **Process**: Once the user uploads a PDF, pdf.js reads and decodes the document, page by page, extracting raw text content.
   - **Interaction**: The extracted text is then passed to the main JavaScript logic for analysis, allowing further processing.

2. **Chart.js**  
   - **Role**: Generates an interactive bar chart to visualize age-group distribution.
   - **Process**: After text extraction, JavaScript logic processes the text to identify ages, categorize them into age groups, and calculate the counts for each group. Chart.js then takes these processed data points and renders a bar chart.
   - **Interaction**: Chart.js uses the age data to create a clear, visual representation that updates dynamically as soon as text extraction completes.

3. **jsPDF**  
   - **Role**: Allows users to download the age distribution chart as a PDF.
   - **Process**: When the user clicks "Download Chart as PDF," jsPDF captures the chart as an image and adds it to a new PDF document.
   - **Interaction**: This PDF can be saved to the user’s device, providing a downloadable copy of the analyzed age distribution chart.

## Code Structure

- **index.html**: Main HTML structure for the user interface.
- **style.css**: Styling for a visually appealing and centered layout.
- **script.js**: JavaScript logic for PDF extraction, age-group counting, chart generation, and PDF export.

## Use Case and Audience

This tool is ideal for researchers, educators, and analysts working with survey results, historical documents, or any text-heavy content containing age data. Specifically, health researchers, epidemiologists, and medical professionals can leverage this tool for demographic analysis in public health. For demonstration, a sample PDF (linked below) contains imaginary data of 1,000 individuals (names and ages) who tested positive for COVID-19. The tool extracts age data, generates a visual chart to highlight affected age groups, and allows users to download the extracted text in a text format. This functionality enables healthcare providers to quickly analyze data, prioritize age-specific research, develop targeted health guidelines, and recommend immunity-boosting interventions for vulnerable groups.

Download the [Demonstration PDF](https://drive.google.com/file/d/1zmQJGDxMqPjzgfGOufWQiNdE6XQ76EmA/view?usp=drive_link).

## Screenshots

1.Interface_Upload_View ![Interface_Upload_View](https://github.com/RahulRouchanGogoi/PDF-Insight-Data-Visualizer/blob/main/Image1.png)  
   *PDF Upload Interface*

2.Text_Extraction_and_Download ![Text_Extraction_and_Download](https://github.com/RahulRouchanGogoi/PDF-Insight-Data-Visualizer/blob/main/Image2.png)  
   *Text Extraction and Download Options*

3.Age_Distribution_Chart ![Age_Distribution_Chart](https://github.com/RahulRouchanGogoi/PDF-Insight-Data-Visualizer/blob/main/Image3.png)  
   *Age Distribution Chart*

4.Chart_Saved_as_PDF ![Chart_Saved_as_PDF](https://github.com/RahulRouchanGogoi/PDF-Insight-Data-Visualizer/blob/main/Image4.png)  
   *Chart Saved as PDF*

## How It Works

1. **PDF Upload & Text Extraction**  
   - The user uploads a PDF document, and the tool uses pdf.js to read and extract text from all pages.
   - If the PDF is password-protected, the user can enter the password to unlock it for analysis.
   - The extracted text is displayed in the application, and users can download it as a text file for further use.

2. **Age Data Analysis**  
   - The tool parses the extracted text to locate names and ages. Age values are automatically grouped into predefined age ranges (e.g., 0-10, 11-20, etc.).
   - JavaScript logic handles this data grouping and counting, providing a quick view of the age distribution.

3. **Visual Representation**  
   - Based on the grouped age data, Chart.js generates a bar chart to visualize the age distribution.
   - This chart clearly shows the concentration of different age groups, making it easy to identify those with higher counts.

4. **Download Options**  
   - The generated age distribution chart can be downloaded as a PDF using jsPDF, allowing users to have a portable, visual summary of the age analysis.

## Demo

![Demo Link](https://github.com/RahulRouchanGogoi/PDF-Insight-Data-Visualizer/blob/main/PDF%20Insight%20%26%20Data%20Visualizer.gif)

![Scan to launch](https://github.com/RahulRouchanGogoi/PDF-Insight-Data-Visualizer/blob/main/QR.png)

[Click to launch](https://rahulrouchangogoi.github.io/PDF-Insight-Data-Visualizer/) 

## Links

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rahul-rouchan-gogoi-04072001r)
