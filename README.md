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

## 📢 Data Source & Acknowledgements

We explicitly acknowledge and thank the **L3Cube-Pune** team for providing the underlying raw text used in this annotation project.

- **Source Corpus:** [L3Cube-MahaCorpus (news)](https://github.com/l3cube-pune/MarathiNLP)
- **Repository:** [L3Cube-Pune MarathiNLP](https://github.com/l3cube-pune/MarathiNLP)

The raw news articles were sourced from their open-source repository, which acts as a foundational resource for Marathi NLP tasks. Our work builds upon this by adding the layer of semantic coreference annotations.

---

## 📊 Dataset Statistics

The following statistics describe the scale and density of the annotated corpus:

| Metric | Count |
| :--- | :--- |
| **Total Processed Documents** | **490** |
| **Total Sampled Sentences** | **9,994** |
| **Unique Tokens (Vocabulary)** | **5,053** |
| **Annotated Coreference Pairs** | **12,963** |
| **Average Sentence Length** | **29.83 words** |

---

## 🧪 Data Structure & Format

The dataset is provided in **JSON (JavaScript Object Notation)** format, optimized for Hypergraph-based approaches.

### JSON Schema Fields

Each file in the dataset follows this structure:

* **`document_id`**: Unique identifier for the document.
* **`sentences`**: A list containing the raw text of the sentences.
* **`mentions`**: A list of all identified entities (Nouns/Pronouns) with the following metadata:
    * `id`: Unique mention ID.
    * `text`: The surface word (e.g., "पंतप्रधान").
    * `sentence_index`: Index of the sentence containing the mention.
    * `start_char`, `end_char`: Character-level spans of the mention.
* **`clusters`**: A list of coreference chains. Each chain is a list of `mention_ids` that refer to the same underlying entity.

---

## 📂 Repository Contents

The repository includes:

- `processed_documents/` — Raw Marathi text documents (Sourced from L3Cube-MahaCorpus).
- `annotated_documents/` — Gold-standard coreference annotations in JSON+CoNLL format.
- `schema.md` — Annotation guidelines and tag definitions.

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
"Coreference Resolution for Marathi Text Using Hypergraph Method"
PICT, 2025.
