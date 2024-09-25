# Multiple Choice Question (MCQ) Generator

This project is a web application built using **Streamlit** that generates multiple-choice questions (MCQs) from a PDF document. It leverages **LangChain**, **Google Generative AI (Gemini)**, and **PyPDFLoader** for extracting text and generating questions. Users can upload a PDF, and the app will automatically generate a set of questions based on the document's content.

## Features

- **PDF Upload**: Upload any PDF document to generate questions.
- **AI-powered Question Generation**: Uses the **Google Generative AI (Gemini)** model via LangChain to create multiple-choice questions.
- **Dynamic MCQs**: Automatically generates 2-10 MCQs for each section of the document.
- **Interactive UI**: Users can select their answers and get instant feedback on their performance.
- **Customizable**: Easily modify the code to adjust the number of questions, types of answers, and layout.

## Tech Stack

- **Python**
- **Streamlit**: Front-end interface for web-based interaction.
- **LangChain**: For handling language model prompts and output parsing.
- **Google Generative AI (Gemini)**: For generating MCQs based on PDF content.
- **PyPDFLoader**: For loading and processing PDF documents.
- **Pydantic**: For structured data validation.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/mcq-generator.git
   cd mcq-generator

## Set up a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

## Install the required packages:

```bash
pip install -r requirements.txt
```

## Set up your Google API key:

Create a `.env` file in the root directory and add your Google API key:

```makefile
GOOGLE_API_KEY=your-google-api-key
```

## Run the Streamlit app:

```bash
streamlit run app.py
```

## Usage

- **Upload a PDF**: On the web app, upload any PDF file. The app will parse the content and generate multiple-choice questions based on the text.

- **View Generated Questions**: The app will display the generated questions and possible answer options for each section of the PDF.

- **Answer the Questions**: Select the options for each question, then hit **Submit**.

- **Get Feedback**: The app will show your score along with the list of correct and incorrect answers.

## Example

Here’s a quick example of how the application works:

- **Upload PDF**: Choose a PDF file from your computer.

### Generated MCQs:

- **Question 1**: What is AI?
  - a) Artificial Intelligence
  - b) Alligator Intelligence
  - c) Alien Intervention
  - d) None of the above
  
- **Question 2**: What is the purpose of propositional logic?

- **Submit**: Once you have selected the options, click on **Submit** to see your score.

## Code Overview

- `app.py`: The main Streamlit app that handles the UI and question generation logic.
- `generate_questions`: This function takes PDF content and generates MCQs using Google Generative AI via LangChain.
- **Error Handling**: Logs errors internally while continuing execution to avoid app crashes.

## Future Improvements

- Add more customization for question generation, such as difficulty levels or question types (True/False, etc.).
- Enhance the UI to support more advanced interactions, such as providing explanations for wrong answers.
- Extend the support for multi-page PDFs and more detailed question generation.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For any issues or contributions, feel free to open an issue on the repository or reach out at:

- **Email**: kotturilasya0306@example.com
- **LinkedIn**: https://www.linkedin.com/in/lasya-priya03/
