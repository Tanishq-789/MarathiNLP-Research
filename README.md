# Marathi Coreference Resolution Gold-Standard Dataset

This repository contains a manually curated **Gold-Standard Coreference Annotated Dataset** for the Marathi language.  
The dataset is designed to support research in **coreference resolution**, **hypergraph models**, **Marathi NLP**, and **low-resource language processing**.

---

## 📌 Overview

Marathi is a morphologically rich, low-resource language with linguistic features such as:
- **SOV sentence order**
- **Pro-drop pronouns (null subjects)**
- **Gender and number inflections**
- **Flexible word order**
- **Complex case suffixes**

These properties make coreference resolution significantly more challenging compared to English.  
This dataset provides **high-quality human annotations** to enable more accurate modeling.

---

## 📂 Dataset Contents

The repository includes:

- `processed_documents/` — Raw Marathi text documents  
- `annotated_documents/` — Gold-standard coreference annotations in JSON+CoNLL format  
- `schema.md` — Annotation guidelines and tag definitions  

---

## 🎯 Annotation Guidelines

Each document is manually annotated for:
- **Named Entities**  
- **Pronouns (explicit + pro-drop)**  
- **Nominal mentions**  
- **Hyperedges / clusters representing entity chains**  

Annotations follow:
- **Gender agreement rules**  
- **Number consistency**  
- **Semantic context checks**  
- **Cross-sentence reference tracking**

A full description of the annotation scheme is provided in `schema.md`.

---

## 🔍 Use Cases

This dataset is suitable for:

- Coreference resolution model training/testing  
- Hypergraph-based NLP research  
- Benchmarking for low-resource Indian languages  
- Linguistic analysis  
- Fine-tuning transformer models (e.g., IndicBERT, MahaBERT)

---

## 🧪 Format

Annotations are provided in:
- **JSON format** (Hypergraph-friendly structure)  
- **CoNLL-style format** (for traditional coreference models)

---

## 📊 Dataset Statistics

- Total Documents: **X**  
- Total Mentions: **X**  
- Coreference Chains: **X**  
- Avg. Mentions per Doc: **X**

*(Fill these once your stats are finalized)*

---

## 📜 License

This dataset is released under the **CC BY-NC 4.0 License**  
(Non-commercial research usage permitted.)

---

## 🤝 Contributions

If you wish to add more annotations or help expand this corpus, feel free to open an issue or submit a pull request.

---

## 📧 Contact

For questions, collaboration, or academic use cases:

**Tanishq Shinde**  
Department of Computer Engineering  
Pune Institute of Computer Technology  

---

## ⭐ Citation

If you use this dataset in academic work, please cite:

Shinde, T., Jangle, M., Bagwan, M.
"Coreference Resolution for Marathi Text Using Hypergraphs: A Hybrid Approach."
PICT, 2025.

---

Thank you for using this resource and contributing to advancing NLP for low-resource Indian languages!  
