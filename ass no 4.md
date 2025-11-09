# 🧠 Viva Questions — Experiment No. 04  
### **Title:** Implement a program to calculate Precision and Recall for sample input

---

## 🎯 **Aim**
To implement a program to calculate **Precision** and **Recall** for a given query and relevant document set.

---

## 🧩 **Conceptual Questions**

### **Q1. What do you mean by Precision?**
> **Precision** is the proportion of retrieved documents that are actually relevant to the query.  
**Precision** = (Number of relevant documents retrieved) / (Total number of documents retrieved)

---

### **Q2. What do you mean by Recall?**
> **Recall** is the proportion of relevant documents that have been successfully retrieved.  
**Recall** = (Number of relevant documents retrieved) / (Total number of relevant documents)

---

### **Q3. Why is Precision and Recall important in Information Retrieval (IR)?**
> They are key metrics to **evaluate the performance** and **effectiveness** of an IR system — measuring how accurately and completely relevant documents are retrieved.

---

### **Q4. What is meant by “Relevant Documents”?**
> Documents that satisfy the user’s **information need** or correctly match the query context.

---

### **Q5. What are “Retrieved Documents”?**
> Documents that the system returns as results for a given query — whether relevant or not.

---

### **Q6. What is meant by “Relevant and Retrieved Documents”?**
> The intersection of relevant and retrieved sets — these are the **true positives**, i.e., documents both relevant and retrieved.

---

### **Q7. Define the goal of an ideal IR system.**
> An ideal IR system should achieve **high precision** and **high recall** — retrieving all relevant documents while minimizing irrelevant ones.

---

### **Q8. What is a Contingency Table in IR evaluation?**
> It’s a 2×2 table that categorizes documents based on relevance and retrieval status:

|                 | Retrieved | Not Retrieved |
|-----------------|------------|---------------|
| **Relevant**     | w          | x             |
| **Not Relevant** | y          | z             |

> - **Precision (P):** w / (w + y)  
> - **Recall (R):** w / (w + x)

---

### **Q9. What is the difference between Precision and Recall?**
| Feature | **Precision** | **Recall** |
|----------|---------------|-------------|
| Definition | Proportion of retrieved docs that are relevant | Proportion of relevant docs that are retrieved |
| Focus | Accuracy of results | Completeness of results |
| Goal | Minimize irrelevant docs | Retrieve all relevant docs |

---

### **Q10. What does high Precision but low Recall indicate?**
> The system retrieves **only a few documents**, but they are **highly relevant**.  
> Example: strict filtering or highly specific search.

---

### **Q11. What does high Recall but low Precision indicate?**
> The system retrieves **most of the relevant documents**, but also **many irrelevant ones**.  
> Example: broad or general searches.

---

### **Q12. What is meant by Relevance?**
> Relevance measures how well a document satisfies the **user’s information need** or query intent.

---

### **Q13. What are the types of Relevance Judgments?**
> 1. **Binary Relevance:** 1 = relevant, 0 = not relevant  
> 2. **Graded (N-ary) Relevance:** 0 = not relevant, 1 = slightly relevant, 2 = relevant, 3 = very relevant  

---

### **Q14. What factors affect Relevance?**
> - User’s query intent  
> - Context of search  
> - Document content quality  
> - Subjectivity of user judgment  

---

### **Q15. What is the trade-off between Precision and Recall?**
> Increasing **Recall** often lowers **Precision**, and vice versa — finding a balance depends on the application.  
> - Example: Legal or medical searches prefer **high recall**.  
> - Web search prefers **high precision**.

---

## ⚙️ **Practical/Algorithm-Based Questions**

### **Q16. What are the inputs for calculating Precision and Recall?**
> - **Answer Set (A):** Documents retrieved by the system.  
> - **Query (q1):** Search query entered by user.  
> - **Relevant Documents (Rq1):** Documents truly relevant to the query.

---

### **Q17. What is the output of the Precision and Recall program?**
> The calculated **Precision** and **Recall** values based on the given input sets.

---

### **Q18. Write the mathematical formulas for both Precision and Recall.**
> - **Precision (P):**  
>   P = |Relevant ∩ Retrieved| / |Retrieved|  
> - **Recall (R):**  
>   R = |Relevant ∩ Retrieved| / |Relevant|

---

### **Q19. What is meant by “Evaluation Workflow” in IR systems?**
> It’s the process of testing the IR system’s performance by comparing retrieved results against a set of known relevant documents.

---

### **Q20. What are the main parameters to evaluate an IR system?**
> - **Effectiveness** (Precision, Recall, F-measure)  
> - **Efficiency** (Time and Space complexity)  
> - **User Satisfaction** (Ease of use, relevance)

---

### **Q21. What is meant by “F-measure” or “F1-score”?**
> A single metric that balances Precision and Recall:  
> \[
F1 = 2 × \frac{(Precision × Recall)}{(Precision + Recall)}
\]
> It is useful when both metrics are equally important.

---

### **Q22. What happens if no relevant documents are retrieved?**
> - **Precision = 0**, because numerator (relevant retrieved) = 0.  
> - **Recall = 0**, as no relevant items were retrieved.

---

### **Q23. What is the range of Precision and Recall values?**
> Both lie between **0 and 1** (or 0% – 100%).  
> - 1 → Perfect performance  
> - 0 → No performance

---

### **Q24. Why is human judgment needed in measuring Relevance?**
> Because determining if a document satisfies a query is **subjective** and depends on human interpretation.

---

### **Q25. Give an example scenario for calculating Precision and Recall.**
> **Relevant documents:** D1, D4, D5, D8, D10  
> **Retrieved documents:** D2, D4, D5, D6, D8  
> - Relevant & Retrieved = D4, D5, D8 → 3  
> - **Precision = 3/5 = 0.6**  
> - **Recall = 3/5 = 0.6**

---

## 💡 **Higher-Level / Analytical Questions**

### **Q26. Explain why Precision and Recall are inversely related.**
> Increasing recall by retrieving more documents often introduces irrelevant ones, reducing precision, and vice versa.

---

### **Q27. How can we improve both Precision and Recall together?**
> - Better query formulation  
> - Improved document indexing and ranking algorithms  
> - Use of relevance feedback mechanisms  

---

### **Q28. What are the limitations of using only Precision and Recall?**
> - They don’t consider **ranking order** of results.  
> - Assume **binary relevance**, ignoring degrees of relevance.  
> - Don’t directly measure **user satisfaction**.

---

### **Q29. Mention other evaluation metrics used in IR.**
> - **F-measure / F1-score**  
> - **Mean Average Precision (MAP)**  
> - **Normalized Discounted Cumulative Gain (nDCG)**  
> - **ROC Curves / Precision-Recall Curves**

---

### **Q30. Why is evaluation important in Information Retrieval systems?**
> Evaluation ensures the system retrieves accurate, relevant, and complete information efficiently — improving user trust and overall system performance.

---

✅ **Conclusion:**  
The experiment demonstrates how **Precision and Recall** are calculated to evaluate the **performance and accuracy** of Information Retrieval systems.

