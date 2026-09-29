# AI-901: Azure AI Fundamentals  
## Industry-Based AI Workload Selection Case Studies

### Team Assignment

**Team Size:** 3–4 students  
**Course:** Microsoft Azure AI Fundamentals (AI-901)  
**Assignment Type:** Industry Case Study and AI Solution Analysis  
**Total Marks:** 100

---

# Assignment Overview

Organizations increasingly have access to large volumes of images, documents, text, audio, video, sensor data, and business records. The challenge is not simply to identify where AI can be used, but to determine **which AI workload is most appropriate**, what Azure capabilities could support it, what alternatives exist, and what risks must be addressed.

For this assignment, each team will analyze **one industry case study** and act as an AI consulting team. You are **not required to implement or code the solution**. Your objective is to understand the business problem, evaluate multiple AI approaches, select the most appropriate workload, and justify your recommendation.

Your analysis should demonstrate that the team can distinguish among:

- Machine Learning
- Computer Vision
- Natural Language Processing
- Conversational AI
- Document Intelligence / Information Extraction
- Knowledge Mining and Search
- Generative AI
- Speech AI
- Responsible AI considerations

### Important

Do not select an AI workload simply because it appears in the available data.

For example:

> The presence of images does not automatically mean Computer Vision is the best solution.

Students must explain **why the selected workload addresses the business objective better than realistic alternatives**.

---

# Scenario 1 — Healthcare
## MedCare Regional Hospital: Intelligent Patient Referral Processing

### 1. Background

MedCare Regional Hospital is a 600-bed multi-specialty hospital serving approximately 400,000 patients annually. The hospital receives referrals from general practitioners, clinics, diagnostic centers, insurance providers, and other hospitals. Referrals may be received through email, scanned documents, PDF forms, handwritten notes, medical reports, or electronic systems.

The hospital's specialist referral department currently employs 18 administrative staff members who manually review incoming referral packages. They identify patient information, medical conditions, previous test results, urgency indicators, referring physician details, and requested specialties before routing the referral to the appropriate department.

The hospital has identified several operational problems. Referral processing can take between several hours and two business days. Staff members spend substantial time reading documents and copying information into hospital systems. Some referrals are routed to the wrong department or marked with the wrong urgency level, resulting in delays for patients. Hospital management wants to improve processing speed while ensuring that AI does **not independently make clinical decisions or replace physicians**.

The hospital's CIO is considering several possibilities, including machine learning, document processing, NLP, and generative AI. The project team must determine where AI would provide the greatest value without introducing unacceptable clinical risk.

### 2. Available Data

The hospital has access to:

- Scanned referral forms
- PDF medical reports
- Laboratory reports
- Radiology summaries
- Patient demographic information
- Referral letters
- Physician notes
- Email messages from referring clinics
- Historical referral routing records
- Historical processing times
- Specialist department information
- Approximately 500,000 historical referral cases
- A small number of handwritten documents
- Multilingual documents, primarily English and two regional languages

The historical dataset includes examples of the department to which each referral was ultimately routed, but some historical routing decisions are inconsistent.

### 3. Business Problem

MedCare wants to create an AI-assisted referral-processing system that can:

1. Extract relevant information from incoming referral packages.
2. Identify the probable specialty required.
3. Highlight potentially urgent referrals for human review.
4. Reduce administrative processing time.
5. Reduce manual data entry.
6. Maintain human oversight for all clinically significant decisions.

The hospital does **not** want the AI system to diagnose patients or independently approve medical treatment.

### 4. Constraints

The solution must consider:

- Strict patient privacy and security requirements.
- High accuracy for extracted patient and medical information.
- Human review for clinically significant decisions.
- A limited initial project budget.
- A target pilot deployment within six months.
- Increasing referral volume over the next five years.
- Historical data quality is inconsistent.
- Handwritten documents may produce lower extraction accuracy.
- The organization cannot tolerate silent AI errors in urgent referrals.
- The hospital wants auditability of important AI-assisted decisions.

### 5. Student Tasks

Your team must:

