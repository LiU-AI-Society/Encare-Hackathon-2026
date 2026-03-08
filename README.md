# Encare Synthetic Data Hackathon 2026

## Overview
The goal of this hackathon is to generate **high-quality synthetic medical records** that preserve the **statistical and clinical characteristics** of the provided dataset while containing **no real patient data**.

Participants are encouraged to experiment with methods such as:

- Statistical sampling
- GANs
- Diffusion models
- LLM-based generation
- Hybrid generative pipelines

---

# Quick Start

Clone the repository:

```bash
git clone <repo-url>
cd Encare-Hackathon-2026
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Place the dataset in:

```
/data/synthetic-data-hackaton-sample.csv
```

Run the generator:

```bash
python main.py
```

Generated datasets will be saved in:

```
/results/
```

---

# Project Structure

```
Encare-Hackathon-2026
│
├── data/
│   └── synthetic-data-hackaton-sample.csv
│
├── results/
│   └── generated synthetic datasets
│
├── examples/
│   └── baseline generators (e.g. random sampler)
│
├── data_processor.py
│   Data cleaning and preprocessing
│
├── validator.py
│   Statistical and clinical validation
│
└── main.py
    Entry point for synthetic data generation
```

---

# Dataset

The dataset contains **anonymized medical records** with clinical variables.

Example categories may include:

- Demographics (age, sex)
- Diagnosis codes
- Vital signs
- Lab results
- Treatment indicators

Your goal is to generate **synthetic records with similar statistical properties**.

---

# Validation

The repository includes validation tools to check generated datasets.

### Statistical validation
- Kolmogorov–Smirnov (KS) tests
- Distribution comparisons

### Clinical validation
- Rule-based plausibility checks

⚠️ Passing these tests **does not guarantee a high score**.  
They are intended only as **basic sanity checks**.

---

# Example Baseline

A simple baseline generator is provided in:

```
/examples
```

Participants are encouraged to **build their own generators**.

---

# Submission

Your submission is **only the generated synthetic dataset**.

Save your synthetic output in:

```
/results/
```

After the submission deadline, all repositories will be **made public**.

---

# Requirements

- Python 3.9+
- pip

Recommended tools:

- Visual Studio Code
- Jupyter Notebook

---

# Notes

- Do **not modify the original dataset**.
- Generated datasets should preserve **statistical realism** while avoiding **patient-level replication**.