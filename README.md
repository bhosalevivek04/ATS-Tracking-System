**README**

## ATS Tracking System

This project utilizes the Gemini AI language model to evaluate resumes based on job descriptions and provide personalized feedback to improve ATS performance.

### Features

* Resume analysis with percentage matching
* Identification of missing keywords for enhanced ATS optimization
* Profile summary generation for resume improvement
* Integrated interface for easy resume upload and job description input

### Setup

**1. API Key**

Create a Google Account and sign in to [AI Studio](https://aistudio.google.com). Navigate to "APIs" and enable the "Generative AI" API. Obtain your API key from the "Credentials" section.

**2. Environment Variable**

Store your API key in a `.env` file at the root of the project directory:

```
GOOGLE_API_KEY="<YOUR_API_KEY>"
```

### Usage

**1. Run in Integrated Terminal:**

```
streamlit run app.py
```

**2. User Interface:**

* Paste the job description into the "Job Description" text area.
* Upload your resume in PDF format.
* Click the "Submit" button.

### Functionality

The app will process the resume and job description using Gemini AI. The response will be displayed in JSON format, including:

* **"JD Match"**: The percentage match between the resume and job description
* **"MissingKeywords"**: A list of keywords missing from the resume
* **"Profile Summary"**: A suggested profile summary for the resume

### Requirements

```
streamlit
google-generativeai
python-dotenv
PyPDF2
```

### Contributions

Contributions are welcome! Please feel free to submit pull requests or report bugs.