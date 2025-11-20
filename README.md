#  Telecom Service Process Mining & AI Redesign

![R](https://img.shields.io/badge/R-276DC3?logo=r&logoColor=white)
![BPMN](https://img.shields.io/badge/BPMN-Modeling-blue)
![Process Mining](https://img.shields.io/badge/Process%20Mining-bupaR-orange)

This repository contains an end-to-end analysis and redesign of a Nordic telecom provider’s enterprise customer service process.  
The project combines **process mining**, **BPMN modeling**, **agent performance analysis**, and an **AI-driven redesign**.

> This work was completed as part of the *Systems and Process Innovation* course during the **first semester of my Master’s degree in Business Analytics at NMBU (Autumn 2023)**.

---

## 🔍 1. Project Summary

The objective of this project was to evaluate and improve the company’s customer service operations by:

- Mapping the **current “as-is” process** using event logs  
- Identifying inefficiencies, bottlenecks, and performance variation  
- Understanding agent workload, throughput times, and topic complexity  
- Designing a future **AI-enabled “to-be” workflow**  
- Recommending organizational, operational, and technological changes

The dataset consists of anonymized customer service event logs containing three activity types:  
**Email, Interaction, End.**

---

## 📊 2. Key Insights

### Process Mining Findings
- **30.9% of cases** exceeded the 100-hour SLA threshold  
- **67 unique process variants**, indicating high inconsistency  
- Emails showed extreme duration variation (max **558 hours**)  
- Significant workload imbalance across agents  
- Certain case topics (esp. **9** and **10**) were far more complex  
- Process capability charts revealed **17 outliers** and **62 pattern breaches**  

## 🗺️ 3. Selected Project Visualizations

### **As-Is Process Map**  
A full representation of all activities and transitions in the customer service workflow.  
<img width="650" alt="As-Is Process Map" src="https://github.com/user-attachments/assets/f51e7d44-88fd-4901-b844-9c2c701825ec" />

### **As-Is BPMN Model**  
Shows the current customer journey from incident reporting to case closure, including both customer and agent workflows.  
<img width="650" alt="As-Is BPMN" src="https://github.com/user-attachments/assets/a66df60c-b7c1-4fe6-a4e9-ca12bbee487d" />

---

### **Variant Analysis – Distribution of Variants**  
Illustrates the high variability across 67 process paths.  
<img width="650" alt="Variant Distribution" src="https://github.com/user-attachments/assets/007ce035-631f-4538-9b2e-ecbd7b09b243" />

### **Variant Analysis – Trace Frequency**  
Displays the most common case pathways, covering ~60 percent of all cases.  
<img width="650" alt="Trace Frequency" src="https://github.com/user-attachments/assets/103d9167-3659-4620-b3d9-60a76df51b77" />

---

### **Case Duration Distribution**  
Histogram of case durations with a visible spike above the 100-hour SLA threshold.  
<img width="650" alt="Case Duration Histogram" src="https://github.com/user-attachments/assets/c092afb7-f657-4bab-a96c-69114287f726" />

### **Average Throughput Time by Agent**  
Highlights significant variation across service agents.  
<img width="650" alt="Agent Throughput Times" src="https://github.com/user-attachments/assets/5e2f7d7b-e82d-4deb-9a21-08813ec01831" />

---

### **Cases per Topic by Agent**  
Shows workload distribution across case topics.  
<img width="650" alt="Cases per Topic by Agent" src="https://github.com/user-attachments/assets/e1387f28-1d59-4e19-96d0-6813fe3d1850" />

### **Process Control Chart**  
17 points exceed control limits and several runs break randomness assumptions.  
<img width="650" alt="Process Control Chart" src="https://github.com/user-attachments/assets/30e387b5-ce4c-47f2-a0f3-fbf5301616ad" />

### **Process Capability Analysis**  
Shows that ~21 percent of cases exceed the 100-hour SLA.  
<img width="650" alt="Process Capability" src="https://github.com/user-attachments/assets/c25eb505-113b-4136-b6b9-c8d2c6206cdf" />

---

### **To-Be BPMN Model**  
Illustrates AI-assisted classification, mandatory documentation, predictive routing and automated updates.  
<img width="650" alt="To-Be BPMN Model" src="https://github.com/user-attachments/assets/944140f8-f90a-4944-9054-fe5aac988e24" /> 

---

## ⚙️ 4. Methods & Tools

### 🔵 Process Mining in R
Libraries used:
- `bupaR`
- `edeaR`
- `processmapR`
- `qcc`
- `tidyverse`

Key analytical steps:
- Event log creation and cleaning  
- Process map generation  
- Variant and trace frequency analysis  
- Throughput and SLA evaluation  
- Resource and agent workload analysis  
- Control chart creation  
- Complexity scoring by topic    

### 🟣 BPMN Modeling
Two models were created:
- **As-Is model:** current workflow and bottlenecks  
- **To-Be model:** redesigned AI-enabled process  

---

## 🤖 5. Proposed AI-Driven Redesign

The new process design integrates Salesforce Einstein AI to support:

### 1. Automatic Case Classification & Routing  
Predicts case type and assigns it to the optimal agent.

### 2. Mandatory Document Submission  
Ensures complete case information at the start.

### 3. Predictive Workload Distribution  
Balances workload and avoids overloading key agents.

### 4. Specialized Agent Training  
Ensures agents can handle complex case types more efficiently.

### 5. AI-Driven Communication  
Automated updates, sentiment analysis and simple-case resolution.

---

## 📈 6. Implementation Strategy

The project includes recommendations for:

- **Agile implementation methodology**  
- **Governance structure** with RACI and BPM standards  
- **8-month project timeline**  
- **Risk analysis** (technical, organizational and ethical)  
- **Change management and user adoption strategies**  
