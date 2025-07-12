# HealthLLM Chatbot MVP Project

## Brief Project Overview
The Migraine Symptom Self-Assessment Chatbot is an educational tool built using **Ollama + AnythingLLM** stack with the **Llama3 model** to help users in Halifax, Nova Scotia, and across Canada recognize typical migraine symptoms and understand when to seek medical care. Based on Canadian health authority guidelines, this chatbot provides structured symptom assessment and educational information while maintaining strict ethical boundaries.

**⚠️ IMPORTANT: This chatbot is for EDUCATIONAL PURPOSES ONLY and does NOT provide medical diagnoses.**

**Key Features:**
- Evidence-based information from Canadian Headache Society guidelines
- Red flag symptom detection for emergency situations
- Educational migraine self-assessment support
- Crisis detection and emergency response protocols
- Canadian health resource referrals

**Technology Stack:** Ollama (Local LLM) + AnythingLLM (RAG Frontend) + Llama3 Model  
**Target Users:** Adults experiencing headaches seeking educational migraine information

## Project Structure
```
📂 /HealthLLM-Chatbot-MVP-Project
├─ knowledge_base/           # Medical knowledge and reference materials
│  ├─ canadian_headache_society_migraine_guidelines.md
│  ├─ choosing_wisely_headache_pain_reliever_pamphlet.md
│  ├─ headache_self_care_tips_health_canada.md
│  ├─ migraine_canada_patient_education_kit.md
│  ├─ q1_migraine_symptoms_with_sources.md    # Test results for core question 1
│  └─ q2_migraine_prevention_home_with_sources.md  # Test results for core question 2
├─ prompt/                   # Chatbot prompts and conversation templates
│  └─ system_prompt.md       # Core system prompt with role, scope, and ethics
├─ documentation/            # Project documentation and use cases
│  ├─ healthllm_chatbot_mvp_project.md   # Project requirements and instructions
│  ├─ migraine_scenario_pack.md          # Scenario pack with test questions
│  └─ use_case_description.md            # Detailed use case analysis
├─ demo/                     # Demo files and examples
│  ├─ Chat_Conscripts_Before_System_Prompt_RAG.txt  # Before implementation
│  ├─ Chat_Conscripts_After_System_Prompt_RAG.txt   # After implementation
│  └─ Demo_Video.mp4         # Demonstration video showing functionality
└─ README.md                 # This file
```

## Local Deployment/Testing Instructions

### Prerequisites
- **Operating System**: macOS, Linux, or Windows
- **Hardware**: Minimum 8GB RAM (16GB recommended for Llama3)
- **Storage**: At least 4GB free space for Llama3 model
- **Internet**: Required for initial downloads

### Setup Steps

#### 1. Install Ollama
**On macOS:**
```bash
# Download and install from https://ollama.com
# Or using Homebrew:
brew install ollama
```

**On Linux:**
```bash
curl -fsSL https://ollama.com/install.sh | sh
```

**On Windows:**
- Download the Windows installer from https://ollama.com
- Run the installer and follow the setup wizard

#### 2. Download and Set Up Llama3 Model
```bash
# Start Ollama service (if not already running)
ollama serve

# In a new terminal, pull the Llama3 model
ollama pull llama3

# Verify the model is installed
ollama list
```

#### 3. Install AnythingLLM
**Option A: Desktop Application (Recommended)**
- Download AnythingLLM desktop app from https://anythingllm.com
- Install and launch the application

**Option B: Docker Installation**
```bash
# Pull and run AnythingLLM with Docker
docker pull mintplexlabs/anythingllm
docker run -d -p 3001:3001 --name anythingllm mintplexlabs/anythingllm
```

