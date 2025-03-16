# Possible Project Ideas

## Food Nutrition Detector

### Where can we find datasets?
- [Kaggle](https://www.kaggle.com/)
- [Hugging Face](https://huggingface.co/datasets)
- [Perplexity](https://www.perplexity.ai/)
- [Arxiv](https://arxiv.org/)

### Available Datasets:
- [Nutrition5k - Google Research](https://github.com/google-research-datasets/Nutrition5k)
- [Nutrition5k Food Name - Hugging Face](https://huggingface.co/datasets/TeeA/nutrition5k-food-name-gemini)

---

## Voxel Food Nutrition Detector

**Project Repository & Resources:**
- Hugging Face Model:
- [GitHub Repository](#)
- [Google Colab](#)
- [Presentation Slides](#)

### Dataset Format:
- VOC, COCO, Image Classification Directory Tree

### Nutritional Facts Dataset:
- [Kaggle - Nutritional Values for Common Foods and Products](https://www.kaggle.com/datasets/trolukovich/nutritional-values-for-common-foods-and-products)

---

## Presentation Slides

### **Slide 1: Problem Statement**
Millions of people worldwide have dietary restrictions due to health conditions such as diabetes, food allergies, celiac disease, or chronic kidney disease. These individuals must carefully monitor their intake of specific nutrients and ingredients to maintain their health. However, when dining at restaurants, obtaining accurate and detailed nutritional information about meals is often difficult, especially for those with unique dietary needs.

Our application will leverage image recognition and AI-powered food analysis to:
- Estimate macronutrient and micronutrient content
- Detect potential allergens
- Highlight ingredients that may be restricted based on the user's dietary profile

This system will empower individuals with dietary restrictions to make informed choices about their meals, improving their ability to dine out safely and confidently.

To address this challenge, we propose developing a computer vision-based application that allows users to take a picture of their meal and receive detailed nutritional information in real time. This application currently leverages a visual language model, **Moondream2**.

---

### **Slide 2: Dataset Selection**
Initially, we considered using **Nutrition5k**, but its large size (181.4GB) posed significant limitations. The dataset contained valuable information, such as per-ingredient mass and macronutrient breakdown (fat, protein, carbohydrates), which could have simplified development. However, the presence of video data made it difficult to use.

As a result, we pivoted to a **Hugging Face dataset** that includes:
- `dish_id`
- `food_name`
- `dish_image`

Although this dataset was not formatted for **Voxel51**, we adapted it accordingly. However, we encountered several challenges during implementation, leading to multiple project adjustments throughout the hackathon.

---

### **Slide 3: Exploring Visual Language Models (VLMs)**
One of the most exciting aspects of our hackathon project was experimenting with **Visual Language Models (VLMs)**, which combine **Computer Vision** and **Natural Language Processing** to analyze images and generate text-based insights.

We aimed to use models such as **Janus** and **Moondream2** for:
- **Image Captioning**
- **Visual Question Answering (VQA)**
- **Object Detection on Voxel**

For VQA, we wanted to analyze food images by asking questions such as:
- **What percentage of each food item is on the plate?**
- **What is the estimated nutritional content?**

Unfortunately, we couldn’t fully test these ideas, but they remain exciting areas for future exploration.

---

### **Slide 4: Future Steps**
Going forward, we would like to:
- Run additional **AI models** to refine our predictions
- Improve our **nutritional mass estimation** using surface area calculations
- Integrate **Hugging Face zero-shot object detection** to identify food items more accurately

With further development, we could calculate food mass based on **detected surface area and density**, allowing for more precise **nutritional analysis**. Combined with **user-provided medical data**, this system could help determine whether a particular food is safe for consumption.

Ultimately, we aimed to convert surface area calculations into grams (we’ll figure that part out later 🤣) and cross-reference nutritional data to provide **macro and micronutrient breakdowns**.

---

## Conclusion
This project was an exciting deep dive into the intersection of **AI, Computer Vision, and Nutrition Analysis**. While we faced challenges and pivots, we gained valuable insights into **VLMs, dataset curation, and real-world AI applications**. We look forward to continuing this journey and refining our approach in the future!

---
