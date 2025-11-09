# 🌐 Viva Questions — Experiment No. 07  
### **Title:** Build a Web Crawler to Pull Product Information and Links from an E-commerce Website using Python  

---

## 🔹 Q1. What is a web crawler?
**Answer:**  
A **web crawler** is an automated program or bot that systematically browses the internet to collect and index data from web pages for search engines or data analysis.

---

## 🔹 Q2. What are other names for a web crawler?
**Answer:**  
Web crawlers are also called **spiders**, **bots**, **automatic indexers**, **web robots**, or **web scutters**.

---

## 🔹 Q3. What is the main function of a web crawler?
**Answer:**  
The main function of a web crawler is to **fetch web pages**, **extract useful information and hyperlinks**, and **index** them for easy searching by search engines.

---

## 🔹 Q4. How does a web crawler work?
**Answer:**  
1. Starts with a **list of seed URLs**.  
2. Downloads the HTML content of each page.  
3. **Extracts links** from the HTML.  
4. Adds new links to a **queue** for crawling.  
5. **Stores and indexes** content for future use.

---

## 🔹 Q5. What is the role of a crawler in search engines?
**Answer:**  
Crawlers help search engines like Google or Bing **discover, analyze, and index web pages**, allowing users to find information through search queries.

---

## 🔹 Q6. What is a seed URL?
**Answer:**  
A **seed URL** is the initial web address from which a web crawler starts exploring and collecting information.

---

## 🔹 Q7. What is a crawl frontier?
**Answer:**  
The **crawl frontier** is the list or queue of URLs that the crawler has discovered and plans to visit next.

---

## 🔹 Q8. What is robots.txt and why is it important?
**Answer:**  
`robots.txt` is a file on a website that gives instructions to web crawlers about **which pages or directories they are allowed or disallowed to access**.  
It helps prevent overloading servers and protects sensitive content.

---

## 🔹 Q9. What are the main challenges faced by web crawlers?
**Answer:**  
- Handling **duplicate content**  
- Managing **infinite dynamic URLs**  
- Respecting **robots.txt** rules  
- **Politeness delay** (avoiding too many requests too quickly)  
- Large **volume of pages** on the internet  

---

## 🔹 Q10. What is the difference between a web crawler and a web scraper?
**Answer:**  
- A **crawler** automatically navigates and collects data from multiple pages or websites.  
- A **scraper** extracts specific data (like prices or titles) from a **particular page or site**.

---

## 🔹 Q11. What is meant by meta crawler?
**Answer:**  
A **meta crawler** does not crawl the web directly. Instead, it sends user queries to **multiple search engines**, combines their results, and displays them together.  
Example: **Dogpile**, **Metacrawler**, **Excite**.

---

## 🔹 Q12. Give some examples of popular web crawlers.
**Answer:**  
- **Googlebot** – used by Google  
- **Bingbot** – used by Bing  
- **Yahoo! Slurp** – used by Yahoo  
- **DuckDuckBot** – used by DuckDuckGo  

---

## 🔹 Q13. What programming language is commonly used for building web crawlers?
**Answer:**  
**Python** is widely used due to its powerful libraries like **BeautifulSoup**, **Scrapy**, **Requests**, and **Selenium**.

---

## 🔹 Q14. What is the purpose of the “requests” library in Python?
**Answer:**  
It is used to **send HTTP requests** to web pages and **fetch HTML content** for parsing.

---

## 🔹 Q15. What is the role of BeautifulSoup in web crawling?
**Answer:**  
**BeautifulSoup** is a Python library used to **parse and extract data** from HTML and XML documents easily.

---

## 🔹 Q16. Why do we need a scheduler or queue in a crawler?
**Answer:**  
A **scheduler/queue** manages the order in which URLs are visited and ensures each page is crawled only once, avoiding repetition.

---

## 🔹 Q17. What is a multi-threaded downloader in web crawling?
**Answer:**  
It allows the crawler to **download multiple web pages simultaneously**, speeding up the crawling process.

---

## 🔹 Q18. What is the output of a web crawler?
**Answer:**  
The output is a **list of URLs**, **product details**, or **page data** extracted from the crawled web pages.

---

## 🔹 Q19. What are the applications of web crawlers?
**Answer:**  
- **Search engine indexing**  
- **Price comparison websites**  
- **Data mining and analytics**  
- **Market research**  
- **Monitoring website updates**

---

## 🔹 Q20. What are ethical considerations in web crawling?
**Answer:**  
- Respect `robots.txt` and site policies  
- Avoid server overload  
- Do not extract private or copyrighted data  
- Use polite crawling rates  

---

## ✅ **Conclusion**
A **web crawler** is an essential tool for collecting and indexing web data.  
By automating the extraction of URLs and page content, it forms the foundation of modern search engines and large-scale data analysis.