#### 4. Configure AnythingLLM with Ollama
1. **Open AnythingLLM** in your browser (usually http://localhost:3001)
2. **Set up LLM Provider:**
   - Go to Settings > LLM Preference
   - Select "Ollama" as your provider
   - Set base URL to `http://localhost:11434`
   - Select "llama3" as your model
3. **Test Connection:** Verify Ollama connection is successful

#### 5. Upload Knowledge Base to AnythingLLM
1. **Create a Workspace** in AnythingLLM called "Migraine Assessment"
2. **Upload Documents:**
   - Navigate to your workspace
   - Upload all files from the `knowledge_base/` folder:
     - `canadian_headache_society_migraine_guidelines.md`
     - `choosing_wisely_headache_pain_reliever_pamphlet.md`
     - `headache_self_care_tips_health_canada.md`
     - `migraine_canada_patient_education_kit.md`
     - `q1_migraine_symptoms_with_sources.md` (test validation file)
     - `q2_migraine_prevention_home_with_sources.md` (test validation file)
3. **Wait for Processing:** Allow AnythingLLM to process and index the documents

#### 6. Configure System Prompt
1. **In your AnythingLLM workspace**, go to Settings
2. **Copy the content** from `prompt/system_prompt.md`
3. **Paste into System Prompt** field in AnythingLLM
4. **Save the configuration**

### Testing the Chatbot

#### Core Test Questions (From Scenario Pack)
Test your chatbot with these specific questions:
1. **"I get one-sided headaches with light sensitivity—is this a migraine?"**
2. **"What can I do to prevent migraine attacks at home?"**

#### Additional Test Scenarios
- Test red flag symptom detection (emergency situations)
- Verify appropriate disclaimers in responses
- Check crisis response protocols
- Test knowledge base retrieval accuracy

### Troubleshooting

#### Common Issues:
1. **Ollama not responding:**
   - Ensure Ollama service is running: `ollama serve`
   - Check if Llama3 model is installed: `ollama list`

2. **AnythingLLM can't connect to Ollama:**
   - Verify Ollama is running on port 11434
   - Check firewall settings
   - Ensure correct URL: `http://localhost:11434`

3. **Knowledge base not working:**
   - Verify documents are properly uploaded and processed
   - Check document format compatibility (Markdown/PDF/TXT)
   - Allow time for indexing to complete

### Performance Notes
- **Llama3 Model**: Requires significant computational resources
- **Response Time**: May be slower than cloud-based solutions
- **Privacy**: All processing happens locally on your machine
- **Resource Usage**: Monitor CPU and memory usage during operation

## Documentation
- `documentation/healthllm_chatbot_mvp_project.md` - Complete project requirements and instructions
- `documentation/migraine_scenario_pack.md` - Scenario pack with core test questions
- `documentation/use_case_description.md` - Detailed use case analysis with user pain points and success criteria
- `prompt/system_prompt.md` - Complete system prompt defining chatbot role, scope, and ethical guidelines

## Key Resources
- **Technology Stack**: Ollama + AnythingLLM + Llama3 Model
- **Knowledge Base**: Evidence-based medical information from Canadian health organizations + validated test results
- **System Prompt**: Comprehensive guidelines for chatbot behavior and safety protocols
- **Test Scenarios**: Specific questions for validation and demonstration
- **Test Results**: Documented responses showing successful implementation of core functionality

### Knowledge Base Files
The chatbot uses evidence-based information from these Canadian health authority sources:
- **Canadian Headache Society Guidelines**: Official migraine diagnostic and treatment guidelines
- **Choosing Wisely Canada**: Evidence-based headache pain reliever recommendations  
- **Health Canada Self-Care Tips**: Official government guidance for headache management
- **Migraine Canada Education Kit**: Comprehensive patient education materials
- **Q1 Test Results**: Validated responses for "one-sided headaches with light sensitivity" question
- **Q2 Test Results**: Validated responses for "migraine prevention at home" question

## Safety & Ethics
This project prioritizes user safety through:
- **Prominent "Not Medical Diagnosis" disclaimer** in all responses
- **Red flag symptom detection** with immediate emergency care direction
- **Crisis response protocols** for self-harm and violence detection
- **Evidence-based information** from Canadian health authorities only
- **Academic use only** - not for clinical deployment
- **Privacy protection** - no storage of personal health information

## ⚠️ IMPORTANT DISCLAIMERS
- **FOR EDUCATIONAL PURPOSES ONLY** - This chatbot does NOT provide medical diagnoses
- **NOT FOR CLINICAL USE** - Academic project only, not for real medical deployment
- **EMERGENCY SITUATIONS** - Always seek immediate medical care for serious symptoms
- **LOCAL PROCESSING** - All data stays on your local machine for privacy

## Development
### Contributing
- Follow medical ethics guidelines when adding content
- Ensure all medical information is evidence-based and properly cited
- Test all changes against the safety criteria outlined in the system prompt
- Update documentation when adding new features or knowledge base content

### Development Roadmap
- [x] Set up project structure and documentation
- [x] Create comprehensive system prompt with safety protocols
- [x] Curate Canadian health authority knowledge base
- [x] Document use cases and test scenarios
- [x] **Complete Ollama + AnythingLLM integration**
- [x] **Test with core scenario questions**
- [x] **Create demonstration video (max 2 minutes)**
- [x] **Document chat transcripts from testing**
- [ ] **Prepare 5-minute presentation**

### Testing Requirements (Academic)
- Test both core scenario questions from migraine_scenario_pack.md
- Document chat transcripts for evaluation
- Create video demonstration showing chatbot responses
- Verify red flag symptom detection works correctly
- Ensure all safety disclaimers appear in responses

### Technology Notes
- **Local Processing**: All LLM inference happens on your machine
- **No Internet Required**: After setup, chatbot works offline
- **Resource Intensive**: Llama3 requires significant CPU/memory
- **Privacy First**: No user data sent to external services

---

## Project Information
**Project**: Migraine Symptom Self-Assessment Chatbot MVP  
**Technology Stack**: Ollama + AnythingLLM + Llama3 Model  
**Author(s)**: Peter6188 (GitHub), HealthLLM Development Team  
**Institution**: 15 5893 Health Data Analytics Course  
**Project Start Date**: July 7, 2025  
**Last Updated**: July 12, 2025  
**Version**: 1.1 (MVP with Test Validation)  
**Purpose**: Academic research and educational use only  

**Contact**: GitHub Repository - https://github.com/Peter6188/HealthLLM-Chatbot-MVP-Project  

**Technology Resources:**
- [Ollama Documentation](https://github.com/ollama/ollama/blob/main/README.md)
- [AnythingLLM Documentation](https://docs.anythingllm.com)
- [Llama3 Model Information](https://ollama.com/library/llama3)

**Acknowledgments**: 
- Canadian Headache Society for evidence-based guidelines
- Health Canada for public health resources
- Migraine Canada for patient education materials
- Choosing Wisely Canada for evidence-based recommendations
- Ollama team for local LLM infrastructure
- AnythingLLM team for RAG frontend platform
