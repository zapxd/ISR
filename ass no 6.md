# 🎨 Viva Questions — Experiment No. 06  
### **Title:** Program for Feature Extraction in 2D Color Images  

---

## 🔹 Q1. What is feature extraction in image processing?
**Answer:**  
Feature extraction is the process of identifying and isolating important features or attributes of an image (like color, texture, or shape) that can be used for image analysis or classification.

---

## 🔹 Q2. What are the main types of image features?
**Answer:**  
The main types of image features are:  
- **Color features**  
- **Texture features**  
- **Shape features**  
- **Edge features**

---

## 🔹 Q3. What is a color model?
**Answer:**  
A **color model** is a mathematical model describing the way colors can be represented as tuples of numbers.  
For example:  
- **RGB** (Red, Green, Blue)  
- **HSV** (Hue, Saturation, Value)  
- **CMYK** (Cyan, Magenta, Yellow, Black)

---

## 🔹 Q4. What is the RGB color model?
**Answer:**  
RGB stands for **Red, Green, and Blue** — the three primary colors of light.  
It is an **additive model**, meaning that colors are created by combining these three colors with varying intensity.

---

## 🔹 Q5. Why is RGB model commonly used?
**Answer:**  
Because it matches how digital devices like monitors and cameras **capture and display colors**, making it ideal for image processing applications.

---

## 🔹 Q6. What is a color histogram?
**Answer:**  
A **color histogram** represents the **distribution of colors** in an image by plotting the number of pixels corresponding to each color intensity value.

---

## 🔹 Q7. What information can you get from a histogram?
**Answer:**  
It provides information about:  
- **Brightness and contrast** of the image  
- **Color distribution**  
- **Dominant colors** and **image balance**

---

## 🔹 Q8. What are the different types of histograms in image processing?
**Answer:**  
1. **Gray level histogram** – based on pixel intensity (black to white).  
2. **Color histogram** – separate histograms for R, G, and B channels.  
3. **Normalized histogram** – scaled version for comparison between images.

---

## 🔹 Q9. How can you extract R, G, and B components from an image?
**Answer:**  
Each pixel contains three values (R, G, B).  
They can be extracted by separating the color channels:  
- R = image[:,:,0]  
- G = image[:,:,1]  
- B = image[:,:,2]  
*(Or in Java, using methods like `getRed()`, `getGreen()`, `getBlue()` on pixel objects.)*

---

## 🔹 Q10. What is the role of color models in feature extraction?
**Answer:**  
Color models help **represent and interpret image data** consistently. They allow extraction of specific color-based features useful for classification, recognition, and retrieval.

---

## 🔹 Q11. What are some common image file formats?
**Answer:**  
- **BMP** – Bitmap image  
- **JPG / JPEG** – Compressed image format  
- **PNG** – Lossless compression format  
- **TIFF** – High-quality image format  

---

## 🔹 Q12. What are the applications of feature extraction?
**Answer:**  
Feature extraction is used in:  
- Image classification  
- Object detection  
- Face recognition  
- Medical imaging  
- Content-based image retrieval (CBIR)

---

## 🔹 Q13. What is the use of an image histogram in processing?
**Answer:**  
Image histograms help in:  
- **Enhancing image contrast**  
- **Equalizing brightness**  
- **Thresholding and segmentation**  
- **Analyzing overall image composition**

---

## 🔹 Q14. How can you identify whether an image is dark or bright using a histogram?
**Answer:**  
- If the histogram is **shifted to the left**, the image is **dark**.  
- If the histogram is **shifted to the right**, the image is **bright**.  

---

## 🔹 Q15. Explain the significance of texture features.
**Answer:**  
Texture features represent **surface patterns and spatial arrangements** of pixel intensities — useful in identifying materials, surfaces, or patterns in an image.

---

## ✅ **Conclusion**
Feature extraction identifies useful properties like color and texture from images.  
Color histograms help visualize the distribution of pixel intensities, aiding in analysis, classification, and enhancement of digital images.

