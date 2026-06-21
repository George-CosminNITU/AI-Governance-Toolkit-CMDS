# AI Risk Assessment Methodology

**Version:** 1.0  
**Phase:** Year 1, Semester 2 Deliverable  

## 1. Overview
The AI Risk Assessment Methodology provides a structured approach to identifying, evaluating, and mitigating the risks associated with the deployment of Generative AI tools within the corporate environment. This methodology serves as the theoretical foundation for the Risk Assessment Matrix (planned for Year 2) and aligns with the NIST AI Risk Management Framework (AI RMF).

## 2. Core Risk Categories
When evaluating a new AI tool or a specific corporate use case, the assessment must address the following primary challenges inherent to AI systems:

### 2.1. Data Privacy and Security
* **The Risk:** Employees may inadvertently share sensitive corporate information, proprietary source code, or customer Personally Identifiable Information (PII) with public AI tools ("Shadow AI"), leading to data breaches and regulatory non-compliance.
* **Assessment Criteria:** Evaluation of the vendor's Terms of Service (ToS). Does the vendor use inputs for model training? Is there a zero-day retention policy available (e.g., Enterprise tiers)?

### 2.2. Bias and Fairness
* **The Risk:** Generative AI models are trained on vast datasets that may contain historical imbalances. This can result in outputs that are biased, unfair, or discriminatory, especially in sensitive areas like HR screening or customer evaluation.
* **Assessment Criteria:** Determining if the use-case involves decision-making about individuals. If so, strict Human-in-the-Loop (HITL) protocols must be enforced to override biased outputs.

### 2.3. Limited Transparency and Explainability
* **The Risk:** Many AI models function as "black boxes," meaning it is difficult to understand how they arrived at a specific conclusion or generated a specific output. This reduces trust and complicates compliance with transparency regulations.
* **Assessment Criteria:** Can the AI's output be easily verified against trusted primary sources? Does the tool provide citations or grounding for its claims?

## 3. Assessment Workflow
To operationalize this methodology, IT and Compliance teams will follow a three-step evaluation process for every AI tool requested by employees:

1. **Vendor & Tool Vetting:** 
   * Review data sovereignty (e.g., EU data residency).
   * Confirm data isolation boundaries (Consumer vs. Enterprise tier).
2. **Use-Case Evaluation:**
   * Map the proposed use case against the *Corporate AI Acceptable Use Policy (AUP)* and the *Data Classification Guide*.
   * Ensure no "Confidential" or "Tier 3" data is exposed to external cloud models.
3. **Risk Scoring (Likelihood vs. Impact):**
   * Assess the probability of a risk occurring (e.g., data leak, biased output) against the potential business impact (e.g., financial loss, GDPR fines).
   * Only tools and use cases that score within the acceptable risk appetite—or those mitigated by strict controls—are approved.

## 4. Mitigation Strategy
The primary mitigation strategy across all risk categories is the mandatory **Human-in-the-Loop (HITL)** requirement. AI tools are approved strictly as "assistants," and accountability for the accuracy, legality, and fairness of any AI-generated output remains entirely with the human user.
