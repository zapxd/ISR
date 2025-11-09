# 🌦️ Viva Questions — Experiment No. 08  
### **Title:** Write a program to find the live weather report (temperature, wind speed, description, and weather) of a given city using Python  

---

## 🔹 Q1. What is the main objective of this experiment?
**Answer:**  
The main objective is to **fetch live weather information** such as **temperature**, **wind speed**, **pressure**, **humidity**, and **description** of a given city using the **OpenWeatherMap API** and Python.

---

## 🔹 Q2. What is OpenWeatherMap?
**Answer:**  
**OpenWeatherMap** is a **web-based service** that provides **weather data, forecasts, and current conditions** for cities around the world through a free **API** (Application Programming Interface).

---

## 🔹 Q3. What is an API key and why is it needed?
**Answer:**  
An **API key** is a unique identifier used to **authenticate your requests** to the OpenWeatherMap server.  
It ensures that only registered users can access the API and helps monitor usage.

---

## 🔹 Q4. Which Python modules are used in this experiment?
**Answer:**  
- **requests** – to send HTTP requests and receive responses from the API.  
- **json** – to parse and extract weather information from the JSON response.  
- (optional) **pprint** – for neatly formatted output.

---

## 🔹 Q5. What is JSON and why is it used here?
**Answer:**  
**JSON (JavaScript Object Notation)** is a lightweight data-interchange format used to store and exchange data between client and server.  
In this experiment, it is used to **parse the weather data** received from the OpenWeatherMap API.

---

## 🔹 Q6. What is the base URL used in this experiment?
**Answer:**  
The base URL for fetching weather data is:  
```
https://api.openweathermap.org/data/2.5/weather?
```

---

## 🔹 Q7. What are the key parameters passed to the OpenWeatherMap API?
**Answer:**  
- `q` → City name (e.g., Pune)  
- `appid` → User’s API key  
- `units` → Temperature units (metric for Celsius, imperial for Fahrenheit)

---

## 🔹 Q8. Explain the working of the program step-by-step.
**Answer:**  
1. Import the required modules (`requests`, `json`).  
2. Define the **base URL** and **API key**.  
3. Ask the user for a **city name**.  
4. Append the city name and API key to the base URL.  
5. Send a **GET request** using `requests.get()`.  
6. Convert the response to JSON using `.json()`.  
7. Extract and print temperature, humidity, pressure, and weather description.

---

## 🔹 Q9. What happens if the city name entered is incorrect?
**Answer:**  
If the city name is invalid, the API returns an **error code (404)** and a message such as **“city not found”**.  
The program handles it by displaying an error message to the user.

---

## 🔹 Q10. What is the purpose of using `response.status_code` in the program?
**Answer:**  
`response.status_code` checks whether the HTTP request was successful.  
- `200` → Success  
- `404` → City not found  
- `401` → Invalid API key  

---

## 🔹 Q11. How is temperature represented in the API response?
**Answer:**  
Temperature is represented in **Kelvin** by default.  
We can use the `units=metric` parameter to get the temperature in **Celsius**.

---

## 🔹 Q12. What are the main weather parameters extracted from the API?
**Answer:**  
- **Temperature**  
- **Humidity**  
- **Pressure**  
- **Wind speed**  
- **Weather description**

---

## 🔹 Q13. What is the significance of using the `requests.get()` method?
**Answer:**  
The `requests.get()` method sends an **HTTP GET request** to the given API URL and retrieves the **server’s response**, which contains the weather data.

---

## 🔹 Q14. What is the difference between requests and urllib modules?
**Answer:**  
- **requests** is simpler and more user-friendly for handling HTTP requests.  
- **urllib** is a built-in library but requires more steps to handle URLs and responses.

---

## 🔹 Q15. What is the output of this program?
**Answer:**  
The program displays live weather information such as:  
```
Temperature: 26.4°C  
Wind Speed: 2.1 m/s  
Description: Clear sky  
Weather: Clear  
```

---

## 🔹 Q16. What is the purpose of the `try-except` block in the code?
**Answer:**  
It handles **runtime errors**, such as entering an invalid city name or API issues, and prevents the program from crashing.

---

## 🔹 Q17. What is the role of the pprint library?
**Answer:**  
The `pprint` (Pretty Print) library is used to **display JSON data in a readable format**, especially when debugging.

---

## 🔹 Q18. How can you modify this program to predict weather for the next few days?
**Answer:**  
Use the **OpenWeatherMap “forecast” API endpoint**:  
```
https://api.openweathermap.org/data/2.5/forecast?
```  
This provides **5-day / 3-hour interval forecasts** for the specified city.

---

## 🔹 Q19. What are some applications of weather data APIs?
**Answer:**  
- **Weather forecasting websites**  
- **Agricultural monitoring**  
- **Travel and logistics planning**  
- **Smart home automation (IoT)**  
- **Disaster management systems**

---

## 🔹 Q20. What are the limitations of the free OpenWeatherMap API?
**Answer:**  
- Limited to **60 requests per minute**.  
- May not include **advanced features** like hourly forecast or radar data.  
- Requires an **active internet connection**.  

---

## ✅ **Conclusion**
Using the **OpenWeatherMap API** with Python enables us to fetch **real-time weather data** for any city easily.  
It demonstrates practical use of **APIs, HTTP requests, and JSON parsing** in real-world applications.