1. Identify the **most suitable primary Azure AI workload**.
2. Explain why it is appropriate for the business problem.
3. Identify at least **two alternative AI workloads** that appear plausible.
4. Explain why those alternatives are less appropriate as the primary solution.
5. Recommend relevant Azure AI services or capabilities.
6. Explain where human review should be included.
7. Identify privacy, safety, fairness, transparency, and accountability risks.
8. Recommend appropriate success metrics.
9. Explain what additional data or validation would be required before production deployment.
10. Identify one situation in which the AI system should deliberately **defer to a human**.

### 6. Expected Learning Outcome

Students should demonstrate understanding of:

- Information extraction and document-processing workloads
- NLP and classification
- Machine-learning classification
- Document Intelligence
- Human-in-the-loop design
- AI reliability and safety
- Healthcare privacy considerations
- Responsible AI in high-impact domains

Azure Document Intelligence can extract text, tables, structure, and key/value information from structured, semi-structured, and unstructured documents and supports prebuilt and custom models.

---

# Scenario 2 — Retail & E-Commerce
## UrbanCart: Intelligent Product Returns and Damage Assessment

### 1. Background

UrbanCart is a large e-commerce retailer selling electronics, appliances, furniture, fashion, and household products. The company processes approximately 35,000 product returns every week. Returns are currently reviewed through a combination of automated rules and human inspection.

Customers may provide photographs of damaged products when submitting a return request. Customer-service representatives then review the photographs, order history, customer comments, delivery information, and previous return records before approving or rejecting the request.

UrbanCart has discovered significant inconsistency in the process. Some genuine damaged products are incorrectly rejected, while other returns involving signs of misuse or repeated abuse are approved. The company also receives thousands of customer reviews and support conversations describing product defects, packaging problems, missing components, and delivery damage.

Management wants an AI solution that can improve return processing while also identifying broader patterns in product quality and customer experience.

### 2. Available Data

UrbanCart has:

- Customer-submitted product photographs
- Warehouse inspection photographs
- Product catalog images
- Order history
- Return history
- Customer reviews
- Customer-service chat transcripts
- Email complaints
- Product descriptions
- Supplier information
- Delivery and logistics data
- Product defect records
- Historical return decisions

More than 10 million customer images are available, although image quality varies significantly.

### 3. Business Problem

UrbanCart wants to improve its returns process by answering questions such as:

- Is the returned product visibly damaged?
- What type of damage is present?
- Does the image appear consistent with the customer's return reason?
- Are certain products or suppliers generating unusually high return rates?
- What product issues are customers discussing most frequently?
- Can customer-service teams receive faster recommendations without automatically denying a return?

The company is considering computer vision, machine learning, NLP, and generative AI.

### 4. Constraints

The solution must account for:

- High transaction volume.
- A requirement for low-latency decisions.
- Inconsistent lighting and camera quality in customer photographs.
- Legitimate variations in product appearance.
- Potential bias against particular customer groups or devices.
- Customer disputes over return decisions.
- Limited budget for manually labeling millions of photographs.
- Need for integration with the existing e-commerce platform.
- Certain high-value returns require mandatory human inspection.

### 5. Student Tasks

Your team must:

1. Select the primary AI workload.
2. Explain what part of the problem that workload addresses.
3. Identify at least two plausible alternatives.
4. Compare supervised ML, computer vision, NLP, and generative AI where appropriate.
5. Recommend Azure services for image analysis, text analysis, or model development.
6. Propose a human-review strategy.
7. Explain how AI errors could affect customers.
8. Identify fairness and transparency concerns.
9. Recommend business and technical success metrics.
10. Explain how the solution could be scaled from a pilot to millions of return transactions.

### 6. Expected Learning Outcome

Students should demonstrate understanding of:

- Computer vision workloads
- Image classification and image analysis
- Machine-learning classification
- NLP and sentiment/opinion analysis
- AI-assisted decision making
- Evaluation metrics
- Fairness and customer-impact considerations

Azure Vision provides image analysis capabilities including image tagging, image captions, and OCR, while Azure Language capabilities can analyze text such as customer reviews and opinions.

