# SCAD (Spam Campaign Attribution Dataset)


**A curated dataset for spam campaign detection, semantic clustering, and cryptocurrency forensic analysis.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📄 Overview

This repository contains a dataset designed to bridge the gap between Natural Language Processing (NLP) and Financial Forensics in the context of email spam. It is intended to support research in:
* Unsupervised Campaign Detection (Clustering/Topic Modeling).
* Multiclass Classification of Attack Vectors.
* Cryptocurrency Forensics & Attribution.

The dataset includes a filtered subset of spam emails from Spam Archive, along with a structured extraction of financial indicators (cryptocurrency addresses) found within the message payloads.


## Original Data (`filtered_spam_archive/`)
Contains the raw data as obtained from the source filtered by the selected date range, without any modification to the content, headers, or structure. 

* **Source:** **Untroubled Spam Archive**.
* **Description:** The dataset includes a filtered subset of spam emails originating from the **Untroubled Spam Archive**. This repository is a widely recognized resource in cybersecurity research, hosting a massive chronological collection of unsolicited emails harvested from honeypots. It serves as a benchmark for evaluating spam filtering, clustering frameworks, and forensic analysis methodologies.
* **Format:** Raw EML / Text files.

**Reference:**
> “Untroubled website,” 2013. [Online]. Available: http://untroubled.org/spam/


## 📂 Dataset Structure

The data is organized into three main components to ensure transparency and reproducibility:

```text

├── filtered_spam_archive.zip/
│   ├── 2022/
│	│	├── 01/
│	│	│	└──xxx.txt
│	│	│	└──....
│	│	│   ...
│	│	│	...
│	│	└── 12/
│	│		└──xxx.txt
│	│		└──....
│	│	...
│	│	...
│	└── 2025/
│		└── 01/
│			│	└──xxx.txt
│			│	└──....
│			│   ...
│			│	...
│			└── 12/
│				└──xxx.txt
│				└──....
│
│
└── processed/
    └── crypto_artifacts.json  