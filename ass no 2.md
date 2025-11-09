# 🧪 Experiment No. 02  
### **Title:** Implement Single-pass Algorithm for Clustering of Files  
---

## 🎯 Viva Questions

### 📘 **Conceptual Questions**

**Q1.** What do you mean by a *cluster*? What is a *cluster seed*?  
**A1.**  
A **cluster** is a group of similar objects having common characteristics.  
A **cluster seed** (or representative) is the initial element or centroid used to represent that cluster.

---

**Q2.** Why do we need clustering in Information Retrieval (IR)? What is the difference between *document-based* and *term-based* clustering?  
**A2.**  
Clustering helps group similar documents together to improve search efficiency and relevance.  
- **Document-based clustering:** Groups documents that share similar content.  
- **Term-based clustering:** Groups terms (words) that frequently appear together in documents.

---

**Q3.** How can we define relevance between documents?  
**A3.**  
Relevance is defined using a **similarity measure** (e.g., cosine similarity or dot product) that indicates how closely two documents are related based on shared terms.

---

**Q4.** How can we form clusters of documents?  
**A4.**  
We compute similarity between document vectors, then group documents into clusters where similarity exceeds a threshold. Each cluster has a representative centroid.

---

**Q5.** How many methods are there to define clusters?  
**A5.**  
There are two main types:  
1. **Hierarchical methods** – build clusters step by step.  
2. **Non-hierarchical methods** – directly form clusters in a single pass.

They can also be classified as:  
- **Exclusive Clusters** (no overlap)  
- **Overlapping Clusters** (elements can belong to multiple clusters)

---

**Q6.** Explain the **Single-Pass Algorithm**. What do you mean by *overlapping* and *exclusive* approach?  
**A6.**  
The **Single-Pass Algorithm** processes each object once:  
1. The first object forms the first cluster.  
2. Each new object is compared with existing cluster representatives.  
3. If similarity ≥ threshold → added to cluster.  
   Else → new cluster is formed.  

- **Exclusive approach:** Each object belongs to only one cluster.  
- **Overlapping approach:** Objects can belong to multiple clusters if similarity allows.

---

**Q7.** What is meant by a **similarity matrix**?  
**A7.**  
A **similarity matrix** is a table showing similarity scores between every pair of objects or documents, calculated using a similarity function like SIMILAR(di, dj).

---

**Q8.** What is the **time and space complexity** for the Single-Pass Algorithm?  
**A8.**  
- **Time Complexity:**  
  - Best Case → Ω(n)  
  - Average/Worst Case → Ω(n²)  
- **Space Complexity:**  
  Depends on the size of the similarity matrix and the number of clusters (O(n²) in general).

---

**Q9.** Which method is better for defining clusters?  
**A9.**  
It depends on the application:  
- **Hierarchical methods** are good for smaller datasets and detailed analysis.  
- **Single-pass (non-hierarchical)** methods are better for large, dynamic datasets due to efficiency.

---

### 💡 **Application-Based Questions**

**Q1.** Illustrate a situation when clustering will not be possible.  
**A1.**  
When all documents or terms are highly dissimilar (low similarity scores below threshold), clustering fails — each item becomes a separate cluster.

---

**Q2.** Create a document-based clustering for 5 documents.  
**A2.**  
Use a document-term matrix, calculate similarity between documents, choose a threshold, and apply the single-pass algorithm to group similar documents into clusters.

---

## 📚 Summary

- **Cluster:** Group of similar objects.  
- **Cluster Representative:** Centroid or average vector of a cluster.  
- **Threshold:** Minimum similarity required to join a cluster.  
- **Similarity Matrix:** Stores similarity between all pairs.  
- **Single-pass Algorithm:** Efficient one-pass clustering method.

---

✅ **Conclusion:**  
Term-based single-pass clustering was successfully implemented. The concept of threshold, similarity, and cluster representatives helps in grouping related documents effectively in an IR system.

---
---

# 📘 Basic Definitions — Clustering Algorithm

### 🔹 Cluster
A **cluster** is an ordered list or group of objects that have some **common characteristics** or similarities.

---

### 🔹 Distance Between Two Clusters
The **distance** between two clusters measures how far apart they are.  
It may involve comparing some or all elements of both clusters, depending on the chosen clustering method.

---

### 🔹 Similarity
A **similarity measure**, written as `SIMILAR(d1, dj)`, represents how **similar or related** two documents or objects are.  
Higher similarity means the documents are more alike.

---

### 🔹 Threshold
The **threshold** is the **minimum similarity value** required for two objects to be placed in the **same cluster**.  
If similarity < threshold → a **new cluster** is created.

---

### 🔹 Similarity Matrix
A **similarity matrix** is a table showing the similarity values between all pairs of objects.  
Each entry in the matrix is calculated using the function `SIMILAR(di, dj)`.

|       | D1  | D2  | D3  |
|-------|-----|-----|-----|
| **D1** | 1.0 | 0.8 | 0.3 |
| **D2** | 0.8 | 1.0 | 0.4 |
| **D3** | 0.3 | 0.4 | 1.0 |

---

### 🔹 Cluster Representative (Seed)
The **cluster representative** (also called a **seed**) is the main element that represents a cluster.  
Every new object’s similarity is compared with this representative to decide if it should join the cluster.

---

### 🔹 Similarity Between Documents
The **similarity value** shows how much two documents or objects are **close to each other** in terms of content.  
It is often calculated using shared keywords, index terms, or vector similarity methods.

---



# 📊 Analysis of Algorithm — Single Pass Clustering

---

### 🔹 Advantages
- **Simple to implement** — the algorithm is straightforward and easy to code.  
- **Less time requirement for searching** — since clustering groups similar data, searching within clusters becomes faster.

---

### 🔹 Disadvantages
- **Order-dependent** — the output depends on the **sequence in which objects are processed**.  
  Different input orders may lead to different clustering results.

---

### 🔹 Input
The program accepts the following inputs:
1. **Number of Tokens** — total unique words or features.  
2. **Number of Documents** — total documents or data points.  
3. **Threshold Value** — minimum similarity required to form or join a cluster.  
4. **Document Token Matrix** — a matrix showing the occurrence of each token in each document.

---

✅ **In short:**  
- **Cluster:** Group of similar items.  
- **Similarity:** How closely two items match.  
- **Threshold:** Minimum similarity needed to join a cluster.  
- **Cluster Representative:** The main document that defines the cluster.  
- **Similarity Matrix:** Table showing how similar each pair of documents is.

---
---
