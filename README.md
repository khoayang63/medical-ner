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
Training result from epoch 10:
Precision: 0.919687
Recall: 0.952872
F1:	0.935986
Accuracy: 0.966937
		
