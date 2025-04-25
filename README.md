# Job Application Agents

A Python-based autonomous agent system that automates and optimizes the job application process using CrewAI. This project demonstrates how multiple specialized agents can collaborate to analyze job postings, tailor resumes, and prepare candidates for interviews.

## 🚀 Features

- **Multi-Agent Job Application Pipeline**: Four specialized agents work together to optimize your job application.
- **Automated Job Analysis**: Extracts and analyzes key requirements from job postings.
- **Smart Profile Building**: Synthesizes information from GitHub, personal write-ups, and other sources.
- **Resume Tailoring**: Automatically adapts resumes to match job requirements.
- **Interview Preparation**: Generates relevant questions and talking points.
- **Environment Configurable**: API keys and settings via `utils.py` or environment variables.

## 🧩 Main Agents

- **Tech Job Researcher**: Analyzes job postings to extract key requirements and qualifications.
- **Personal Profiler**: Builds comprehensive candidate profiles from various sources.
- **Resume Strategist**: Tailors resumes to highlight relevant skills and experiences.
- **Interview Preparer**: Creates interview questions and talking points based on the job and candidate profile.

## 🏗️ How It Works

1. **Setup**: Configure your API keys in `utils.py` or as environment variables.
2. **Run the App**: Execute `main.py` to start the agent workflow.
3. **Agent Collaboration**: Agents analyze the job, build your profile, tailor your resume, and prepare interview materials.
4. **Output**: Produces a tailored resume (`tailored_resume.md`) and interview preparation materials (`interview_materials.md`).

## 📦 Installation

```bash
git clone <repo-url>
cd job-application-agents
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## ⚙️ Usage

1. Set up your API keys in `utils.py` or as environment variables.
2. Prepare your initial resume in `fake_resume.md`.
3. Run the main script:
   ```bash
   python main.py
   ```
4. Edit job inputs in `main.py` to customize:
   - Job posting URL
   - GitHub profile URL
   - Personal write-up

## 📝 Example

```
$ python main.py
[Researcher] Analyzing job posting...
[Profiler] Building candidate profile...
[ResumeStrategist] Tailoring resume...
[InterviewPreparer] Generating interview materials...
Output: Tailored resume and interview prep materials saved to files.
```

## 🛠️ Customization

- Add new agents for additional job application tasks.
- Modify agent logic to match specific industry requirements.
- Integrate with additional job boards or professional networks.
- Customize resume and interview prep output formats.

## 📚 Dependencies

- Python 3.8+
- CrewAI
- crewai_tools (FileReadTool, ScrapeWebsiteTool, MDXSearchTool, SerperDevTool)
- Other packages in `requirements.txt`

## 🤝 Contributing

Pull requests are welcome! For major changes, open an issue first to discuss what you want to change.

---
Feel free to modify or extend the agents for your own job application automation needs!
