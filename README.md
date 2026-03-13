# Retrato_Cantado: Corpus for Identity Representation in Brazilian Song Lyrics

This repository provides the dataset and experimental resources associated with the research project:

**Retrato_Cantado: Creation and Analysis of a Corpus for Identity Representation in Brazilian Song Lyrics**

The project introduces a corpus of sentences extracted from Brazilian song lyrics and manually annotated to identify **predicative constructions describing individuals**. The dataset enables computational analysis of how people are characterized in Brazilian music, including aspects such as identity, appearance, behaviors, and social roles.

---

# 📄 Paper

The link to the published version will be added here once it becomes available.

---

# 📊 Dataset

Due to GitHub file size limitations, the dataset is available for download via Google Drive:

📥 **Download dataset**
https://drive.google.com/file/d/1Ri6V95Kfc1BS3OVD5I1p6hcg5hap4p6i/view?usp=sharing

---

# 🏷 Dataset Description

The dataset contains sentences extracted from Brazilian song lyrics and annotated to identify whether they describe or characterize a person.

Annotations include:

**Predicative sentence detection**

* Whether the sentence characterizes a person

**Sentiment polarity**

* Positive
* Negative
* Neutral

**Semantic categories of characterization**

The annotation scheme includes the following categories:

* Identity
* Appearance
* Social Role
* Skills / Competences
* Values / Beliefs
* Behaviors
* Other

The corpus was annotated by **38 volunteers from different academic programs**, ensuring diverse perspectives in the annotation process.

---

# 🧠 Method Overview

The corpus construction pipeline includes:

1. Collection of Brazilian song lyrics
2. Sentence segmentation using **spaCy**
3. Extraction of candidate sentences using **lexical-syntactic patterns**
4. Manual annotation by human annotators
5. Sentiment and semantic categorization
6. Training of a **BERT-based classifier** for predicative sentence detection

The classification model was based on the Portuguese BERT model:

`neuralmind/bert-base-portuguese-cased`

---

# 📈 Experiments

A supervised classifier was trained to automatically detect predicative sentences describing individuals.

Evaluation was performed using **stratified cross-validation**, achieving approximately:

* **Accuracy:** ~0.90
* **Weighted F1-score:** ~0.90

These results demonstrate the feasibility of automatically identifying person-characterization patterns in song lyrics.

---

# ▶️ Reproducing the Analysis

1. Clone this repository

```
git clone https://github.com/YOUR_USERNAME/retratro-cantado-corpus
```

2. Download the dataset from Google Drive.

3. Run the exploratory notebook:

```
notebooks/1.1.explore_sentences.ipynb
```

The notebook provides examples of how to load and analyze the dataset.

---

# 🔬 Research Applications

The dataset can support research in areas such as:

* Natural Language Processing for Portuguese
* Gender representation in culture
* Cultural analytics
* Bias and stereotype detection
* Social discourse analysis
* Digital humanities


