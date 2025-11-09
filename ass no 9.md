# 🎯 Viva Questions — Experiment No. 09  
### **Title:** Case Study on Recommender System for a Product / Doctor / Product Price / Music  

---

## 🔹 Q1. What is a Recommender System?
**Answer:**  
A **Recommender System (RS)** is a software application that suggests relevant items (such as products, music, movies, or doctors) to users based on their **preferences, past interactions, or behaviors**.  
It helps users discover items of interest and reduces information overload.

---

## 🔹 Q2. What is the main aim of a recommender system?
**Answer:**  
The main aim is to **predict user preferences** and **recommend items** that users are likely to find useful or interesting, thereby improving user satisfaction and business sales.

---

## 🔹 Q3. Why are recommender systems important?
**Answer:**  
- They **reduce information overload**.  
- Improve **user experience and satisfaction**.  
- Help **increase sales** and **customer retention** for e-commerce platforms.  
- Provide **personalized** recommendations.

---

## 🔹 Q4. What are the main types of recommender systems?
**Answer:**  
1. **Collaborative Filtering (CF)**  
2. **Content-Based Filtering (CBF)**  
3. **Hybrid Recommender Systems**  
4. **Knowledge-Based Systems**  
5. **Demographic-Based Systems**

---

## 🔹 Q5. Explain Collaborative Filtering.
**Answer:**  
Collaborative Filtering recommends items to a user based on **the preferences of similar users**.  
It assumes that **users who agreed in the past tend to agree again in the future**.  
For example, if User A and User B have similar ratings for movies, movies liked by User A will be recommended to User B.

---

## 🔹 Q6. What are the two types of Collaborative Filtering?
**Answer:**  
1. **User-based CF:** Finds users similar to the target user and recommends what those users liked.  
2. **Item-based CF:** Finds items similar to the items a user has already liked and recommends them.

---

## 🔹 Q7. What is Content-Based Filtering?
**Answer:**  
Content-Based Filtering recommends items similar to those the user has liked before, based on **item features** such as genre, color, or keywords.  
For example, if you like a “romantic movie,” the system recommends other romantic movies.

---

## 🔹 Q8. What is a Hybrid Recommender System?
**Answer:**  
A **Hybrid Recommender System** combines **Collaborative Filtering** and **Content-Based Filtering** to overcome their individual limitations like the **cold-start problem** or **lack of data**.

---

## 🔹 Q9. What is Knowledge-Based Recommendation?
**Answer:**  
Knowledge-based systems recommend items based on **explicit knowledge about item features and user requirements**.  
For example, in a doctor recommender, the system matches the doctor’s specialization with the user’s health condition.

---

## 🔹 Q10. What are the main components of a recommender system?
**Answer:**  
- **User Profile:** Stores information about user preferences and behavior.  
- **Item Database:** Contains information about items to be recommended.  
- **Recommendation Engine:** The algorithm that matches users with items.  
- **Feedback System:** Collects explicit or implicit user feedback.

---

## 🔹 Q11. What are explicit and implicit feedbacks?
**Answer:**  
- **Explicit Feedback:** Direct user input (ratings, likes, reviews).  
- **Implicit Feedback:** Indirect user behavior (clicks, purchases, browsing time).

---

## 🔹 Q12. What is the main purpose of a recommender system in e-commerce?
**Answer:**  
To suggest **relevant products** to users, **increase sales**, **cross-sell** or **up-sell** items, and **enhance the overall shopping experience**.

---

## 🔹 Q13. Explain how Amazon uses a recommender system.
**Answer:**  
Amazon uses multiple recommenders such as:  
- **Customers who bought this also bought** (Collaborative Filtering)  
- **Book Matcher** (Content-Based)  
- **Amazon Eyes / Delivers** (Notification-based recommendations)  
These systems track user activity and preferences to personalize suggestions.

---

## 🔹 Q14. What is the Pearson Correlation Coefficient used for?
**Answer:**  
It measures the **similarity between two users’ preferences** in Collaborative Filtering.  
The value ranges between **–1 and +1**, where +1 indicates high similarity.

---

