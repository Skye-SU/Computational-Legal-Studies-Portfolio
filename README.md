# ⚖️ Computational Legal Studies: Quantifying the "Gap of Justice"
### A Comparative Analysis of Matrimonial Property Division (UK vs. China)

> **Project Status:** 🟢 Active (Capstone Extension)
> **Domain:** Computational Social Science, Family Law, NLP
> **Tech Stack:** Python, spaCy, Pandas, WordCloud, Regex

## 📖 Project Background
This repository serves as the **computational extension** of my Master's thesis: *"The Impact of Chinese and British Marital Property Division Mechanism on Chinese Women's Post-divorce Economic Security"*.

While my thesis used **Grounded Theory** to qualitatively diagnose the "Formal Equality Trap" in Chinese divorce settlements, this project aims to **quantitatively verify** these findings using Natural Language Processing (NLP). By analyzing 100+ judicial documents from Shanghai and the UK, I aim to visualize the divergence between the UK's *"Needs-Based"* dynamic fairness and China's *"Property-Focused"* formal equality.

## 📊 Key Findings (Notebook 01)
The linguistic landscape of judgments reveals a systemic difference in judicial focus:

| **UK Judgments: "Human-Centric"** | **China Judgments: "Asset-Centric"** |
|:---------------------------------:|:-----------------------------------:|
| ![UK WordCloud](assets/wordcloud_uk.png) | ![China WordCloud](assets/wordcloud_cn.png) |
| Dominance of **"Child"**, **"Needs"**, **"Care"**. Reflects the *Welfare Principle* and *Dynamic Fairness*. | Dominance of **"Property" (房产)**, **"Payment" (支付)**. Reflects the *Formal Equality Trap* and transactional focus. |

## 📂 Portfolio Roadmap
This portfolio demonstrates a progressive pipeline from raw legal text to policy insight, mirroring the **"System-Technology-Culture"** reconstruction model proposed in my thesis.

- [x] **01. Legal Text Mining & Visualization** ([View Notebook](notebooks/01_legal_text_processing.ipynb))
    - **Objective:** Build an ETL pipeline for heterogeneous legal data (HTML/PDF) and visualize judicial focus.
    - **Tech Highlights:**
        - **Polite Scraper:** Ethical data collection from BAILII with rate limiting.
        - **Dual-Language NLP:** Custom cleaning pipelines for English (HTML) and Chinese (PDF) texts.
        - **Taxonomy Analysis:** Mapping keywords to the "Three Pillars" (Needs, Compensation, Sharing).
    - **Insight:** Quantitatively confirmed the lack of "Needs" language in Chinese judgments.

- [ ] **02. NER & Information Extraction** (Coming Soon)
    - **Objective:** Train spaCy/Transformers to extract financial values (e.g., Housing Value vs. Compensation Award).
    - **Goal:** To calculate the "Compensation Deficit" for non-economic contributions.

- [ ] **03. Citation Network Analysis** (Planned)
    - **Objective:** Map the influence of landmark cases like *White v White* using NetworkX.

## 🛠️ Installation & Reproduction
To reproduce the analysis in Notebook 01:

1. **Clone the repo:**
   ```bash
   git clone https://github.com/Skye-SU/Computational-Legal-Studies-Portfolio.git

2. **Run the notebook:**
   ```bash
   jupyter notebook notebooks/01_legal_text_processing.ipynb

3. **Install dependencies:Bashpip install -r requirements.txt**
   ```bash
   python -m spacy download en_core_web_sm
   python -m spacy download zh_core_web_sm

## 👩‍💻 About the Author
I am a Master's graduate in Social Policy (Lingnan University) with a background in qualitative research. This project represents my pivot into Computational Law, aiming to leverage AI and data agents to:

1. Reduce the "drudgery" of legal research.
2. Provide empirical evidence to support substantive justice reforms.
3. Bridge the gap between legal theory and technical implementation.

Note: Raw case data (PDFs) is not included in this repository to comply with privacy regulations and copyright terms. Processed datasets are available upon request for academic verification.
