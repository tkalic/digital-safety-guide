# 03 — Ethical AI

## AI Is Already Making Decisions About You

Credit scores. Job application screening. Loan approvals. Bail recommendations. Content moderation. Fraud detection.

AI systems are already embedded in decisions that affect people's lives in significant ways — often without those people knowing an algorithm was involved, let alone being able to challenge it. The ethics of AI isn't a future problem. It's a current one.

---

## The Bias Problem

AI systems learn from data. If the data reflects historical inequalities, the system will too — and may amplify them.

A well-documented example: a recruitment tool used by a major tech company was trained on historical hiring data, which skewed male. The system learned to penalize CVs that included the word "women's" (as in "women's chess club") and downgraded graduates of all-women's colleges. The tool was eventually scrapped, but not before it had been in use.

Bias in AI isn't always intentional. It's often invisible until someone looks for it. This is why auditing matters.

**Key issues:**
- **Training data bias** — if historical data reflects discrimination, the model will too
- **Proxy discrimination** — a model might not use race as a variable, but use zip code, which correlates strongly with race
- **Feedback loops** — a model predicting crime risk used in policing leads to more policing in certain areas, generating more crime data, reinforcing the prediction

---

## Transparency and Explainability

If an algorithm denies you a loan or a job, you should be able to find out why. In practice, this is often difficult or impossible — particularly with complex deep learning models where even the developers can't fully explain individual decisions.

The EU AI Act (which came into force in 2024) addresses this directly. High-risk AI systems — those used in hiring, credit, education, law enforcement, and critical infrastructure — are required to be transparent, explainable, and subject to human oversight.

**What explainability means in practice:**
- Users should be able to request a human review of an AI decision
- Developers should be able to identify which features drove a specific output
- Documentation should exist explaining how the model was trained and validated

---

## Privacy in AI Systems

AI systems consume enormous amounts of data. The more personal that data, the higher the risk.

**Things worth knowing:**
- Many AI tools (chatbots, image generators, writing assistants) store your inputs and may use them for further training — check the privacy policy
- Federated learning is an approach that trains models on-device without sending raw data to a central server — it's more privacy-preserving but less common
- Differential privacy adds statistical noise to datasets so individual data points can't be extracted even if the model is compromised

---

## The EU AI Act — What It Actually Says

The EU AI Act categorizes AI by risk level:

| Risk Level | Examples | Requirements |
|------------|----------|--------------|
| Unacceptable | Social scoring, real-time mass surveillance | Banned outright |
| High | Hiring tools, credit scoring, law enforcement | Strict oversight, transparency, human review |
| Limited | Chatbots, deepfakes | Disclosure requirements |
| Minimal | Spam filters, AI in games | No specific requirements |

This is the most comprehensive AI regulation passed anywhere in the world so far. If you're building or deploying AI systems in Europe — or systems used by Europeans — this applies to you.

---

## What This Means If You're Building AI

- Use diverse, representative datasets and document your data sources
- Audit your model for disparate impact across demographic groups before deployment
- Build in a mechanism for users to contest automated decisions
- Don't deploy high-stakes AI without a human review layer
