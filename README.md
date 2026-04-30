# Causal Diagnosis Agent

A multi-source causal inference agent for root cause analysis and automated intervention with closed-loop validation.

---

## 🚀 Overview

This project implements a **cross-system causal diagnosis agent** designed to:

- Detect anomalies from multi-source data
- Identify root causes using causal inference
- Automatically execute interventions
- Validate outcomes through a closed-loop system

Unlike traditional monitoring or analytics tools, this system provides:
> **Diagnosis + Decision + Execution + Validation**

---

## 🧠 Core Capabilities

- Multi-source data fusion (logs, metrics, events)
- Causal graph modeling
- Difference-based attribution (before vs after)
- Counterfactual reasoning (what-if simulation)
- Automated intervention execution
- Self-evaluation and re-planning

---

## 🏗️ System Architecture
            ┌──────────────────────────┐
            │     Multi-Source Data    │
            │ Logs / Metrics / Events  │
            └────────────┬─────────────┘
                         │
                         ▼
            ┌──────────────────────────┐
            │   Data Alignment Layer   │
            │ Time Sync + Cleaning     │
            └────────────┬─────────────┘
                         │
                         ▼
            ┌──────────────────────────┐
            │   Causal Modeling Layer  │
            │ Causal Graph + Sequences │
            └────────────┬─────────────┘
                         │
                         ▼
            ┌──────────────────────────┐
            │  Reasoning Engine        │
            │ Diff + Causal Inference  │
            └────────────┬─────────────┘
                         │
                         ▼
            ┌──────────────────────────┐
            │ Decision & Intervention  │
            │ API / Rollback / Adjust  │
            └────────────┬─────────────┘
                         │
                         ▼
            ┌──────────────────────────┐
            │ Validation Layer         │
            │ Counterfactual + Metrics │
            └────────────┬─────────────┘
                         │
                         ▼
            ┌──────────────────────────┐
            │ Memory & Feedback        │
            │ Learning + Replanning    │
            └──────────────────────────┘
            
---

## 🔄 Execution Flow

1. **Anomaly Detection**
   - Triggered by abnormal metrics (conversion drop, error spike)

2. **Data Fusion**
   - Align logs, metrics, and events into a unified timeline

3. **Difference Attribution**
   - Compare before/after states to identify candidate changes

4. **Causal Inference**
   - Evaluate which changes actually caused the anomaly

5. **Intervention Decision**
   - Select minimal-risk action (rollback, adjust config, switch API)

6. **Execution**
   - Perform action via API or generate human approval task

7. **Validation**
   - Use counterfactual reasoning + real metrics to verify effectiveness

8. **Replanning (if needed)**
   - If failed, select alternative strategy

---

## ⚙️ Tech Highlights

### 1. Causal vs Correlation
This system distinguishes:
- Correlation → observed relationship
- Causation → validated impact through intervention

### 2. Multi-step Reasoning
Pipeline:

### 3. Closed-loop System
- Not just analysis
- Executes and verifies outcomes automatically

### 4. Graph-based Modeling
- System dependencies modeled as causal graphs
- Enables structured reasoning instead of flat analysis

---

## 📊 Metrics

| Metric | Description |
|------|------------|
| MTTR | Mean time to resolve anomaly |
| Accuracy | Root cause identification accuracy |
| Incident Impact | Reduction in affected users |
| Intervention Success Rate | % of successful automated fixes |

---

## 🧪 Demo

Run locally:

```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
.
├── api.py
├── streamlit_app.py
├── src/
│   └── causal_agent/
│       ├── model.py
│       ├── reasoning.py
│       ├── intervention.py
│       └── validator.py
├── samples/
├── tests/
└── README.md
