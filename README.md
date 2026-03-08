# Encare Synthetic Data Hackathon 2026

## Overview

The goal of this hackathon is to generate **high-quality synthetic medical records** that preserve the **statistical and clinical characteristics** of the provided dataset while containing **no real patient data**.

---

## Table of Contents

- [How It Works](#how-it-works)
- [Rules](#rules)
- [Quick Start](#quick-start)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Validation](#validation)
- [Submission](#submission)

---

# How It Works

1. Each team can make a fork of this **repository** as a base to work from.
2. Feel free to use any method you like to generate synthetic medical records. Original and creative ideas are highly encouraged!
3. Save your generated dataset in the `/results` folder.
4. **Submit the synthetic dataset** each as many times as you want. The submissions will be tested once a day in a batch job.
5. After deadline, each repostitory should be **made public** to be able to win.

---

# Rules

- Do **not** share the original dataset outside of the hackathon.
- Do **not** modify the original dataset.
- You may use **any libraries, tools, or AI assistants**.
- The generated dataset must be **reproducible from the code in your repo**.
- Generated data should preserve **statistical realism** while avoiding **patient-level replication**.

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
├── approaches/
│   └── a placeholder approach
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

The repository includes validation tools to check generated datasets. These are only intended as **basic checks** and does not garuantee a high score .

### Statistical validation
- Kolmogorov–Smirnov (KS) tests
- Distribution comparisons

### Clinical validation
- Rule-based plausibility checks

---

# Submission

Your submission is **only the generated synthetic dataset**.

Save your synthetic output in:

```
/results/
```

After the submission deadline, all repositories will be **made public**.