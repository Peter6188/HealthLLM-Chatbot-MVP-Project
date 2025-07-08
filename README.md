# HealthLLM Chatbot MVP Project

## Brief Project Overview
The HealthLLM Chatbot is an evidence-based health data analytics tool designed to provide accessible support for individuals experiencing headaches and migraines. Built on Canadian medical guidelines and reputable health resources, this chatbot offers structured symptom assessment, educational information, and appropriate healthcare guidance while maintaining strict ethical and safety standards.

**Key Features:**
- 24/7 accessible symptom assessment
- Evidence-based information from Canadian Headache Society guidelines
- Red flag symptom detection for emergency situations
- Self-care and prevention education
- Appropriate healthcare provider referrals

**Target Users:** Adults experiencing headaches/migraines, caregivers, and individuals seeking reliable health information between medical appointments.

## Project Structure
```
📂 /HealthLLM-Chatbot-MVP-Project
├─ knowledge_base/           # Medical knowledge and reference materials
│  ├─ canadian_headache_society_migraine_guidelines.md
│  ├─ choosing_wisely_headache_pain_reliever_pamphlet.md
│  ├─ headache_self_care_tips_health_canada.md
│  └─ migraine_canada_patient_education_kit.md
├─ prompt/                   # Chatbot prompts and conversation templates
│  └─ system_prompt.md       # Core system prompt with role, scope, and ethics
├─ documentation/            # Project documentation and use cases
│  ├─ scenario_pack.pdf      # Provided scenario pack
│  ├─ use_case_description.pdf # Original use case descriptions
│  └─ use_case_description.md  # Detailed use case analysis
├─ demo/                     # Demo files and examples
└─ README.md                 # This file
```

## Local Deployment/Testing Instructions

### Prerequisites
- Python 3.8 or higher
- Git
- Text editor or IDE (VS Code recommended)

### Setup Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/Peter6188/HealthLLM-Chatbot-MVP-Project.git
   cd HealthLLM-Chatbot-MVP-Project
   ```

2. **Set Up Virtual Environment** (Recommended)
   ```bash
   python -m venv healthllm_env
   
   # On macOS/Linux:
   source healthllm_env/bin/activate
   
   # On Windows:
   healthllm_env\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt  # (To be created based on chosen framework)
   ```

4. **Review Configuration**
   - Review `prompt/system_prompt.md` for chatbot behavior settings
   - Ensure all knowledge base files are present in `knowledge_base/` folder
   - Check documentation for use case requirements

5. **Testing the Chatbot** (Framework dependent)
   ```bash
   # Example commands (will vary based on implementation)
   python main.py                    # For standalone Python implementation
   streamlit run app.py             # For Streamlit web app
   jupyter notebook demo.ipynb      # For Jupyter notebook demo
   ```

### Development Testing
- **Knowledge Base Testing**: Verify all `.md` files in `knowledge_base/` are accessible
- **Prompt Testing**: Test system prompt effectiveness with sample queries
- **Safety Testing**: Ensure red flag symptoms trigger appropriate warnings
- **Edge Case Testing**: Test with various symptom combinations and edge cases

### Deployment Notes
- Ensure all sensitive information is properly secured
- Review medical disclaimers before public deployment
- Consider implementing rate limiting for production use
- Set up proper logging for monitoring and improvement

## Documentation
- `documentation/scenario_pack.pdf` - Provided scenario pack
- `documentation/use_case_description.pdf` - Original use case descriptions  
- `documentation/use_case_description.md` - Detailed use case analysis with user pain points and success criteria
- `prompt/system_prompt.md` - Complete system prompt defining chatbot role, scope, and ethical guidelines

## Key Resources
- **Knowledge Base**: Evidence-based medical information from Canadian health organizations
- **System Prompt**: Comprehensive guidelines for chatbot behavior and limitations
- **Use Cases**: Detailed user personas and success metrics for development guidance

## Safety & Ethics
This project prioritizes user safety through:
- Clear medical disclaimers and limitations
- Red flag symptom detection (SNOOPPPP criteria)
- Mandatory emergency referrals when appropriate
- Evidence-based information from reputable medical sources
- Regular content updates based on current medical guidelines

## Development
### Contributing
- Follow medical ethics guidelines when adding content
- Ensure all medical information is evidence-based and properly cited
- Test all changes against the safety criteria outlined in the system prompt
- Update documentation when adding new features or knowledge base content

### Development Roadmap
- [ ] Implement core chatbot framework
- [ ] Integrate knowledge base with conversation logic
- [ ] Add symptom assessment questionnaire
- [ ] Implement red flag detection system
- [ ] Create web interface for user interaction
- [ ] Add comprehensive testing suite
- [ ] Implement usage analytics and feedback collection

### Code Standards
- Follow PEP 8 for Python code formatting
- Include comprehensive docstrings for all functions
- Implement proper error handling and logging
- Ensure HIPAA compliance for any user data handling

---

## Project Information
**Author(s)**: Peter6188 (GitHub), HealthLLM Development Team  
**Institution**: 15 5893 Health Data Analytics Course  
**Project Start Date**: July 7, 2025  
**Last Updated**: July 7, 2025  
**Version**: 1.0 (MVP)  
**License**: [To be determined - consider medical software licensing requirements]

**Contact**: GitHub Repository - https://github.com/Peter6188/HealthLLM-Chatbot-MVP-Project  

**Acknowledgments**: 
- Canadian Headache Society for evidence-based guidelines
- Health Canada for public health resources
- Migraine Canada for patient education materials
- Choosing Wisely Canada for evidence-based recommendations
