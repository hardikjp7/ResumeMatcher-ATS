# ResumeMatcher-ATS [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://resume-matcher-ats.streamlit.app/)


## Overview

Smart ATS is a tool designed to enhance the efficiency of the resume review process by leveraging advanced AI capabilities. The project contains the following key files:

- **app.py**: The main application file built with Streamlit, allowing users to paste a job description, upload their resume in PDF format, and receive AI-generated feedback on resume improvement.

- **requirements.txt**: Lists the required Python packages for easy installation.

## How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/hardikjp7/ResumeMatcher-ATS
cd ResumeMatcher-ATS
```

### 2. Installation

Install the required Python packages:

```bash
pip install -r requirements.txt
```

### 3. Running the Application

Execute the following command to launch the Smart ATS application:

```bash
streamlit run app.py
```

This will open a local development server, and you can access the application in your web browser.

### 4. Usage

1. **Paste the Job Description**: Enter the job description into the provided text area.

2. **Upload Your Resume**: Upload your resume in PDF format.

3. **Submit**: Click the "Submit" button to initiate the AI-driven resume analysis.

### Note

- Ensure that your environment variables are set, including the API key required for communication with Google's Generative AI.

## Prompt Template

The application uses a specific prompt template to guide the AI in generating responses. The template includes sections for the resume text and job description, and the expected response has a structured format:

```json
{
  "JD Match": "%",
  "Missing Keywords": [],
  "Profile Summary": ""
}
```

This format provides a percentage match, a list of missing keywords, and an optional profile summary.

## Disclaimer

This project relies on Google's Generative AI, and a valid API key is required for proper functioning. Ensure that you have the necessary permissions and comply with any usage policies related to the API.

---

