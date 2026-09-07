# HormoneBench AI
### Open AI Research Infrastructure for Women's Hormonal Health

HormoneBench AI is an open-source research platform that standardizes, analyzes, and benchmarks women's hormonal health datasets through an integrated AI-powered scientific validation pipeline.

The platform enables researchers, students, and healthcare innovators to transform heterogeneous datasets into a unified benchmark, generate transparent AI predictions, explain model outputs, retrieve evidence from scientific literature, and produce downloadable research reports.

> **Disclaimer:** HormoneBench AI is a research and educational project. It is not a medical device and should not be used for diagnosis, treatment, or clinical decision-making.

---

## Key Features

- **Dataset Standardization**
  - Upload CSV datasets
  - Automatic schema mapping
  - Unified HormoneBench benchmark format
  - Missing value handling & duplicate removal
  - Automated data validation

- **Data Processing Pipeline**
  - Automated data cleaning
  - Feature preprocessing & engineering
  - Standardized benchmark generation

- **AI Risk Prediction & Explainability**
  - AI-powered hormonal health risk assessment
  - Record-level predictions, risk scoring, and confidence estimation
  - Identification of key contributing factors
  - Feature contribution analysis & global feature importance
  - Transparent prediction pipeline

- **AI Research Copilot (RAG)**
  - Powered by Retrieval-Augmented Generation (RAG)
  - Multi-source evidence retrieval: Local knowledge base, scientific literature, arXiv, and public web sources
  - Delivers evidence-grounded insights for women's hormonal health research

- **Automated Research Reporting**
  - Generates downloadable reports (HTML/PDF) containing:
    - Dataset summary & pipeline metadata
    - Prediction statistics & risk distribution
    - Prediction preview & research disclaimers

---

## Project Workflow

```text
CSV Upload
    │
    ▼
Dataset Validation
    │
    ▼
Schema Mapping
    │
    ▼
Data Cleaning
    │
    ▼
Feature Engineering
    │
    ▼
Preprocessing
    │
    ▼
AI Risk Prediction
    │
    ▼
Explainability
    │
    ▼
AI Research Copilot (RAG)
    │
    ▼
Research Report Generation


Tech StackLayerTechnologiesFrontendStreamlitBackendPython 3.11+Data ProcessingPandas, NumPyMachine LearningScikit-learnAI & LLMGoogle Gemini, LangChainVector RetrievalFAISSResearch SourcesArXiv, DuckDuckGo Search, Local Knowledge BaseReportingHTML, PDF (when supported)Project StructurePlaintextHormoneBench-AI/
│
├── app.py
├── requirements.txt
├── assets/
│   └── style.css
│
├── services/
│   ├── __init__.py
│   ├── cleaning_service.py
│   ├── preprocessing_service.py
│   ├── prediction_service.py
│   ├── rag_service.py
│   └── report_service.py
│
├── utils/
│   ├── __init__.py
│   ├── constants.py
│   └── schema_mapper.py
│
├── knowledge_base/
├── models/
├── data/
└── README.md
Getting Started1. Clone the RepositoryBashgit clone [https://github.com/yourusername/HormoneBench-AI.git](https://github.com/yourusername/HormoneBench-AI.git)
cd HormoneBench-AI
2. Set Up a Virtual EnvironmentWindows:Bashpython -m venv .venv
.venv\Scripts\activate
Linux / macOS:Bashpython -m venv .venv
source .venv/bin/activate
3. Install DependenciesBashpip install -r requirements.txt
4. Configure Environment VariablesCreate a .env file in the root directory:Code snippetGOOGLE_API_KEY=YOUR_GEMINI_API_KEY
5. Run LocallyBashstreamlit run app.py
DeploymentThe application can be deployed directly on platforms such as Streamlit Community Cloud, Railway, or Render.Streamlit Community Cloud Setup:Push the project repository to GitHub.Sign in to Streamlit Community Cloud and click New app.Select your repository, branch, and set app.py as the entry point.Navigate to App Settings → Secrets and add:Ini, TOMLGOOGLE_API_KEY = "YOUR_GEMINI_API_KEY"
Click Deploy.Data SchemaThe platform expects a CSV file containing hormonal health metrics. The schema mapper automatically translates common column variations into the unified schema:Target ColumnDescriptionageParticipant agesleepAverage sleep duration/quality metricsheart_rateResting or baseline heart ratetemperatureBasal body temperaturestressRecorded stress level indicatorscycle_dayMenstrual cycle day indexbmiBody Mass IndexResearch Components & LimitationsResearch ComponentsDataset StandardizationScientific Validation PipelineAI Risk Prediction & Explainable AIRetrieval-Augmented Generation (RAG)Automated Research ReportingLimitationsResearch Prototype: Intended strictly for research and academic exploration.Clinical Validation: The models are not clinically validated or certified for medical diagnosis.API Dependency: The AI Research Copilot requires an active Google Gemini API key.TeamRoleMemberAI ArchitectTayyab NisarLead Data ScientistBeenish MeharUX ResearcherMahnoor AkramTechnical Lead (CTO)ZeeshanCitationIf you use HormoneBench AI in your research or academic work, please cite the project:Code snippet@software{hormonebench_ai,
  author = {Nisar, Tayyab and Mehar, Beenish and Akram, Mahnoor and Zeeshan},
  title = {HormoneBench AI: Open AI Research Infrastructure for Women's Hormonal Health},
  year = {2026},
  url = {[https://github.com/yourusername/HormoneBench-AI](https://github.com/yourusername/HormoneBench-AI)}
}
License & ContactLicense: Intended for research, education, and non-commercial innovation unless otherwise specified.Contact: Tayyab Nisar — LinkedInAcknowledgementsSpecial thanks to the open-source community and the developers of Streamlit, Pandas, NumPy, Scikit-learn, LangChain, Google Gemini, FAISS, ArXiv, and DuckDuckGo Search for enabling accessible AI research and innovation in women's health.
    │
    ▼
Download Results
