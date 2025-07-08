# Use Case Description: Migraine Symptom Self-Assessment Chatbot

## Executive Summary
The Migraine Symptom Self-Assessment Chatbot is an educational tool designed to help users in Halifax, Nova Scotia, and across Canada recognize typical migraine symptoms, identify red flag features, and understand lifestyle management strategies. Built using the Ollama + AnythingLLM stack with Canadian health authority resources, this chatbot serves as a preliminary self-assessment tool while emphasizing that it does NOT provide medical diagnoses.

## User Pain Points

### Primary Pain Points
1. **Difficulty Recognizing Migraine Symptoms**
   - Users struggle to differentiate between tension headaches and migraines
   - Uncertainty about whether their symptoms warrant medical attention
   - Lack of awareness about red flag symptoms requiring immediate care

2. **Limited Access to Immediate Symptom Assessment**
   - Healthcare appointments not immediately available for non-emergency headaches
   - Users need quick guidance on whether symptoms are typical migraine features
   - Uncertainty about self-management strategies during migraine episodes

3. **Information Overload About Migraine Management**
   - Overwhelming amount of conflicting information about migraine triggers and treatments
   - Difficulty identifying evidence-based Canadian health resources
   - Confusion about which lifestyle modifications are scientifically supported

4. **Inadequate Understanding of Warning Signs**
   - Users may not recognize red flag symptoms that require emergency care
   - Lack of clear guidance on when self-assessment is appropriate vs. professional consultation
   - Uncertainty about migraine vs. other headache types requiring different approaches

### Secondary Pain Points
- Anxiety about symptom severity and progression
- Geographic barriers to specialist care (especially in Nova Scotia)
- Language barriers in accessing Canadian health resources
- Time constraints preventing thorough symptom documentation
- Fear of "bothering" healthcare providers with non-emergency symptoms

## Target Users

### Primary Users
- **Adults experiencing headaches** who want to understand if their symptoms match migraine patterns
- **Individuals with suspected migraines** seeking educational information about their condition
- **People in Halifax/Nova Scotia** and across Canada looking for Canadian health authority guidance
- **Students and working adults** needing quick symptom assessment during busy schedules

### User Personas
1. **Sarah, 32, Marketing Professional in Halifax**
   - Experiences one-sided headaches with light sensitivity 2-3 times per month
   - Wonders if these are migraines and wants to understand typical patterns
   - Needs quick assessment during work hours without immediate medical consultation
   - Goals: Understand if symptoms match migraine criteria, learn evidence-based management

2. **David, 45, Construction Worker in Rural Nova Scotia**
   - Has severe headaches occasionally, unsure about when to seek medical care
   - Limited access to immediate healthcare in rural area
   - Needs clear guidance on red flag symptoms requiring emergency attention
   - Goals: Recognize warning signs, understand when self-care is appropriate vs. medical care

3. **Maria, 28, University Student**
   - Recently started experiencing headaches with nausea and light sensitivity
   - Wants to understand if this could be migraine before seeing campus health services
   - Interested in lifestyle modifications and trigger identification
   - Goals: Learn about migraine features, understand prevention strategies

## Core Scenario Test Questions
The chatbot must effectively respond to these specific test scenarios:
1. **"I get one-sided headaches with light sensitivity—is this a migraine?"**
2. **"What can I do to prevent migraine attacks at home?"**

## Success Criteria

### User Experience Success Metrics
- **Educational Value**: Users learn to recognize typical migraine symptoms and patterns
- **Safety**: 100% accurate identification and response to red flag symptoms  
- **Clarity**: Users understand the chatbot's educational purpose and limitations
- **Accessibility**: Available 24/7 for initial symptom assessment and education
- **Canadian Relevance**: Responses based on Canadian health authority guidelines

### Clinical Success Metrics
- **Symptom Recognition**: Accurate description of migraine characteristics vs. other headache types
- **Red Flag Detection**: Perfect identification of symptoms requiring immediate medical attention
- **Educational Effectiveness**: Users gain knowledge about migraine management and triggers
- **Appropriate Referrals**: Clear guidance on when to seek professional medical evaluation

