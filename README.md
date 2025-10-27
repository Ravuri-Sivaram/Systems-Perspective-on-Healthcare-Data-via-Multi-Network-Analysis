# Systems-Perspective-on-Healthcare-Data-via-Multi-Network-Analysis
This project applies Social Network Analysis (SNA) to EHR data from 2,000 patients to reveal links among conditions, drugs, and risk factors. Three networks were built to identify key diseases, comorbidity clusters, and treatment hubs, supporting data-driven insights for personalized healthcare.
# 🧠 EHR Network Analysis using Social Network Analysis (SNA)

## 📄 Abstract  
This project applies **Social Network Analysis (SNA)** to **Electronic Health Record (EHR)** data to uncover relationships among medical conditions, treatments, and risk factors. Using structured data from **2,000 patients** in the **EHRShot dataset**, we built three distinct networks:  
1. 🧩 **Condition–Drug Bipartite Network**  
2. 🔗 **Condition–Condition Co-occurrence Network**  
3. ❤️ **Condition–Risk Factor Correlation Network**

These networks reveal hidden patterns in healthcare data, highlighting key diseases, comorbidity clusters, and treatment hubs. Centrality measures and community detection help interpret complex relationships that can support data-driven and predictive healthcare.

---

## ⚙️ Methodology  
- **Dataset:** Subset of 2,000 patients from *EHRShot* (synthetic EHR dataset)  
- **Techniques:** Classical SNA using `NetworkX`, `PyVis`, and Louvain community detection  
- **Metrics Used:**  
  - Degree Centrality  
  - Eigenvector Centrality  
  - Clustering Coefficient  
  - Louvain Modularity  

Networks were filtered using **edge thresholds** to improve interpretability and reduce visualization density.

---

## 🧩 Networks Built  
### 1️⃣ Condition–Drug Bipartite Network  
Shows interactions between medical conditions and prescribed drugs.  

### 2️⃣ Condition–Condition Co-occurrence Network  
Highlights conditions that frequently occur together among patients.  

### 3️⃣ Condition–Risk Factor Correlation Network  
Explores how diseases correlate with demographic and cardiovascular risk factors (e.g., gender under 45, biomarkers).  

---

## 📈 Results & Insights  
- Over **3,500 strong co-occurrence edges** among ~229 conditions.  
- Detected **high-degree nodes** representing dominant conditions and treatment hubs.  
- Interactive visualizations generated using **PyVis** (`.html` files).  

---

## 🧠 Tools & Libraries  
- Python 🐍  
- Pandas, NumPy, NetworkX, PyVis  
- Matplotlib  
- Jupyter Notebook  

---

---

## 🚀 Future Work  
- Extend dataset to multi-year patient histories  
- Integrate Graph Neural Networks (GNNs) for predictive modeling  
- Explore dynamic temporal networks for longitudinal EHR data  

---

## 👨‍💻 Author  
**Ravuri Sivaram**  
Graduate Researcher – Data Science & Machine Learning  

---

⭐ *If you find this project insightful, consider giving it a star on GitHub!*
