# Medical Triage & Medication Guidance System

AI-assisted clinical decision support framework using structured prompt engineering, probabilistic symptom analysis, and medication safety validation.

---

## Overview

The **Medical Triage & Medication Guidance System** is a structured AI framework designed to improve the safety and reliability of AI-driven healthcare assistance.

The system focuses on:

- Symptom intake and extraction
- Differential diagnosis ranking
- Emergency escalation detection
- Medication recommendation safety
- Drug interaction validation
- Longitudinal symptom tracking
- Transparency and auditability

Unlike traditional symptom checkers, this architecture emphasizes structured reasoning, uncertainty handling, and safety-first clinical guidance.

---

## Key Features

### Structured Symptom Intake

The system extracts and stores:

- Age
- Sex
- Pregnancy status (if applicable)
- Weight / height
- Symptoms
- Severity and progression
- Allergies
- Current medications
- Pre-existing conditions
- Medication history

---

### Differential Diagnosis Engine

Uses weighted symptom analysis to generate:

- Ranked probable conditions
- Confidence levels
- Probability estimates
- Dynamic re-ranking after clarification questions

Supports Bayesian-style reasoning logic for future upgrades.

---

### Severity Classification System

Conditions are classified into four triage danger levels:

| Level | Classification | Recommendation |
|---|---|---|
| 1 | Green | Rest at home |
| 2 | Yellow | Visit pharmacy |
| 3 | Orange | Visit doctor immediately |
| 4 | Red | Emergency room required |

Severity considers:

- Red flag symptoms
- Age risk factors
- Comorbidities
- Drug interactions
- Symptom duration
- Immunocompromised states

---

### Emergency Override Logic

Automatically escalates emergency situations including:

- Chest pain with shortness of breath
- Severe abdominal pain
- Neurological deficits
- Anaphylaxis symptoms
- Severe dehydration
- Suicidal ideation
- Uncontrolled bleeding
- Loss of consciousness

---

### Medication Recommendation System

For each medication recommendation, the system checks:

- Drug allergies
- Drug-drug interactions
- Contraindications
- Duplicate therapeutic classes
- Age restrictions
- Pregnancy risks
- Renal/hepatic impairment adjustments

Interaction severity is categorized as:

- Minor
- Moderate
- Major
- Contraindicated

---

### Side Effect Monitoring

The system tracks reported side effects and:

- Compares them against known reactions
- Detects allergic response patterns
- Reclassifies danger levels if necessary
- Escalates care recommendations

---

### Auditability & Transparency

The architecture maintains:

- Structured JSON records
- Historical symptom logs
- Medication version tracking
- Diagnostic reasoning traces
- Future compatibility with probabilistic engines

---

## System Architecture

Main subsystems include:

1. Input Processing Engine  
2. Structured Data Storage  
3. Symptom Weighting Module  
4. Differential Diagnosis Engine  
5. Diagnostic Narrowing System  
6. Severity Classification Engine  
7. Medication Recommendation System  
8. Drug Interaction Analyzer  
9. Side Effect Monitoring Module  
10. Audit & Transparency Layer  

---

## Workflow

```text
User Input
   ↓
Structured Data Extraction
   ↓
Symptom Weighting
   ↓
Differential Diagnosis Generation
   ↓
Clarifying Questions
   ↓
Severity Classification
   ↓
Medication Recommendation
   ↓
Drug Interaction Analysis
   ↓
Safety Validation & Logging
```

---

## JSON Data Structure Example

```json
{
  "user_id": "",
  "probable_condition": "",
  "confidence_score": "",
  "danger_level": "",
  "medications": [
    {
      "identifiers": {
        "generic_name": "",
        "brand_name": "",
        "rxnorm_id": "",
        "class": ""
      }
    }
  ],
  "timestamp": ""
}
```

---

## Research Findings

Comparative testing against California pharmacy graduate students showed:

| Metric | AI System | Pharmacy Graduates |
|---|---|---|
| Cases Correctly Diagnosed | 23 | 27 |
| Primary Drug Accuracy | High | High |
| Secondary Drug Accuracy | Moderate | High |
| Contraindication Handling | Moderate | High |
| User Safety Reliability | Moderate | High |

### Key Observation

The AI system performed well with first-line medication suggestions but reliability decreased with secondary and tertiary recommendations due to:

- Missed contraindications
- Duplicate therapeutic classes
- Drug interaction risks
- Long-term prescribing considerations

This highlighted the importance of maintaining physician and pharmacist oversight.

---

## Future Work

Planned improvements include:

- Bayesian probability engines
- EHR integration
- Real-time pharmaceutical APIs
- Voice-enabled intake systems
- Expanded clinical validation studies

---

## Safety Disclaimer

This system is intended for:

- Educational research
- AI safety experimentation
- Clinical decision-support research

It is **not** a replacement for:

- Licensed physicians
- Emergency services
- Pharmacists
- Professional medical diagnosis

The system should always encourage professional medical consultation when uncertainty or elevated risk exists.

---

## Technologies & Concepts

- Large Language Models (LLMs)
- Structured Prompt Engineering
- Probabilistic Reasoning
- Clinical Decision Support
- Medication Safety Logic
- JSON-Based State Management
- Bayesian Diagnostic Concepts

---

## Author

**Gordon Wray Undergraduate Research**  
May 2026

---

## References

1. Eric Topol — *Deep Medicine: How Artificial Intelligence Can Make Healthcare Human Again*  
2. Esteva et al. — *A Guide to Deep Learning in Healthcare*  
3. Rajkomar, Dean, Kohane — *Machine Learning in Medicine*  
4. World Health Organization — *Ethics and Governance of AI for Health*  
5. FDA — *Clinical Decision Support Software Guidance*  
