# Multi-Domain Text Summarization Model Selection using TOPSIS

## Overview
This project evaluates **pre-trained NLP Text Summarization models** across **multiple text domains** and identifies the most optimal model using **TOPSIS (Technique for Order Preference by Similarity to Ideal Solution)**.  
Instead of judging models only by accuracy, this study balances **quality, speed, and computational efficiency**.

---

## Objective
To determine the **best summarization model** by comparing alternatives on multiple criteria and across different real-world content domains.

---

## Domains Evaluated
- **Politics**
- **Sports**
- **Health / Medical**

These domains represent formal, statistical, and technical writing styles, ensuring fair and diverse evaluation.

---

## Models Compared
- **BART**
- **T5-Small**
- **DistilBART**

Models were selected based on popularity, architecture diversity, and practical efficiency.

---

## Evaluation Criteria

| Criterion | Impact | Description |
|---------|--------|------------|
| **ROUGE-L Score** | Maximize (+) | Measures summary quality vs human reference |
| **Inference Time** | Minimize (–) | Measures response speed |
| **Model Size** | Minimize (–) | Indicates storage & computational cost |

---

## Methodology
1. **Dataset Selection** – CNN/DailyMail benchmark dataset  
2. **Domain Filtering** – Articles categorized using keyword matching  
3. **Model Execution** – Each model generated summaries per domain  
4. **Metric Calculation** – ROUGE-L, inference time, and model size recorded  
5. **Decision Matrix Creation** – Structured comparison table built  
6. **TOPSIS Application** – Ranking based on weighted multi-criteria analysis  
7. **Visualization** – Combined bar chart for cross-domain comparison

---

## Results

### Decision Matrix
<img width="473" height="380" alt="image" src="https://github.com/user-attachments/assets/c0fb45db-25ae-4619-b1d8-a323db21a68d" />


### TOPSIS Ranking
<img width="657" height="389" alt="image" src="https://github.com/user-attachments/assets/e8fbb4b5-a00a-4023-9d3a-51b342a179ca" />


### Combined Domain Comparison
<img width="864" height="563" alt="image" src="https://github.com/user-attachments/assets/f3a318f1-b190-42e1-adf1-d22f847a942c" />


---

## Key Insights
- Higher accuracy alone does **not** guarantee overall superiority  
- Lightweight models often deliver **better efficiency-performance balance**  
- Model effectiveness varies by domain, highlighting the importance of **context-aware selection**

---

## Conclusion
Using TOPSIS enabled a **holistic evaluation** rather than a single-metric comparison.  
The analysis demonstrates that the optimal summarization model is the one that **balances quality, speed, and efficiency across domains**, not merely the one with the highest ROUGE score.

---

## Tools & Technologies
**Python • HuggingFace Transformers • Datasets • ROUGE • NumPy • Pandas • Matplotlib • Google Colab**

---

> *A representative subset of the dataset was used to ensure computational feasibility while maintaining analytical validity.*
