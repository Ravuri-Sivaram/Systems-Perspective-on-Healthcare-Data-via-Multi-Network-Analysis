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

### 🧩 1. Condition–Drug Bipartite Network  
- **Extreme Centralization:** The condition *“Transplanted lung present”* emerged as a dominant hub with a weighted degree exceeding **12 million**, indicating strong drug connectivity.  
- **Bridging Edges:** Drug–condition pairs such as *“Primary malignant neoplasm of female breast”* and opioid-based treatments showed high betweenness, acting as critical connectors across medical domains.  
- **Clinical Insight:** Highly centralized nodes correspond to complex, multi-drug regimens, revealing polypharmacy risks and treatment dependencies for chronic or transplant patients.  

---

### 🔗 2. Condition–Condition Co-occurrence Network  
- **Threshold Impact:** Increasing the co-occurrence threshold from 40 to 60 reduced edges by **56%** and nodes by **39%**, highlighting how strict criteria refine the network to core disease relationships.  
- **Stable Disease Hubs:** *Essential hypertension* and *Hyperlipidemia* remained highly central even under stricter thresholds, representing the backbone of chronic multimorbidity.  
- **Clinical Insight:** The refined network focuses on persistent disease pairings fundamental to chronic disease management, though some rare but meaningful connections are filtered out.  

---

### ❤️ 3. Condition–Risk Factor Correlation Network  
- **Moderate Modularity:** The network displayed a clustering coefficient of **0.2822** and near-neutral assortativity (**–0.0003**), showing slightly disassortative mixing—highly connected nodes tend to link to less connected ones.  
- **Influential Biomarkers:** Hematologic indicators such as **MCHC** and **MCV** had high eigenvector centrality (>0.13), highlighting their influence in cardiovascular risk modeling.  
- **Clinical Insight:** Modular biomarker clusters align with physiological pathways, improving the interpretability of disease-risk linkages for precision medicine applications.  

---

### 🧠 Overall Interpretation  
- Each network demonstrates **unique structural patterns**—from centralized hubs and bridging edges to modular biomarker groups.  
- These properties reveal hidden medical dependencies and highlight critical connections that can inform **predictive modeling, treatment optimization, and chronic disease prevention** strategies.  


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
Graduate Student - University of South Florida

---

⭐ *If you find this project insightful, consider giving it a star on GitHub!*
