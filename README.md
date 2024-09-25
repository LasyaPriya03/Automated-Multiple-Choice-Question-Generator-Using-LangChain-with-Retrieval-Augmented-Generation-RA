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

2. **Set up a virtual environment**:
''' python3 -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

