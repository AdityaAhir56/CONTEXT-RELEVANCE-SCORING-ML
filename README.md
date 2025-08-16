# Context Relevance Scoring for Enterprise Knowledge Management Systems

## 📌 Overview  
This project develops a **regression-based machine learning model** to predict continuous relevance scores (0–1) for query–context pairs in enterprise knowledge management systems (e.g., HR, legal, IT support). The goal is to **optimize context retrieval for Large Language Models (LLMs)**, improving the accuracy, coherence, and efficiency of generated responses.

By scoring and ranking candidate documents, FAQs, or database records, the model filters out irrelevant or marginally relevant context items, reducing noise and boosting response quality.

---

## 🎯 Problem Statement  
Enterprise knowledge systems often retrieve noisy or irrelevant context due to ineffective scoring. This leads to:  
- Lower LLM response accuracy  
- Increased user frustration  
- Higher operational latency  

**Objective:** Train and deploy a regression model to:  
1. Predict relevance scores for potential context items.  
2. Select the top-k most relevant items for the LLM’s context window.  
3. Maintain low-latency performance for real-time systems.  

---

## 📊 Dataset  
- **Size:** 10,000+ query–context pairs  
- **Features:**  
  - Query embeddings, context embeddings  
  - Metadata (document type, recency, author)  
  - Interaction history (clicks, session features)  
  - Similarity scores, keyword overlaps  
- **Target:** Relevance score (0–1) labeled with realistic noise

---

## ⚙️ Methodology  
1. **Data Generation:** Synthetic but realistic enterprise queries and context items.  
2. **Preprocessing:**  
   - Missing value imputation  
   - Feature scaling  
   - Embedding-based similarity calculation  
3. **Modeling:**  
   - **LightGBM Regressor** (for speed & interpretability)  
   - **Neural Network Regressor** (for complex feature interactions)  
4. **Evaluation Metrics:**  
   - Mean Absolute Error (MAE)  
   - Root Mean Squared Error (RMSE)  
   - Precision@K  
   - Inference latency  

---

## 🚀 Results  
- **MAE:** XX.XXX  
- **RMSE:** XX.XXX  
- **Precision@5:** XX%  
- **Latency Reduction:** ~XX% vs baseline  

*(Replace XX with actual results from notebook execution.)*

---

## 📈 Key Features  
- Synthetic dataset generation with realistic enterprise noise  
- Multi-turn query handling for context coherence  
- Bias detection and analysis  
- Scalable for real-time deployment with LLM pipelines  

---

## 🛠️ Technologies Used  
- **Python 3.x**  
- **Pandas, NumPy**  
- **Scikit-learn**  
- **LightGBM / XGBoost**  
- **Sentence-BERT** (for embeddings)  
- **Matplotlib, Seaborn**  

For questions or collaborations, feel free to connect via Linkedin:- https://www.linkedin.com/in/adityaahir/.
