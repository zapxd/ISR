# 🎯 Viva Questions — Experiment No. 05  
### **Title:** Program to calculate Harmonic Mean (F-Measure) and E-Measure  

---

## 🔹 Q1. What is the F-Measure?
**Answer:**  
The **F-Measure (or F1-Score)** is the **harmonic mean of Precision and Recall**.  
It gives a single value that balances both Precision and Recall.  

**Formula:**  
F = 2 × (Precision × Recall) / (Precision + Recall)

---

## 🔹 Q2. Why is the F-Measure called a harmonic mean?
**Answer:**  
It is called a harmonic mean because it **balances** the effect of large differences between Precision and Recall — giving a **lower value** if either one is low.  

---

## 🔹 Q3. What is the importance of the F-Measure in Information Retrieval?
**Answer:**  
The F-Measure helps to **evaluate the overall performance** of an IR system by combining both Precision and Recall into a single metric.  
It is useful when there is a need to **balance relevance and completeness** of retrieved results.

---

## 🔹 Q4. What are the ideal values of F-Measure?
**Answer:**  
- **F = 1:** Perfect system (all retrieved documents are relevant)  
- **F = 0:** Poor system (no relevant document retrieved)

---

## 🔹 Q5. What is the E-Measure?
**Answer:**  
The **E-Measure** is another evaluation metric that combines Precision and Recall, but it includes a parameter **β (beta)** to indicate the **relative importance** of Precision and Recall.

---

## 🔹 Q6. What does β (beta) represent in E-Measure?
**Answer:**  
β represents the **relative importance** of Precision and Recall.  
- If **β < 1** → Precision is more important.  
- If **β > 1** → Recall is more important.  
- If **β = 1** → Equal importance of both.

---

## 🔹 Q7. Write the formula for E-Measure.
**Answer:**  
E = 1 - F / [(β² × Precision) + Recall]

*(Note: Formula may vary depending on the definition used; main idea is to combine Precision and Recall with β weight.)*

---

## 🔹 Q8. Why do we use E-Measure instead of only Precision or Recall?
**Answer:**  
Because **Precision** alone ignores completeness, and **Recall** alone ignores accuracy.  
E-Measure gives a **weighted combination**, depending on what is more important to the user (Precision or Recall).

---

## 🔹 Q9. In which situations is F-Measure most useful?
**Answer:**  
F-Measure is most useful when dealing with **imbalanced data**, or when we want a **balance between Precision and Recall**, such as in **Information Retrieval** or **Classification** problems.

---

## 🔹 Q10. What is the main difference between F-Measure and E-Measure?
**Answer:**  
- **F-Measure:** Harmonic mean of Precision and Recall (equal importance).  
- **E-Measure:** Weighted measure that allows different importance levels for Precision and Recall (using β).

---

## ✅ **Conclusion**
The concepts of **F-Measure** and **E-Measure** help evaluate Information Retrieval systems by combining Precision and Recall into a single, meaningful score that reflects both relevance and completeness.

