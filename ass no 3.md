# 🧠 Viva Questions — Experiment No. 03  
### **Title:** Implement a program for retrieval of documents using inverted files

---

## 📘 **Conceptual Questions**

### **Q1.** What do you mean by an **inverted file**?  
> An inverted file is a data structure that stores a mapping from content (such as words or terms) to their locations in a database, document, or a set of documents.

---

### **Q2.** What is a **word-oriented mechanism**?  
> It refers to indexing based on words rather than characters, where each word in the document vocabulary points to the positions where it appears.

---

### **Q3.** What do you mean by a **dictionary** in the context of inverted files?  
> The dictionary (or vocabulary) is a list of all unique terms or words that appear in the document collection.

---

### **Q4.** What is the role of **postings** in an inverted file?  
> Postings store the information about the occurrence of each term — such as document IDs, positions, and frequencies.

---

### **Q5.** What are the **different applications of inverted index**?  
> - Document retrieval systems (e.g., search engines)  
> - Text mining and data analysis  
> - Information filtering  
> - Natural language processing tasks  
> - Plagiarism detection  

---

### **Q6.** How is an **inverted index helpful in searching**?  
> It allows direct access to documents containing a given keyword, enabling faster retrieval compared to sequential searching.

---

### **Q7.** What do you mean by **merging similar terms** from different documents?  
> It refers to combining entries of the same term that appear in multiple documents to form a unified postings list.

---

### **Q8.** What is the **time complexity** and **space complexity** for the Single Pass algorithm?  
> - **Time Complexity:** O(n) (for linear scanning)  
> - **Space Complexity:** O(t + d), where *t* = number of terms and *d* = number of documents  

---

### **Q9.** What are the **applications of inverted file structures**?  
> - Web search engines (like Google)  
> - Digital libraries  
> - Email or log searching  
> - Text categorization systems  

---

## ⚙️ **Application-Based Questions**

### **Q1.** Illustrate a situation when an **inverted file will not be effective** as a storage option.  
> When the document collection is highly dynamic — i.e., frequent insertions or deletions occur — as updating the inverted file becomes expensive.

---

### **Q2.** Explain the **steps** to build an inverted index.  
> 1. Input documents.  
> 2. Tokenize and remove stop words.  
> 3. Generate frequency and position tables for each document.  
> 4. Combine and sort terms alphabetically.  
> 5. Merge entries across documents.  
> 6. Create a dictionary and postings list.  
> 7. Accept queries and retrieve relevant documents.

---

### **Q3.** What are the **main components** of an inverted index?  
> - **Vocabulary (Dictionary):** List of unique words.  
> - **Postings List:** List of documents and positions where each word appears.  

---

### **Q4.** What are the **advantages** of using inverted files?  
> - Efficient document retrieval.  
> - Faster search performance.  
> - Suitable for large and semi-static datasets.

---

### **Q5.** What are the **disadvantages** of inverted files?  
> - High storage requirements for large vocabularies.  
> - Slow updates for dynamic collections.  
> - Complex structure management.

---

### **Q6.** Why are addresses in an inverted file usually **kept in sorted order**?  
> To perform logical operations such as AND / OR efficiently in a single pass through both lists.

---

### **Q7.** What is the difference between **Sequential Searching** and **Indexed Searching**?  
> - Sequential: Scans all data linearly → slower for large datasets.  
> - Indexed: Uses inverted file or data structure → faster retrieval.  

---

### **Q8.** What data structures can be used for **vocabulary search**?  
> - Hashing  
> - Trie (Prefix tree)  
> - B-tree  
> - Sorted array with Binary Search  

---

### **Q9.** What is the function of the **threshold** in clustering or retrieval systems?  
> It defines the minimum similarity required for grouping documents or selecting results in retrieval.

---

### **Q10.** What are **stop words** and why are they removed?  
> Stop words are common words like *and*, *is*, *the* which carry little meaning and are removed to reduce index size and improve efficiency.

---

## 🧩 **Extra Technical Questions (For Higher CO/BT Levels)**

### **Q1.** Explain the process of **query evaluation** using an inverted index.  
> - Parse the query terms.  
> - Retrieve postings lists for each term.  
> - Perform set operations (AND, OR, NOT) based on the query type.  
> - Return the matching document IDs.

---

### **Q2.** What is the difference between **word position indexing** and **character position indexing**?  
> - **Word position indexing:** Indexes terms by word number (useful for phrase/proximity queries).  
> - **Character position indexing:** Indexes by character offset (useful for exact text matching).  

---

### **Q3.** What happens when a **new document** is added to the collection?  
> The inverted file must be updated — new terms are added to the vocabulary, and postings lists are extended, which is time-consuming.

---

### **Q4.** Mention any **real-world example** of inverted index usage.  
> Search engines like **Google**, **Elasticsearch**, or **Apache Lucene** use inverted indices for fast keyword-based retrieval.

---

✅ **In short:**  
These viva questions cover all the **conceptual, procedural, and application-level** aspects of Experiment No. 03, ensuring full preparation for both oral and written evaluation.

