# Medical Named Entity Recognition (NER)

This project implements a Named Entity Recognition (NER) system to extract medical entities from clinical text using transformer-based models.

---

## Overview

The goal of this project is to build a model that can automatically identify important medical information such as:

- Age
- Sex
- Medical History
- Symptoms
- Medication
- Dosage

The model is trained and evaluated on the MACCROBAT dataset using BIO tagging scheme.

---

## Methodology

- Tokenize input text using pretrained tokenizer
- Apply BIO tagging for sequence labeling
- Align word-level labels with subword tokens
- Fine-tune transformer-based model for NER task
- Evaluate performance using F1-score, Precision, Recall

---

## Dataset

- **MACCROBAT (Medical Abdominal CT Corpus with Radiology Reports)**
- Contains clinical text with annotated medical entities

---

## Technologies

- Python
- PyTorch
- Hugging Face Transformers
- SeqEval (evaluation)

---

## Training

I used a pretrained biomedical NER model from Hugging Face and fine-tuned it on the MACCROBAT dataset

---

## result
Epoch	Training Loss	Validation Loss	Precision	Recall	F1	Accuracy
1	No log	0.270725	0.911658	0.927099	0.919314	0.960476
2	No log	0.272653	0.900844	0.943299	0.921583	0.961616
3	No log	0.274693	0.910256	0.941090	0.925416	0.965163
4	No log	0.274531	0.909993	0.945508	0.927411	0.965290
5	No log	0.273414	0.921316	0.948454	0.934688	0.967317
6	No log	0.280762	0.918746	0.949190	0.933720	0.966810
7	No log	0.287607	0.917080	0.952872	0.934633	0.966937
8	No log	0.283100	0.917496	0.949926	0.933430	0.966557
9	No log	0.288345	0.918382	0.952872	0.935309	0.966684
10	No log	0.287793	0.919687	0.952872	0.935986	0.966937