---

# Scenario 3 — Smart City / Government
## CityConnect: Intelligent Municipal Service Management

### 1. Background

CityConnect is a municipal government platform used by citizens to report problems such as potholes, overflowing waste bins, broken streetlights, illegal dumping, damaged road signs, water leakage, and traffic-related issues.

The city receives approximately 8,000 citizen complaints every day through a mobile application, telephone call center, website, email, and social media. Citizens may submit text descriptions, photographs, videos, or voice messages. Complaints are currently classified manually before being forwarded to different municipal departments.

The city is planning to introduce AI to reduce complaint-processing time and improve prioritization. However, city officials want to avoid a system that automatically determines public-service priorities without considering human oversight, local policy, or safety requirements.

### 2. Available Data

Available data includes:

- Citizen text complaints
- Photographs
- Short videos
- Voice recordings
- Call-center transcripts
- GPS coordinates
- Historical complaints
- Municipal work orders
- Repair completion records
- Weather information
- Traffic information
- IoT sensor data from selected locations
- Department and service-category information
- Historical response times

Citizen reports are received in English as well as several Indian regional languages.

### 3. Business Problem

The city wants to build an AI-assisted service management solution that can:

- Identify the type of municipal issue.
- Extract location and other relevant information.
- Combine citizen reports with sensor information.
- Identify duplicate reports.
- Detect potentially urgent public-safety issues.
- Route requests to appropriate departments.
- Provide citizens with status information through a conversational interface.
- Translate or understand multilingual citizen reports.

A single complaint may contain text, an image, a voice message, and geographic information.

### 4. Constraints

The solution must consider:

- Very high daily request volumes.
- Multiple languages.
- Low tolerance for misclassifying safety-related issues.
- Citizen privacy.
- Potential bias related to neighborhoods or demographic groups.
- Need for explainable routing rules.
- Limited municipal technology budgets.
- Need for near-real-time processing in certain cases.
- Poor-quality mobile photographs and audio.
- Public accountability for AI-assisted decisions.

### 5. Student Tasks

Your team must:

1. Identify the primary AI workload.
2. Determine whether one workload is sufficient or whether a combination is required.
3. Identify the primary workload and justify why it should lead the solution architecture.
4. Compare conversational AI, computer vision, NLP, speech AI, and machine learning.
5. Recommend appropriate Azure AI capabilities.
6. Explain how multilingual input should be handled.
7. Discuss how duplicate complaints or contradictory reports might be addressed.
8. Identify Responsible AI risks related to public-sector decision making.
9. Define success metrics for both citizens and municipal departments.
10. Explain which decisions should remain under human control.

### 6. Expected Learning Outcome

Students should demonstrate:

- Multimodal AI workload analysis
- Conversational AI concepts
- Speech-to-text
- NLP classification
- Computer vision
- Machine-learning-based prioritization
- Multilingual AI considerations
- Public-sector Responsible AI

Azure Speech supports speech-to-text, text-to-speech, speech translation, and live voice experiences; Azure Speech can also be used in applications operating at the cloud or edge.

---

# Scenario 4 — Banking & Financial Services
## Horizon Bank: SME Loan Application Risk Assessment

### 1. Background

Horizon Bank operates a digital lending platform for small and medium-sized businesses. SME customers submit loan applications containing financial statements, tax documents, bank statements, identity documents, business registration documents, invoices, and other supporting evidence.

Loan officers currently spend significant time reviewing these documents and verifying information against historical records. A second team performs risk analysis using financial ratios, transaction history, credit history, and business characteristics.

The bank wants to reduce loan-processing time while maintaining strong controls around credit risk and regulatory compliance. Management is considering an AI-based pre-screening system that could identify potentially high-risk applications and recommend which cases should receive additional review.

The bank is particularly concerned about fairness. An AI system that produces systematically different outcomes for certain groups of applicants could create significant regulatory and reputational risk.

### 2. Available Data

The bank has:

