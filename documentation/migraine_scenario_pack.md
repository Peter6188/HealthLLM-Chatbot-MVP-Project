
# 🩺 Migraine Symptom Self-Assessment Chatbot Scenario Package

## 📖 Scenario Background
In Halifax, Nova Scotia, migraine is a common neurological condition that can cause severe, throbbing headaches, often on one side of the head.  
Symptoms may include nausea, light or sound sensitivity, and can be disabling if not properly managed.  
Health Canada, the Canadian Headache Society, and patient organizations provide guidelines to help people recognize migraine features, identify warning signs, and adopt self-management strategies.

This scenario asks students to use the **Ollama + AnythingLLM** stack, combined with locally available, authoritative health education materials, to design a chatbot for **Migraine Symptom Self-Assessment**.

## 🎯 Scenario Goals
- Help users recognize typical migraine symptoms and red flag features  
- Guide users on lifestyle triggers and home-care strategies  
- Clearly communicate that the chatbot does **not** provide professional medical diagnoses  

## 🗂 Recommended Knowledge Base Materials
Students should collect and organize **retrievable, structured** local health education materials to serve as their RAG knowledge base.  
Recommended sources include:
- Canadian Headache Society – Migraine Diagnosis and Management Guidelines  
- Health Canada – Patient Tips for Headache Self-Care  
- Headache Network Canada – Red Flag Symptom Checklists  
- Nova Scotia Health – Managing Headache Triggers and Lifestyle Advice  
- Any relevant local public health resources  

**Requirement:** Upload as PDF, Markdown, or plain text, using consistent file names such as:
- `knowledge_document_1.pdf`  
- `knowledge_document_2.md`  
- `knowledge_document_3.txt`  

## 🎯 Suggested User Questions for Testing
Your final system must be able to answer these scenario questions using your uploaded knowledge base materials:
1. *"I get one-sided headaches with light sensitivity—is this a migraine?"*  
2. *"What can I do to prevent migraine attacks at home?"*

---

## 📦 Suggested GitHub Repository Structure
All project deliverables must be uploaded to a GitHub Repository. Recommended folder structure:
```
/cold-flu-chatbot
├─ knowledge_base/
│  ├─ knowledge_document_1.pdf
│  ├─ knowledge_document_2.md
│  └─ knowledge_document_3.txt
├─ prompt/
│  └─ system_prompt.txt
├─ documentation/
│  ├─ scenario_pack.md (Provided)
│  └─ use_case_description.md
├─ demo/
│  ├─ demo_video.mp4
│  └─ chat_transcript.txt
└─ README.md
```

---

## 📑 Deliverables
- **Knowledge Base:**  
  Include all documents actually used in AnythingLLM, clearly structured and properly named.
- **System Prompt:**  
  Defines chatbot role, tone, scope, and disclaimers.
- **Use Case Description:**  
  Document identifying user pain points and success criteria.
- **Demo Materials:**  
  - Screen recording or video showing chatbot responses to the core scenario questions.  
  - Chat transcript.
- **README.md:**  
  - Project overview  
  - Deployment/testing instructions  
  - Author(s) and date

---

## ⚠ Important Notes
- All materials must be uploaded to a **public or private GitHub Repository** for review.
- The project is for **educational research use only** and must **not** be used for real diagnosis or treatment.
- The chatbot’s README.md file must prominently display a **“Not Medical Diagnosis”** disclaimer.
