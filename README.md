# AI-Assisted CDSS Evaluation Tool: Overcoming Automation Bias

This data collection and testing tool was developed for evaluating Cognitive Forcing Functions (CFFs) in Artificial Intelligence-assisted Clinical Decision Support Systems (AI-CDSS) in Dentistry. Specifically, this application was built to simulate a dental diagnostic workflow (detecting proximal caries in bite-wing radiographs) to measure and mitigate clinician over-reliance on AI.

## Features

The tool acts as a simulated AI-CDSS and tests participants across three distinct User Interface (UI) conditions, employing Latin Square Design randomization to mitigate learning effects:

-	**Standard AI Interface (Control)**: The radiograph is presented alongside a simultaneous overlay of the AI's diagnostic recommendation. Designed to mimic standard "frictionless" workflows. <p align="center"> <img src="images/standard.png" width="300"> </p>
-	**Optional AI Interface (CFF 1)**: Introduces intentional cognitive friction. The user is presented with the radiograph and must explicitly click a button if they choose to view the AI output. <p align="center"> <img src="images/optional.png" width="300"> </p>
-	**Staged AI Interface (CFF 2)**: Forces analytical engagement. The AI recommendation is withheld until the user submits their initial, independent diagnosis. Afterward, the AI output is displayed, and the user is given the opportunity to submit a revised, final diagnosis. <p align="center"> <img src="images/staged.png" width="300"> </p>

## Experimental Workflow
### 1. Project Introduction
The landing page introducing the scope of the study. It discloses that the embedded AI assistant is 90% accurate in identifying proximal caries on bitewing radiographs and establishes task scope and criteria.
<p align="center"> <img src="images/intro_page.png" width="300"> </p>

### 2. Informed Consent

<p align="center"> <img src="images/consent_page.png" width="300"> </p>

### 3. Participant Details
Collection of demographic data and professional details (Age, Years of Dental Experience, Dental Specialization), and a **Pre-Task Questionnaire -** Trust in AI-Generated Health Advice Scale.
<p align="center"> <img src="images/parti_page.png" width="300"> </p>

### 4. Diagnostic Task
Participants evaluate 12 bitewing radiographs (4 per interface condition). *Note: To test for automation bias (Errors of Omission and Commission), 50% of the cases within each interface deliberately feature incorrect AI recommendations.*

### 5. Post-Task Questionnaires
After completing the cases for a specific interface, participants complete 1-5 Likert scale surveys:
      - Raw NASA-TLX (measuring Mental Demand, Temporal Demand, Performance, and Frustration).
      - Overall Usefulness scale
      - Ease of Use scale
<p align="center"> <img src="images/post_task_ques_1.png" width="300"> </p>
<p align="center"> <img src="images/post_task_quest_2.png" width="300"> </p>

### 6. Post Study Debrief
After completing all the 12 cases, a debrief about the study mentioning its true purpose is displayed. 
<p align="center"> <img src="images/debrief_page.png" width="300"> </p>

## Metrics

- **Diagnostic Accuracy:** Recorded by comparing the user's final submitted diagnosis against the ground-truth label of the radiograph.
- **Decision Time:** The total time taken (in seconds) to diagnose each individual case.
- **Diagnosis Change Rate:** Tracking instances where a user alters their initial diagnosis after viewing the AI recommendation (specifically in the Staged interface).

## Ethics 

This application is designed in compliance with the General Data Protection Regulation (GDPR) and the Declaration of Helsinki.
- Anonymization: All participant data (demographics, performance metrics) are strictly anonymized.
- Consent: Digital informed consent is built into the first view of the application.
- Data Sourcing: The radiographic images utilized in the application are derived from an existing validated dataset specifically for research purposes.


