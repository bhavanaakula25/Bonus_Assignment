# Bonus_Assignment
# Bonus Assignment – Question Answering with Transformers & Conditional GAN

**Name:** Bhavana Akula  
**Course:** CS5720 – Neural Networks and Deep Learning  
**University:** University of Central Missouri  
**Assignment:** Bonus Assignment  
**Points:** 1  
**Submission Includes:** Source Code (Jupyter Notebook), README File, Video Link

---

## 📌 Overview

This assignment is divided into two parts:

1. **Question Answering with Transformers** – Utilizing Hugging Face's `transformers` library to create a question-answering system using both default and custom pre-trained models.
2. **Digit-Class Controlled Image Generation using Conditional GAN (cGAN)** – Modifying a basic GAN to conditionally generate MNIST digits based on class labels (0–9).

---

## ✅ Requirements

Ensure the following Python libraries are installed:

```bash
pip install transformers torch torchvision matplotlib
```

---

## 📖 Part 1: Question Answering with Transformers

### Task Summary:

- Used `transformers.pipeline` for question answering.
- Tested with:
  - **Default pre-trained model**
  - **Custom model**: `deepset/roberta-base-squad2`
- Created and tested on a custom context with two questions.

### Sample Output:

- Example Answer: `'Charles Babbage'`
- Confidence Score: `> 0.70`
- Includes valid `start` and `end` indices

---

## 🎨 Part 2: Conditional GAN (cGAN) for MNIST

### Task Summary:

- Modified GAN architecture to condition generator and discriminator on digit labels.
- Input:
  - Generator: Noise vector + label embedding
  - Discriminator: Image + label embedding
- Trained on the MNIST dataset.
- Generated one row of digits for labels 0–9.

### Visual Results:

- Each row of images corresponds to digits 0 through 9.
- Output digit shape: 28x28
- Training shows improved label-specific digit generation.

---

## 🧠 Short Answers

**Q1: How does a Conditional GAN differ from a Vanilla GAN?**  
A Conditional GAN takes an additional label as input, allowing it to generate outputs based on class control.  
**Real-world Example**: Generating specific clothing types (e.g., shirts, pants) using labeled fashion images.

**Q2: What does the Discriminator learn in an image-to-image GAN? Why is pairing important?**  
It learns to distinguish real vs. fake image pairs (e.g., sketches → photos).  
Pairing is crucial to ensure the generator learns correct mapping and not just produce random outputs.

---

## 💬 Comments

- Code has been properly commented.
- Each section in the notebook corresponds to assignment tasks.

---

## 🔗 Submission Links

- **GitHub Repository**:https://github.com/bhavanaakula25/Bonus_Assignment.git


---

## 📂 Files Included

- `Bonus_Assignment.ipynb` – Source Code
- `README.md` – This file