- Historical loan applications
- Loan approval and rejection records
- Financial statements
- Bank statements
- Tax documents
- Business registration documents
- Customer demographic information
- Credit history
- Transaction histories
- Repayment history
- Loan default information
- Customer-service conversations
- Loan officer notes

Some documents are digital, while others are scanned PDFs or images.

### 3. Business Problem

Horizon Bank wants an AI-assisted loan assessment solution that can:

- Extract financial information from documents.
- Identify missing or inconsistent information.
- Estimate credit risk.
- Prioritize applications for human review.
- Reduce manual processing.
- Provide explanations or supporting evidence for risk indicators.
- Detect potentially fraudulent or suspicious documentation.

The bank has not decided whether the central solution should be machine learning, document intelligence, NLP, or a combination.

### 4. Constraints

Consider the following:

- Financial services are a high-impact application area.
- Decisions must be auditable.
- Sensitive customer data must be protected.
- Historical decisions may contain bias.
- False positives can delay legitimate businesses.
- False negatives can increase financial losses.
- The bank has strict security requirements.
- The system must support high transaction volumes.
- A pilot is expected within six months.
- Fully autonomous loan approval is not permitted during the initial phase.

### 5. Student Tasks

Your team must:

1. Select the primary AI workload.
2. Identify supporting workloads that could operate alongside it.
3. Explain the difference between information extraction and predictive machine learning in this scenario.
4. Compare generative AI with traditional ML approaches.
5. Recommend suitable Azure services.
6. Explain what data should and should not be used as model features.
7. Propose fairness and bias evaluation techniques.
8. Identify privacy and security risks.
9. Explain how human oversight should be incorporated.
10. Define business, model-performance, and Responsible AI metrics.

### 6. Expected Learning Outcome

Students should demonstrate understanding of:

- Predictive machine learning
- Classification
- Document intelligence
- Information extraction
- Feature selection
- Model evaluation
- Fairness
- Explainability and transparency
- Privacy and accountability

Azure Machine Learning supports the ML lifecycle including model development, deployment, monitoring, and MLOps, making it appropriate for student discussion around operationalizing predictive ML models.

Microsoft's Responsible AI guidance identifies fairness, reliability and safety, privacy and security, inclusiveness, transparency, and accountability as core principles.

---

# Scenario 5 — Manufacturing
## Apex Manufacturing: Predictive Maintenance and Quality Assurance

### 1. Background

Apex Manufacturing operates several factories producing precision-engineered automotive components. Production lines contain automated presses, CNC machines, robotic arms, conveyor systems, and inspection stations.

Unexpected equipment failures currently result in production downtime, missed delivery commitments, overtime costs, and expensive emergency maintenance. The organization currently performs preventive maintenance on fixed schedules, but engineers believe many failures could be predicted earlier.

At the same time, the quality team uses cameras to inspect finished components. Maintenance engineers also record observations in free-text maintenance logs and sometimes leave voice notes after troubleshooting equipment.

The company wants to explore AI, but its engineering leadership does not want to deploy a complex solution unless there is measurable evidence that AI can reduce downtime and improve maintenance decisions.

### 2. Available Data

The organization has:

- Machine temperature readings
- Vibration measurements
- Pressure readings
- Motor current
- Acoustic sensor data
- Equipment operating hours
- Historical breakdown events
- Maintenance schedules
- Maintenance records
- Engineer notes
- Photographs of defective components
- Production-line camera images
- Production speed
- Environmental data
- Quality inspection results

Some equipment provides sensor readings every second, while other machines produce data only every few minutes.

### 3. Business Problem

Apex wants to determine whether AI can:

- Predict equipment failure before it happens.
- Identify abnormal operating conditions.
- Estimate remaining useful life of equipment.
- Detect visual defects in manufactured components.
- Summarize maintenance information for engineers.
- Identify recurring causes of equipment failure.

Management initially proposes building “one AI model that detects everything.”

The engineering team is not convinced that a single AI workload is appropriate.

### 4. Constraints

The team must consider:

