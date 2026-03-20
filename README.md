# IR_InvertedMatrix_Workshop
**PROG 8245 — Machine Learning Programming**  
Conestoga College — Graduate Diploma in Applied AI & Machine Learning

---

## Student
**Emmanuel Ihejiamaizu**  
Individual submission

---

## Dataset Description

The corpus used in this notebook is an **original, self-authored cybersecurity dataset** of **30 documents** written specifically for this workshop.

Each document is a detailed paragraph covering a distinct cybersecurity topic. The full corpus spans the following domains:

| # | Topic |
|---|-------|
| 1 | Network Intrusion Detection |
| 2 | Malware Analysis |
| 3 | Penetration Testing Methodologies |
| 4 | Cryptographic Protocols |
| 5 | Social Engineering & Phishing |
| 6 | Cloud Security Architecture |
| 7 | Zero Trust Architecture |
| 8 | Ransomware Attacks |
| 9 | Threat Intelligence Programs |
| 10 | Web Application Security |
| 11 | Identity & Access Management |
| 12 | Incident Response Frameworks |
| 13 | Endpoint Detection & Response |
| 14 | Vulnerability Management |
| 15 | SIEM Platforms |
| 16 | Supply Chain Security |
| 17 | Mobile Device Security |
| 18 | Insider Threat Programs |
| 19 | Firewall & Network Segmentation |
| 20 | Digital Forensics & Incident Response |
| 21 | Security Operations Center Design |
| 22 | Application Security Testing |
| 23 | Red Team Operations |
| 24 | Wireless Network Security |
| 25 | Data Privacy Regulations |
| 26 | Threat Modeling |
| 27 | Operational Technology Security |
| 28 | Deception Technology |
| 29 | Cryptomining Malware & Botnets |
| 30 | Bug Bounty Programs |

**Total unique vocabulary (raw):** 2,000+ words  
**License:** Original work — no external dataset or license required

---

## What the Notebook Does

The notebook builds a complete **Inverted Index NLP pipeline** from scratch:

1. **Step 1 — Document Collection:** Loads the 30 cybersecurity documents and verifies vocabulary size exceeds 2,000 unique words.
2. **Step 2 — Tokenizer:** Splits text into lowercase alphabetic tokens using regex.
3. **Step 3 — Normalization:** Removes English stopwords and applies Porter stemming via NLTK.
4. **Step 4 — Inverted Index + Phrase Queries:** Builds the index and runs two phrase queries — *"network intrusion"* and *"machine learning"*.
5. **Challenge 1 — Positional Index:** Stores exact token positions; includes a TF vs IDF comparison table and a talking point on bigram search.
6. **Challenge 2 — Optimized Positional Index:** Reduces memory usage with delta encoding and typed arrays (`array.array`).
7. **Challenge 3 — IDF:** Computes Inverse Document Frequency for all stems.
8. **Challenge 4 — TF & TF-IDF:** Computes Term Frequency and a full TF-IDF matrix across all 30 documents.

---

## How to Run

1. Open `IR_InvertedMatrix_Workshop.ipynb` in **Visual Studio Code** or **Google Colab** or **Jupyter Notebook**.
2. Run all cells from top to bottom.
3. NLTK stopwords will download automatically on first run.

---

## References & Frameworks Used

- [NLTK](https://www.nltk.org/) — stopword removal and Porter stemming
- [MITRE ATT&CK](https://attack.mitre.org/) — adversary technique framework referenced in corpus
- [OWASP Top Ten](https://owasp.org/www-project-top-ten/) — web application security categories referenced in corpus
- [NIST SP 800-61](https://csrc.nist.gov/publications/detail/sp/800-61/rev-2/final) — incident response lifecycle referenced in corpus
- Python standard libraries: `re`, `math`, `array`, `collections`
- [pandas](https://pandas.pydata.org/) — TF-IDF matrix display