### Safety Success Metrics
- **Zero False Reassurance**: Never minimizes potentially serious symptoms
- **Crisis Detection**: Identifies and responds appropriately to emergency situations
- **Clear Disclaimers**: Consistently reinforces educational purpose, not medical diagnosis
- **Professional Care Advocacy**: Encourages appropriate medical consultation when indicated

## Functional Requirements

### Core Features
1. **Migraine Symptom Assessment Tool**
   - Structured questions about headache characteristics (location, quality, duration)
   - Assessment of associated symptoms (nausea, light/sound sensitivity, aura)
   - Red flag symptom detection (sudden onset, neurological signs, fever, etc.)

2. **Educational Resources from Canadian Authorities**
   - Canadian Headache Society guidelines and recommendations
   - Health Canada patient education materials
   - Nova Scotia Health resources for local users
   - Evidence-based information about migraine features and management

3. **Trigger and Lifestyle Guidance**
   - Information about common migraine triggers
   - Evidence-based prevention strategies
   - Lifestyle modifications supported by Canadian health guidelines
   - Home care strategies during migraine episodes

4. **Crisis Detection and Response**
   - Immediate identification of emergency symptoms
   - Clear instructions to seek emergency medical care when appropriate
   - Crisis response for mental health emergencies (self-harm, violence)
   - Connection to emergency resources and hotlines

### Technical Requirements
- **Ollama + AnythingLLM Integration**: Local LLM backend with RAG capabilities
- **Canadian Knowledge Base**: Documents from Canadian Headache Society, Health Canada, NS Health
- **Natural Language Processing**: Understanding of symptom descriptions and medical terminology
- **Multi-format Support**: PDF, Markdown, and TXT document compatibility
- **Privacy Compliance**: No storage of personal health information

## Expected Outcomes

### Short-term (1-3 months)
- Improved recognition of migraine symptoms among users
- Increased awareness of red flag symptoms requiring immediate care
- Better understanding of evidence-based migraine management strategies
- Reduced anxiety through educational support and clear guidance

### Medium-term (3-6 months)
- More informed discussions between users and healthcare providers
- Appropriate self-assessment leading to timely medical consultation when needed
- Increased adoption of lifestyle modifications for migraine prevention
- Enhanced user confidence in recognizing symptom patterns

### Long-term (6+ months)
- Improved health literacy regarding migraine and headache disorders
- Strengthened patient-provider relationships through better symptom communication
- Reduced inappropriate emergency department visits for routine headaches
- Enhanced quality of life through better migraine self-understanding and management

## Risk Mitigation

### Academic and Ethical Compliance
- **Educational Use Only**: Explicitly designed for academic research, not clinical deployment
- **"Not Medical Diagnosis" Disclaimer**: Prominently displayed in all interfaces and documentation
- **Canadian Privacy Laws**: Compliance with provincial and federal privacy regulations
- **No Personal Data Storage**: Absolute prohibition on storing users' sensitive health information
- **Professional Oversight**: Regular review by healthcare professionals for content accuracy

### Technical and Operational Risks
- **Ollama/AnythingLLM Integration**: Ensure robust local deployment and knowledge base updating
- **Knowledge Base Currency**: Regular updates to reflect current Canadian health guidelines
- **Response Consistency**: Validation of chatbot responses across different query types
- **User Feedback Integration**: Continuous improvement based on user testing and feedback

### Safety and Crisis Management
- **Crisis Response Protocols**: Immediate referral to emergency services for mental health crises
- **Red Flag Symptom Recognition**: Fail-safe identification of emergency medical symptoms
- **Clear Scope Communication**: Consistent messaging about chatbot limitations and educational purpose
- **Emergency Resource Connection**: Direct links to Canadian crisis hotlines and emergency services

---
**Document Version**: 2.0  
**Last Updated**: July 7, 2025  
**Author**: HealthLLM Development Team - 15 5893 Health Data Analytics Course  
**Project**: Migraine Symptom Self-Assessment Chatbot MVP  
**Technology Stack**: Ollama + AnythingLLM  
**Review Date**: October 7, 2025  
**Scenario**: Halifax, Nova Scotia Migraine Self-Assessment Support