## 🔹 Q15. What are the advantages of Collaborative Filtering?
**Answer:**  
- No need for content analysis.  
- Produces serendipitous results (discovering unexpected items).  
- Learns from user behavior patterns.  
- Works across multiple domains.

---

## 🔹 Q16. What are the disadvantages of Collaborative Filtering?
**Answer:**  
- **Cold-start problem** (new user/item has no history).  
- **Data sparsity** (few ratings available).  
- **Scalability issues** for large datasets.  
- **Grey sheep problem** (users with unique tastes hard to match).

---

## 🔹 Q17. What are the advantages of Content-Based Filtering?
**Answer:**  
- No need for data from other users.  
- Can recommend even for new users (once preferences known).  
- Easy to interpret and explain recommendations.

---

## 🔹 Q18. What are the disadvantages of Content-Based Filtering?
**Answer:**  
- Requires detailed item features.  
- Cannot surprise users (limited to similar items).  
- Struggles with new items having no description.

---

## 🔹 Q19. What is the Hybrid Approach advantage?
**Answer:**  
- Combines strengths of CF and CBF.  
- Reduces **cold-start** and **sparsity** problems.  
- Provides more **accurate and diverse** recommendations.

---

## 🔹 Q20. What is the "Cold Start" problem?
**Answer:**  
It occurs when the system cannot make recommendations because **new users or new items** have insufficient data or interaction history.

---

## 🔹 Q21. What is meant by "Serendipity" in recommender systems?
**Answer:**  
Serendipity refers to the system’s ability to **recommend unexpected yet relevant items** that the user might not have discovered otherwise.

---

## 🔹 Q22. Define the term “User-Item Matrix.”
**Answer:**  
A **User-Item Matrix** represents user preferences for items in tabular form, where rows are users, columns are items, and cell values are ratings given by users to items.

---

## 🔹 Q23. What is the difference between Recommendation and Information Retrieval?
**Answer:**  
- **Information Retrieval:** Finds material that satisfies a known query (user knows what they want).  
- **Recommendation:** Suggests items users may **not know about**, based on predicted interests.

---

## 🔹 Q24. What evaluation metrics are used for recommender systems?
**Answer:**  
- **Precision**  
- **Recall**  
- **F1-score**  
- **Mean Absolute Error (MAE)**  
- **Root Mean Squared Error (RMSE)**

---

## 🔹 Q25. What is the difference between Collaborative and Content-Based Systems?
| Feature | Collaborative Filtering | Content-Based Filtering |
|----------|--------------------------|--------------------------|
| Basis | Similarity between users | Similarity between items |
| Data Needed | Ratings from many users | Item features |
| Cold Start | High problem | Lower problem |
| Surprise Factor | High | Low |

---

## 🔹 Q26. What is the role of a recommender system in healthcare (doctor recommendation)?
**Answer:**  
It recommends doctors or specialists based on **patients’ symptoms, ratings, and reviews**, improving **personalized healthcare suggestions**.

---

## 🔹 Q27. What is Social Recommender System?
**Answer:**  
A system that uses **social media data** or **social interactions** (likes, followers, friends) to recommend items.

---

## 🔹 Q28. What is the significance of “Neighbourhood-Based” algorithms?
**Answer:**  
Neighbourhood-based algorithms identify **similar users or items** and compute recommendations using **weighted averages of their ratings**.

---

## 🔹 Q29. What is the Knowledge-Based approach advantage?
**Answer:**  
- Works well when there is **no rating data**.  
- Provides **accurate, deterministic** results.  
- Ideal for **high-involvement purchases** (e.g., doctors, cars, houses).

---

## 🔹 Q30. How do recommender systems improve customer engagement?
**Answer:**  
They offer **personalized suggestions**, **reduce search time**, and **increase satisfaction**, leading to **repeat visits** and **higher sales**.

---

## ✅ **Conclusion**
Different types of recommender systems — **Collaborative, Content-Based, Hybrid, and Knowledge-Based** — were studied.  
Each system has specific **advantages and limitations**, and their application depends on the domain such as **e-commerce, healthcare, or entertainment**.

