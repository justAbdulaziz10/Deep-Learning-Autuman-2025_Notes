# CS230 – Lecture 3: Introduction to Deep Learning  
**Date:** 2025-10-16  
**Instructor:** Andrew Ng  

---

## 🧠 Overview

In this lecture, Andrew Ng introduces the **core workflow of building a deep learning model**, breaking it down into clear, actionable stages — from problem definition to ongoing model maintenance.

---

## ⚙️ Steps to Build a Machine Learning Model

1. **Specify the Problem**  
   Clearly define what the model should accomplish.  
   > Example: Identify whether an image contains a human face.

2. **Get Data**  
   Collect and prepare the dataset for training and testing.  
   > Example: Gather labeled facial images from multiple angles and lighting conditions.

3. **Train the Model**  
   Feed the data into your chosen model architecture and optimize it using training algorithms (e.g., gradient descent).

4. **Deploy the Model**  
   Integrate the trained model into a real-world environment such as a web app, mobile app, or embedded device.

5. **Maintain the Model**  
   Continuously monitor, retrain, and update the model as new data becomes available to prevent performance degradation (data drift).

---

## 🔁 The Iterative Loop (Steps 2–4)

Between **data collection**, **model design**, and **training**, there’s an iterative process:
Design → Train → Analyze → (Repeat)

- **Design:** Choose the model architecture (CNN, RNN, Transformer, etc.)
- **Train:** Fit the model to your data and tune hyperparameters.
- **Analyze:** Evaluate performance, identify weaknesses, and adjust design or dataset accordingly.

This feedback loop continues until the model achieves acceptable accuracy and generalization.

---

## 🧍‍♂️ Example: Facial Recognition Model

To build a **facial recognizer**, you typically need **at least 15,000 labeled photos** for robust performance.  
This ensures:
- Diversity in lighting, angles, and expressions  
- Better generalization to unseen faces  
- Reduced overfitting  

---

## 🧩 Summary Table

| Step | Description | Example |
|------|--------------|----------|
| 1. Specify Problem | Define the task | Detect faces in photos |
| 2. Get Data | Collect images | Gather 15k+ labeled photos |
| 3. Train Model | Use CNN or similar | Train with backpropagation |
| 4. Deploy Model | Integrate in app | Use in phone’s photo unlock |
| 5. Maintain Model | Monitor & retrain | Update with new user data |

---

## 🧭 Key Insight

> “Deep learning is not a one-shot process — it’s a continuous loop of learning, refining, and adapting.”  
> — *Andrew Ng*

---
