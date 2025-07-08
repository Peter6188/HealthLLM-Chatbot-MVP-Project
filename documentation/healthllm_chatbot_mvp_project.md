project-description.md 2025-07-04

Yep HealthLLM Chatbot MVP Project

Design and Evaluate a Domain-Specific Chatbot with Ollama +
AnythingLLM

Project Overview

In this project, you will be randomly assigned a specific healthcare scenario. You will build a Minimum
Viable Product (MVP) LLM-powered chatbot designed to support that scenario, using RAG (Retrieval-
Augmented Generation) and System Prompt engineering techniques on a local framework.

A You will not train your own model. Your goal is to design, configure, and test:
©) A well-curated, scenario-specific Knowledge Base.
©) A precise System Prompt defining the chatbot's role, tone, and ethical boundaries.

@ Project Goals

Goal Description
Understand the design of conversational Al in Including user needs, scenario constraints, and
sensitive domains compliance requirements.

From data collection > cleaning > indexing > usage

Master the RAG pipeline . .
in AnythingLLM.

. . Clearly define role, tone, scope, and ethical
Craft high-quality System Prompts

boundaries.
Identify and mitigate ethical risks in Including crisis response, privacy protection, and
healthcare Al disclaimers.
& Provided Technology Stack
Component Purpose Notes

Local LLM backend (e.g., Mistral,

CLI-based, downloads and runs models locally.
LLaMA)

Ollama

. Supports document upload, indexing, prompt
AnythingLLM Front-end and RAG management
management.

Tutorial . . . . ae
. Quickstart guides & demos Setup instructions, troubleshooting tips.
Materials

@ Scenario Materials

Each student will receive a “Scenario Pack” (Markdown) containing:

1/4


project-description.md 2025-07-04

Field Example Description

Scenario . . . Background context, user needs,
woe “Managing Mild Anxiety for College Students” .

Description constraints.

Undergraduate students experiencing mild

Target User May include demographic details.

anxiety
C ti Identify st & t evid -based
‘onversation en ify si ressors suggest evidence-base Defines what success looks like.
Goal coping strategies
. . Define the role that the chatbot
Chatbot Role “Friendly, supportive wellness coach” .
will play.
Test Questions 2 standard test questions Used for evaluation.
f@ Task Breakdown
1] Read Your Assigned Scenario Pack
© Produce a clear that identifies user pain points and success criteria.

I]

Prepare the Knowledge Base

* Collect highly relevant, evidence-based resources (e.g., clinical guidelines, hotline information,
authoritative blogs, etc.).

© Clean and format these as PDF/Markdown/TXT compatible with AnythingLLM.

¢ Emphasize clarity, focus, and utility.

|

Design Your System Prompt

* Must include:

© Explicit role definition and tone (e.g., warm, non-judgmental).

© Scope limitations.

© Required disclaimers (e.g., "Not professional medical advice").

© Crisis-response instructions (e.g., self-harm triggers emergency help suggestions).
¢ Iterate: test and refine for clarity and alignment.

4] Integration and Testing

© Upload documents and prompt in AnythingLLM.
* Bind the model and run realistic conversation tests.
¢ Record transcripts and refine as needed.

Submission

a

¢ Push all materials to a GitHub repository.
¢ Prepare a demonstration video (no more than 2 mins)
¢ Be ready for a 5-minute presentation session.

© Expected Deliverable Structure
214


project-description.md

6

/healthcarellm-chatbot-mvp

knowledge_base/

t- knowledge_document_1.pdf
t- knowledge_document_2.md
L knowledge_document_3.txt

2025-07-04

prompt/
L system_prompt.txt
documentation/

[- demo/

EL demo_video.mp4

LU chat_transcript.txt
“README .md

L scenario_pack.md (Provided)
L use _case_description.md

The chatbot README.md file must prominently display a “Not Medical Diagnosis” disclaimer.

Grading Rubric

Criterion

Description

Knowledge Base Relevance and
Quality
(20 points)

1. Curates highly relevant, evidence-based documents tailored to the
assigned scenario.

2. Ensures clean, structured, AnythingLLM-compatible formatting.

3. Demonstrates clear focus without irrelevant content, with explained
selection rationale.

System Prompt Design and
Ethics
(20 points)

1. Explicitly defines chatbot role, tone, functionality, and boundaries.
2. Includes mandatory disclaimers and crisis-response guidance.
3. Shows understanding of ethical risks and integrates safeguards.

Integration and Testing in
AnythingLLM
(20 points)

1. Successfully uploads and configures the knowledge base and
prompt.

2. Conducts realistic test conversations simulating user queries.
3. Documents and iterates design based on test results.

Documentation and Reflection
(20 points)

1. Clearly describes use case, user group, goals, and ethical
considerations.

2. Explains knowledge base content and prompt design reasoning.
3. Includes reflective analysis of design decisions, challenges, and
potential improvements.

Presentation and
Demonstration
(20 points)

1. Provides a clear, structured video showcasing the chatbot in action.
2. Highlights integration of RAG and ethical guidelines.

3. Successfully uploads to personal GitHub repo in the provided
format.

& Ethical and Compliance Requirements

3/4



project-description.md 2025-07-04

¢ A\ For academic use only; NOT for deployment in clinical settings.

¢ Must prominently display a “Not Medical Diagnosis” disclaimer in the README.md.

¢ Must design for crisis detection (e.g., self-harm, violence) and direct users to emergency resources.
* Absolutely no collection or storage of real users’ sensitive personal data.

@ Recommended Resources

* Ollama Docs

¢ AnythingLLM Docs

© Prompt Engineering Guide

© OBS Studio (for recording)

¢ GitHub Documentation (official guide)

@5 Questions / Technical Support

Please email . Teaching Assistant will respond within 24 hours.

Let's rapidly prototype responsible, domain-aware Al tools that truly support users in healthcare contexts!