- Production systems cannot be interrupted for experimentation.
- False alarms create unnecessary maintenance costs.
- Missed failures can cause substantial financial losses.
- Some machines generate huge volumes of sensor data.
- Equipment from different vendors produces different data formats.
- Camera conditions vary across production lines.
- Certain AI workloads may need edge processing.
- Maintenance engineers need understandable alerts.
- The project budget supports only a limited pilot.

### 5. Student Tasks

Your team must:

1. Select the primary AI workload for predictive maintenance.
2. Determine whether other AI workloads should be secondary components.
3. Compare machine learning, computer vision, speech AI, and generative AI.
4. Explain what type of ML problem is involved.
5. Recommend suitable Azure AI/Azure ML capabilities.
6. Explain how training data should be labeled.
7. Define appropriate performance metrics.
8. Discuss false positives and false negatives.
9. Consider whether cloud, edge, or hybrid processing would be appropriate.
10. Develop a Responsible AI and operational-risk checklist.

### 6. Expected Learning Outcome

Students should demonstrate:

- Machine-learning workload identification
- Classification, regression, anomaly detection, or time-series reasoning
- Computer vision concepts
- Data preparation and feature selection
- Model evaluation
- Predictive maintenance concepts
- Scalability
- Reliability and safety

Azure Machine Learning provides capabilities for training, deploying, monitoring, and managing ML models and MLOps workflows.

---

# Scenario 6 — Education
## LearnSphere University: AI-Assisted Student Success and Academic Support

### 1. Background

LearnSphere University has approximately 35,000 undergraduate students across engineering, business, arts, science, and management programs. Student performance is currently monitored through examination results, attendance, Learning Management System activity, assignment submissions, and faculty observations.

Academic advisors are responsible for identifying students who may require additional support. However, each advisor may be responsible for hundreds of students, making it difficult to identify changes in student engagement early.

The university is considering an AI-based student-support platform. The proposed system could identify students who may need assistance, answer common academic questions, summarize relevant policies, and help advisors prepare for student meetings.

Faculty members support the idea but are concerned that AI could incorrectly label students, generate inappropriate recommendations, or create privacy concerns.

### 2. Available Data

LearnSphere has:

- Student demographic information
- Course enrollment information
- Attendance records
- Examination results
- Assignment scores
- LMS activity
- Assignment submission history
- Academic policy documents
- Course handbooks
- Student emails
- Student support conversations
- Faculty notes
- Recorded lectures
- Student feedback surveys
- Historical graduation and withdrawal records

The university also has thousands of pages of policies, procedures, FAQs, and academic regulations.

### 3. Business Problem

The university wants an AI-enabled student support system that can:

- Identify students who may benefit from academic support.
- Help advisors understand student engagement patterns.
- Answer questions about academic policies and procedures.
- Summarize long policy documents.
- Assist faculty in preparing student-support meetings.
- Provide students with conversational access to approved university information.

The university is debating whether the central approach should be predictive machine learning, generative AI, knowledge mining, NLP, or a combination.

### 4. Constraints

The solution must address:

- Student privacy and sensitive personal information.
- Risk of labeling students incorrectly.
- Differences in student access to technology.
- Multilingual student populations.
- Need for reliable policy answers.
- Requirement that academic decisions remain with authorized staff.
- Risk of generative AI producing incorrect information.
- High volume during registration and examination periods.
- Limited IT resources.
- Need for clear escalation when a student's issue requires human intervention.

### 5. Student Tasks

Your team must:

1. Identify the primary AI workload.
2. Identify which workload should be used for predictive student-support insights.
3. Identify which workload could support a university knowledge assistant.
4. Explain why the organization should not necessarily use generative AI for every requirement.
5. Recommend Azure AI services.
6. Explain how university documents should be searched and grounded.
7. Identify privacy, fairness, inclusiveness, transparency, and accountability risks.
8. Recommend human-escalation mechanisms.
9. Define technical and business success metrics.
10. Explain how the university could evaluate the system before allowing broad student access.

### 6. Expected Learning Outcome

Students should demonstrate understanding of:

