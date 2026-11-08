# arogyashield-ai-health-risk-monitoring
An AI-driven health risk assessment system integrating voice input, image analysis, symptom extraction, and medical document-based question answering.
# ArogyaShield: AI-Driven Diagnosis and Risk Monitoring System

## Overview

ArogyaShield is an AI-driven health risk assessment system designed to make preliminary health information more accessible through multiple input methods. It combines voice interaction, image analysis, natural language processing, machine learning, and medical document-based question answering in a single application.

The system allows users to provide health-related information through voice, images, text, or manually selected symptoms. It processes these inputs to identify relevant symptoms and estimate health risk levels.

ArogyaShield also includes a medical document question-answering feature that allows users to retrieve information from uploaded medical PDFs.

## Key Features

- **Voice-Based Input:** Uses Groq Whisper Large-v3 for speech-to-text transcription, allowing users to describe symptoms through voice.
- **Image Analysis:** Uses LLaMA-3 Vision to analyse uploaded images and extract relevant information.
- **Symptom Extraction:** Applies NLP techniques using NLTK to identify symptoms and map them to relevant features.
- **AI-Based Risk Assessment:** Uses a Random Forest classifier to analyse symptom patterns and categorise the estimated health risk as Low, Medium, or High.
- **Medical Document Q&A:** Uses LangChain, FAISS vector storage, and Mistral-7B to retrieve relevant information from uploaded medical PDFs.
- **Text-to-Speech:** Integrates ElevenLabs to convert generated responses into speech.
- **Email Alerts:** Uses SMTP-based email notifications to send alerts when a high-risk result is identified.
- **Interactive Interface:** Provides a Gradio-based interface for interacting with the system.

## Technology Stack

| Component | Technologies |
|---|---|
| Programming Language | Python |
| User Interface | Gradio |
| Machine Learning | Scikit-learn, Random Forest |
| Natural Language Processing | NLTK |
| Speech Recognition | Groq Whisper Large-v3 |
| Image Analysis | LLaMA-3 Vision |
| LLM Integration | Mistral-7B |
| Document Retrieval | LangChain, FAISS |
| Text-to-Speech | ElevenLabs |
| Notifications | SMTP |

## System Workflow

1. **Input Collection:** Users provide health-related information through voice, images, text, or manual symptom selection.
2. **Input Processing:** Voice input is transcribed, images are analysed, and text is processed to extract relevant symptoms.
3. **Symptom Mapping:** Extracted symptoms are processed and mapped into features for the machine learning model.
4. **Risk Assessment:** The Random Forest classifier analyses the symptom features and generates a risk category.
5. **Information Retrieval:** Users can also ask questions about uploaded medical PDFs through the document-based question-answering module.
6. **Response Generation:** The system generates responses and can read them aloud using text-to-speech.
7. **Alert Notification:** Email alerts are triggered for high-risk results.

## Model Evaluation

The research evaluated the Random Forest classifier against other machine learning approaches.

| Model | Reported Accuracy |
|---|---:|
| Random Forest | 93% |
| K-Nearest Neighbours (KNN) | 62% |
| Decision Tree | 58% |
| Support Vector Machine (SVM) | 51% |

The reported results indicate that Random Forest performed best among the evaluated models in the experimental setup described in the research paper.

*Note: These are research-reported experimental results, not evidence of clinically validated diagnostic performance.*

## Project Structure

The following are the main files identified in the research paper. Update this section to match the actual repository structure.

```text
ArogyaShield/
│
├── main_app.py
├── llm_interface.py
├── voice_of_the_patient.py
├── README.md
└── ...
```

## Getting Started

### Prerequisites

- Python installed on your system.
- Required Python libraries and dependencies.
- API access for the external AI services used by the application.

### Installation

1. Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
```

2. Navigate to the project directory:

```bash
cd YOUR_REPOSITORY_NAME
```

3. Install the dependencies using the project's requirements file, if available:

```bash
pip install -r requirements.txt
```

4. Configure the required API credentials and environment variables for the external services.

5. Run the application using its main entry-point file. Confirm the correct command from the project code before running it.


