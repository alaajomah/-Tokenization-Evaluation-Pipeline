# -Tokenization-Evaluation-Pipeline

# 📘 NLP Mini Project – Tokenization & Summarization Evaluation

This project explores how different tokenization methods and summarization models affect NLP output quality.  
The work is divided into three main components:

---

## 🔹 1. Tokenization Experiment

Three tokenizers were applied to the **same biomedical text sample**:

- **TicToken**
- **WordPiece (BERT tokenizer)**
- **SentencePiece (Unigram/BPE model)**

### Tasks Performed

### ✔ Tokenized Output  
Each tokenizer was applied to the same input text to observe how words—especially technical biomedical terms—were split into tokens.

### ✔ Sequence Length  
The number of resulting tokens was recorded for each tokenizer to compare efficiency and compression.

### ✔ Explanation of Differences  
A discussion highlights:
- How each tokenizer handles rare or long words  
- The subword splitting behavior  
- How vocabulary size affects tokenization  
- How tokenization impacts computational cost and downstream model understanding  

---

## 🔹 2. Mini Evaluation Task 

A summarization task was performed using **two different models**:

- **Model A:** BART (`facebook/bart-large-cnn`)  
- **Model B:** T5-small (`t5-small`)

### ✔ Model Outputs  
Each model generated a summary of the same biomedical paragraph.

### ✔ ROUGE-1 
Automatic metrics were computed:

- **ROUGE-1** → Measures unigram overlap  

These metrics quantify how closely each summary aligns with the original text.

### ✔ Human Evaluation Rubric  
Each summary was manually evaluated on a **1–5 scale**:

| Criterion     | Description |
|---------------|-------------|
| **Clarity**   | Readability and fluency of the summary |
| **Correctness** | Accuracy of preserved medical facts |
| **Coherence** | Logical flow and structure |

The averaged scores were used to compare the two models.

---

## 🔹 3. Optimization Reflection 

A reflection discussing how the following factors influenced results:

### ✔ Tokenization  
- Impact on sequence length  
- Effects on how biomedical terminology is split  
- Influence on model comprehension and evaluation metrics  

### ✔ Prompt Quality  
- Why consistent prompts ensure fair comparison  
- How well-structured prompts reduce hallucination  
- How prompt specificity influences detail retention  

### ✔ Sequence Length  
- Relationship between input length and computational cost  
- How models compress dense information  
- Trade-offs between short vs. long generated summaries  

---

## 📂 Project Structure

