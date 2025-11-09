# 🧠 Viva Questions & Answers  
### **Experiment No. 01 — Conflation Algorithm**  
**Subject:** Information Retrieval  
**Language Used:** C/C++ (with File Handling)  

---

## 🔹 **Basic Conceptual Questions**

### 1. What is Information Retrieval (IR)?
**Answer:**  
Information Retrieval is the process of obtaining relevant information from a large collection of unstructured data (like text documents) based on a user’s query.

---

### 2. What is a Document Representative?
**Answer:**  
A document representative is a short summary made up of important words or terms that best describe the main content and meaning of a document.

---

### 3. What is the Conflation Algorithm?
**Answer:**  
The conflation algorithm reduces related words to a common base or root form (called a stem). It includes **removal of stop words**, **suffix stripping**, and **detecting equivalent stems** to create a document representative.

---

### 4. What is the main purpose of the Conflation Algorithm in IR?
**Answer:**  
To normalize and reduce word variations, making document retrieval more effective by mapping similar terms to the same base form.

---

### 5. What are “stop words”?  
**Answer:**  
Stop words are common, high-frequency words (like *the, is, an, of, and*) that do not carry significant meaning and are usually removed from the text to reduce noise.

---

### 6. Why are stop words removed in text processing?
**Answer:**  
They do not contribute to the meaning or retrieval efficiency and occupy unnecessary space, so removing them reduces data size and improves processing speed.

---

### 7. What is suffix stripping?
**Answer:**  
Suffix stripping removes common word endings (like *-ing, -ed, -s*) to obtain the base or stem form of the word, e.g., *playing → play*.

---

### 8. What is stemming?
**Answer:**  
Stemming is the process of reducing words to their root or base form. For example, *“studies”, “studying”, “studied”* all become *“study”*.

---

### 9. What is Luhn’s contribution to IR?
**Answer:**  
Luhn proposed using **word frequency** and **position** to determine word and sentence significance in a document — forming the foundation for automatic text analysis.

---

### 10. What are the three stages of the Conflation Algorithm?
**Answer:**  
1. **Removal of stop words**  
2. **Suffix stripping**  
3. **Detection of equivalent stems**

---

## 🔹 **Intermediate Questions**

### 11. What are high-frequency words?  
**Answer:**  
Words that occur very frequently across most documents (like “the”, “of”, “is”) and carry little semantic value.

---

### 12. Why do we remove high-frequency words in IR systems?  
**Answer:**  
Because they appear in almost all documents and do not help distinguish between relevant and non-relevant documents.

---

### 13. What is the advantage of removing stop words?  
**Answer:**  
It reduces document size by 30–50% and improves retrieval efficiency by focusing only on meaningful terms.

---

### 14. What is meant by “equivalent stems”?  
**Answer:**  
Different words that have the same root meaning, e.g., *“connect”, “connection”, “connected”*, are treated as belonging to the same class or stem.

---

### 15. What is the output of the Conflation Algorithm?  
**Answer:**  
A **set of classes or stems** representing the key terms of the document — called the **document representative** or **index terms**.

---

### 16. What happens if suffix removal is done without context rules?  
**Answer:**  
It may cause errors — for example, removing *“ual”* from *“equal”* gives *“eq”*, which is incorrect. Hence, context-based rules are required.

---

### 17. Give an example of Conflation Algorithm output.  
**Example Input:**  
“Some text is here”  
**After removing stop words:**  
“text”  
**After stemming:**  
“text”  
**Final Output:**  
[text (frequency: 1)]

---

### 18. What is the difference between Information Retrieval (IR) and Data Retrieval (DR)?  
| Aspect | Information Retrieval | Data Retrieval |
|--------|------------------------|----------------|
| Data Type | Unstructured (text, docs) | Structured (databases) |
| Matching | Approximate or fuzzy | Exact |
| Query | Natural language | Formal query language |
| Output | Ranked documents | Exact data values |

---

### 19. What is meant by the “upper cut-off” in Luhn’s theory?  
**Answer:**  
It is a threshold above which words are too frequent to be meaningful — they are considered non-significant (stop words) and are ignored.

---

### 20. What is the “lower cut-off” in Luhn’s theory?  
**Answer:**  
It refers to words that occur too rarely to be meaningful; such words are also ignored.

---

## 🔹 **Advanced / Application-Based Questions**

### 21. What will happen if a search word occurs rarely in the document?  
**Answer:**  
The document may not be retrieved if the term frequency is below the threshold or if it doesn’t appear in the representative set.

---

### 22. Why is feedback important in an IR system?  
**Answer:**  
Feedback (like relevance feedback) helps the system improve search results by learning from user input and refining future retrievals.

---

### 23. How does conflation improve retrieval performance?  
**Answer:**  
By grouping words with similar meanings under one stem, conflation increases recall (retrieves more relevant documents) without significantly affecting precision.

---

### 24. How is frequency count used in document representation?  
**Answer:**  
Word frequency helps determine the importance of a term within a document. Higher frequency often implies greater significance.

---

### 25. What are index terms or keywords?  
**Answer:**  
They are the significant words (stems) that represent the content of a document and are used during retrieval.

---

### 26. What are the main advantages of the Conflation Algorithm?  
**Answer:**  
- Reduces data redundancy  
- Improves retrieval accuracy  
- Handles linguistic variations  
- Minimizes storage usage  

---

### 27. What are the limitations of Conflation Algorithms?  
**Answer:**  
- Over-stemming (merging unrelated words)  
- Under-stemming (not merging related words)  
- Context dependency  

---

### 29. What language is used to implement this experiment?  
**Answer:**  
The experiment is implemented using **C or C++** with file handling operations.

---

## 🔹 **Additional Frequently Asked Questions (from context)**

### 31. What is the necessity of feedback mechanism in IR?  
**Answer:**  
Feedback mechanisms enhance search accuracy by learning from user responses and adjusting retrieval parameters accordingly.

---

### 33. Draw or explain the block diagram of IR system.  

                ┌──────────────────────────┐
                │        User Query         │
                └────────────┬──────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │     Query Processing      │
                │ (Tokenization, Stop-word  │
                │  removal, Stemming etc.)  │
                └────────────┬──────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │     Information Retrieval │
                │          System           │
                │  (Search Engine / IR Model│
                │   e.g. Vector Space Model)│
                └────────────┬──────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │     Document Index /      │
                │     Database Storage       │
                └────────────┬──────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │   Retrieved Documents     │
                │ (Ranked by Relevance)     │
                └────────────┬──────────────┘
                             │
                             ▼
                ┌──────────────────────────┐
                │     User Feedback         │
                │ (Relevance Feedback helps │
                │   refine future queries)  │
                └──────────────────────────┘
                

---

### 34. If your search is based on a word that occurs very rarely in the document, what will happen?  
**Answer:**  
The IR system may fail to retrieve relevant documents or return very few results since rare words have low frequency and might not be indexed.

---

### 37. What is the output of the Conflation Algorithm for input “Some text is here”?  
**Answer:**  
- After stop word removal → “text”  
- After suffix stripping → “text”  
- **Output:** “text” (Frequency count = 1)

---

## 🔹 **Conclusion (for viva)**  
**The Conflation Algorithm** helps generate a concise **document representative** by eliminating stop words, performing suffix stripping, and grouping equivalent stems. This improves retrieval efficiency and reduces data redundancy in Information Retrieval systems.

---
