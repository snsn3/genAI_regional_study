# GenAI Regional Study: LLM Bias Across Geographical Regions

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

Research code and data accompanying the study on **geographical bias and response quality** of AI-driven language models (e.g. ChatGPT) across North America, Europe, and Africa, with a focus on topics in public administration.

---

## Abstract

We investigate bias and quality of state-of-the-art AI-driven language models through a geographical lens. Using OpenAI’s ChatGPT and a diverse, non-representative sample of respondents from North America, Europe, and Africa, we assess the model’s advice on issues of public interest. The study focuses on topics such as paying taxes, Indigenous Peoples’ rights and self-determination, whistleblowing, and related themes in public administration. We apply machine-learning methods to evaluate the quality and topical orientation of ChatGPT’s responses and compare them across regions. The analysis is grounded in public administration literature and aims to support the development of region-fair conversational AI and to inform policymakers, educators, and users.

---

## Table of Contents

- [Repository structure](#repository-structure)
- [Getting started](#getting-started)
- [Data and code](#data-and-code)
- [Publication](#publication)
- [Citation](#citation)
- [Funding](#funding)
- [License](#license)

---

## Repository structure

```
genAI_regional_study/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── CITATION.cff
├── requirements.txt
│
├── GML_Lab_EN.csv                    # English responses (full)
├── GML_Lab_FR.csv                    # French responses (full)
├── gmlLab-Reponses-6-mai-2024.csv    # Combined EN + FR responses
├── FR_monthly_aggregated_data.csv    # French, aggregated by month
├── topics_GML_Lab_FR.csv             # French topic assignments
├── https-doi.org10.1007s43681-025-00906-2.pdf   # Published article (PDF)
│
├── EN_topic_model.ipynb              # Topic model, English
├── FR_topics_modelling.ipynb         # Topic model, French
└── article_code_2_analyse_descr_des_reponses.ipynb   # Descriptive analysis
```

Notebooks expect to be run from the **repository root** so that relative paths to the CSV files resolve correctly (e.g. in Jupyter, VS Code, or Google Colab after cloning).

---

## Getting started

### Requirements

- Python 3.8+
- Jupyter (optional; notebooks can be run in Colab or another environment)

### Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/snsn3/genAI_regional_study.git
   cd genAI_regional_study
   ```

2. **Create a virtual environment (recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run the notebooks**

   - Open any `.ipynb` in Jupyter, JupyterLab, or VS Code, or use the “Open in Colab” link inside each notebook.
   - Execute cells from the top; notebooks assume the working directory is the repo root (where the CSV files are).

---

## Data and code

| File | Description |
|------|-------------|
| `GML_Lab_EN.csv` | English responses (full dataset). |
| `GML_Lab_FR.csv` | French responses (full dataset). |
| `gmlLab-Reponses-6-mai-2024.csv` | All responses (English and French). |
| `FR_monthly_aggregated_data.csv` | French responses aggregated by month. |
| `topics_GML_Lab_FR.csv` | Topic labels for French responses. |
| `EN_topic_model.ipynb` | Topic modelling for English responses (LDA, TF–IDF). |
| `FR_topics_modelling.ipynb` | Topic modelling for French responses. |
| `article_code_2_analyse_descr_des_reponses.ipynb` | Descriptive analysis (response length, time series, regional comparisons). |

---

## Publication

The associated article is available as:

- **PDF** (local): `https-doi.org10.1007s43681-025-00906-2.pdf`
- **DOI**: [10.1007/s43681-025-00906-2](https://doi.org/10.1007/s43681-025-00906-2)

---

## Citation

If you use this code or data in your work, please cite the paper and this repository:

**Paper (BibTeX):**

```bibtex
@article{nzobonimpa2025regional,
  author  = {Nzobonimpa, Stany and others},
  title   = {Study on {LLMs'} Regional Bias},
  journal = {AI and Ethics},
  year    = {2025},
  doi     = {10.1007/s43681-025-00906-2}
}
```

**Code and data:**  
Stany Nzobonimpa. *genAI_regional_study*. GitHub. <https://github.com/snsn3/genAI_regional_study>.

You can also use the [CITATION.cff](CITATION.cff) file in this repository for automated citation.

---

## Funding

This doctoral research is funded by the **Social Sciences and Humanities Research Council of Canada (SSHRC)** through the [Canada Vanier Graduate Scholarships](https://vanier.gc.ca/en/home-accueil.html). Further details: [ÉNAP – Stany Nzobonimpa, lauréat Bourse Vanier 2023](https://enap.ca/nouvelles/doctorant-stany-nzobonimpa-laureat-prestigieuse-bourse-vanier-2023).

---

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
