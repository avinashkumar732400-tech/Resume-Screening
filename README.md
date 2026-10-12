# AI-Powered Resume Screening System 🤖

## About the Project

I built this project to make the resume screening process easier with the help of AI. Manually checking multiple resumes against a job description can take a lot of time, so I wanted to create a system that can automate the initial screening process.

This project uses Python and the Groq API to analyze job descriptions, extract important information from resumes, and calculate how closely a candidate's profile matches the job requirements.

## What Can It Do?

- Analyze job descriptions and identify the required skills, qualifications, and responsibilities.
- Extract candidate details, skills, education, projects, and experience from PDF and DOCX resumes.
- Compare resumes with job requirements using an LLM.
- Generate a matching score for each candidate.
- Rank candidates based on their matching scores.
- Display the top and lowest-scoring candidates.

## Technologies I Used

- Python
- Groq API
- Large Language Models (LLMs)
- Pydantic
- PyPDF
- python-docx
- python-dotenv

## How It Works

1. I provide a job description to the system.
2. The AI extracts the important job requirements.
3. The system reads resumes from the `resumes` folder.
4. Each resume is analyzed and converted into structured information.
5. The AI compares each candidate's profile with the job requirements.
6. The system generates matching scores and ranks the candidates.

## Getting Started

**1. Clone the repository**

```bash
git clone <your-repository-url>
cd Resume-Screening-System
```

**2. Install the required libraries**

```bash
pip install groq python-dotenv pydantic pypdf python-docx
```

**3. Set up your API key**

Create a `.env` file in the project folder and add your Groq API key:

```env
GROQ_API_KEY=your_groq_api_key
```

**4. Add resumes**

Create a folder named `resumes` and place the candidate resumes inside it. The system supports PDF and DOCX files.

**5. Run the project**

```bash
python main.py
```

## What I Learned

While building this project, I gained practical experience working with LLM APIs, extracting structured data using Pydantic, processing PDF and DOCX files, writing prompts for AI-based analysis, and comparing information using Python.

## Future Improvements

I plan to improve this project by adding a Streamlit interface, allowing users to upload resumes directly, and providing downloadable candidate reports.

## Note

The matching score is an AI-generated estimate, not a final hiring decision. Recruiters should review candidates fairly and verify the results before making decisions.

---

**If you find this project useful, feel free to explore the repository!**