- Predictive machine learning
- NLP
- Generative AI
- Knowledge mining
- Search and retrieval
- Conversational AI
- Grounded AI responses
- Human oversight
- Responsible AI in education

Azure AI Search supports full-text, vector, hybrid, and multimodal retrieval and can enrich and structure enterprise content for search and AI scenarios.

Microsoft Foundry provides access to generative AI models and capabilities for building AI applications and agents, while Foundry Agent Service supports managed agent development and deployment.

---

# Common Student Deliverables

Each team must submit the following for its assigned case study.

## Deliverable 1 — Problem Analysis
**Length:** Approximately 1 page

Include:

- Business context
- Key stakeholders
- Current process
- Core business problem
- AI opportunity
- Major constraints

---

## Deliverable 2 — AI Workload Selection

Identify:

**Primary AI workload:**  
____________________________________

**Supporting AI workloads:**  
____________________________________

Provide a concise explanation of why the selected workload is appropriate.

---

## Deliverable 3 — Azure Services Recommendation

Create a table similar to the following:

| Business Requirement | AI Workload | Azure Service / Capability | Purpose |
|---|---|---|---|
| Requirement 1 | | | |
| Requirement 2 | | | |
| Requirement 3 | | | |
| Requirement 4 | | | |

Students should distinguish between the **AI workload** and the **Azure service used to implement it**.

---

## Deliverable 4 — Solution Justification

Your team must explain:

- Why your selected workload fits the problem.
- Why alternative workloads are less suitable as the primary approach.
- What trade-offs exist.
- What assumptions your solution makes.
- What additional information would be required before implementation.
- Which part of the solution should remain human-controlled.

---

## Deliverable 5 — Responsible AI Review

Evaluate your proposed solution against:

| Responsible AI Principle | Key Question |
|---|---|
| Fairness | Could the system systematically disadvantage a particular group? |
| Reliability & Safety | What happens when the AI is wrong? |
| Privacy & Security | What sensitive data is involved? |
| Inclusiveness | Can different users access and benefit from the system? |
| Transparency | Can users understand how AI is being used? |
| Accountability | Who owns the final decision? |

Microsoft's current Responsible AI guidance uses these six principles as a foundation for trustworthy AI design.

---

## Deliverable 6 — Success Measurement

Define at least **five measurable success criteria**.

Your metrics should include a combination of:

### Business Metrics
Examples:

- Processing time
- Cost reduction
- Customer satisfaction
- Operational efficiency
- Revenue impact

### AI Metrics
Examples:

- Accuracy
- Precision
- Recall
- F1 score
- False-positive rate
- False-negative rate
- Extraction accuracy
- Response relevance

### Responsible AI Metrics
Examples:

- Error rates across user groups
- Human escalation rate
- Privacy incidents
- Unsupported AI responses
- User-reported issues

---

# Presentation Requirement

Each team must deliver a **5–7 slide presentation**.

### Recommended Slide Structure

**Slide 1 — Business Problem**

Organization, stakeholders, current challenges, and business objective.

**Slide 2 — Data & AI Opportunity**

Available data and the AI opportunities identified by the team.

**Slide 3 — AI Workload Selection**

Primary workload and supporting workloads.

**Slide 4 — Azure Solution**

Recommended Azure services and high-level architecture.

**Slide 5 — Alternatives & Trade-offs**

Alternative approaches considered and why they were not selected as the primary approach.

**Slide 6 — Responsible AI**

Key risks, mitigations, and human oversight.

**Slide 7 — Success Measures**

Business, technical, and Responsible AI metrics.

---

# Team Discussion Questions

Before finalizing the solution, teams should discuss:

1. What is the **real business problem**, rather than simply the available data?
2. What would happen if the AI system were wrong?
3. Is AI actually required for every part of the proposed solution?
4. Could a simpler rule-based solution solve part of the problem?
5. Which AI workload provides the greatest business value?
6. What alternative workload could reasonably be selected?
7. What information is missing from the case?
8. Where must a human remain in control?
9. What data could create bias?
10. How would you prove that the solution is successful?

---
