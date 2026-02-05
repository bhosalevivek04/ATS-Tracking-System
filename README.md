# Smart ATS: AI-Powered Resume Optimization System 🚀

**Smart ATS** is a sophisticated resume analysis tool designed to help job seekers bridge the gap between their resumes and modern Applicant Tracking Systems (ATS). By leveraging the power of **Google Gemini Pro (LLM)**, this application provides data-driven insights, keyword gap analysis, and personalized suggestions to increase your chances of landing an interview.

---

## 🌟 Features

*   **Resume-JD Matching:** Calculates a percentage score indicating how well your resume aligns with a specific job description.
*   **Keyword Gap Analysis:** Automatically identifies critical skills and industry-specific keywords missing from your profile.
*   **AI-Generated Profile Summaries:** Provides professional, high-impact summary suggestions to make your resume stand out.
*   **PDF Parsing:** Seamlessly extracts text from PDF resumes for instant analysis.
*   **Intuitive UI:** A clean, Streamlit-powered interface for a smooth user experience.

---

## 🛠️ Technologies Used

*   **Language:** [Python 3.7+](https://www.python.org/)
*   **LLM Engine:** [Google Generative AI (Gemini Pro)](https://ai.google.dev/)
*   **Web Framework:** [Streamlit](https://streamlit.io/)
*   **PDF Processing:** [PyPDF2](https://pypi.org/project/PyPDF2/)
*   **Environment Management:** [python-dotenv](https://pypi.org/project/python-dotenv/)

---

## 📋 Prerequisites

Before you begin, ensure you have the following:

1.  A **Google Cloud API Key**. You can obtain one from the [Google AI Studio (Makersuite)](https://aistudio.google.com/).
2.  Python installed on your local machine.

---

## 🚀 Installation & Setup

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/bhosalevivek04/ATS-Tracking-System.git
    cd ATS-Tracking-System
    ```

2.  **Create a Virtual Environment:**
    ```bash
    # Windows
    python -m venv venv
    .\venv\Scripts\activate

    # macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install Dependencies:**
    ```bash
    pip install -r requirement.txt
    ```

4.  **Configure Environment Variables:**
    Create a `.env` file in the root directory and add your Google API Key:
    ```env
    GOOGLE_API_KEY=your_api_key_here_xxxxxx
    ```

---

## 💻 Usage

1.  **Launch the Application:**
    ```bash
    streamlit run app.py
    ```

2.  **Analyze Your Resume:**
    *   **Step 1:** Paste the target **Job Description** into the provided text area.
    *   **Step 2:** Upload your resume in **PDF format**.
    *   **Step 3:** Click the **Submit** button.

3.  **Review Results:**
    The system will return a structured JSON response containing:
    *   `JD Match`: Percentage of compatibility.
    *   `MissingKeywords`: List of skills to add.
    *   `Profile Summary`: Professional improvement suggestions.

### Example Output
```json
{
  "JD Match": "85%",
  "MissingKeywords": ["Cloud Computing", "Big Data Analytics", "Agile Development"],
  "Profile Summary": "Experienced software engineer with a strong foundation in..."
}
```

---

## 📂 Project Structure

```text
ATS-Tracking-System/
├── app.py              # Main Streamlit application logic
├── .env                # API keys and secrets (ignored by git)
├── requirement.txt     # Project dependencies
├── README.md           # Project documentation
└── ...
```

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information. *(Note: Please add a LICENSE file to the repository to finalize this).*

---

## 📧 Contact

**Project Link:** [https://github.com/bhosalevivek04/ATS-Tracking-System](https://github.com/bhosalevivek04/ATS-Tracking-System)

*Developed with ❤️ using Google Gemini and Streamlit.*