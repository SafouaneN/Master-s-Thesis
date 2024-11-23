
# Data Extraction for the Automation of the Validation Process of German Unit Certificates using Deep Neural Networks

## Abstract

Efficiently extracting information from structured documents is a multidisciplinary task that requires a comprehensive understanding of both document layout and text. Visually rich document understanding techniques have the potential to increase organizational productivity by accelerating processes that rely on document-based information. In this work, I developed an artificial intelligence-based method to extract data from German unit certificates, with the goal of automating the crucial step of data extraction within a larger project. This project aims to streamline the process for photovoltaic (PV) owners to connect their systems to the grid and sell surplus electricity, contributing to reduced global energy costs and the promotion of clean energy. During this work, I gathered and labeled new data representing German unit certificates. To the best of my knowledge, no dataset containing German certificates has been explored in the context of visual document understanding. These newly collected documents have a complex tabular layout and are written in German. For data extraction from the certificates, three state-of-the-art transformer-based machine learning models for visually rich document understanding were fine-tuned using the newly compiled dataset. In this Thesis, the results of the fine-tuning on the three models were analyzed, and the best-performing model was optimized for further effectiveness. Additionally, two visual document understanding paradigms were compared: the OCR-based approach, which requires an external OCR engine, and the OCR-free approach, which does not rely on OCR. The results showed that the two OCR-based models outperformed the OCR-free model on the German unit certificates. The best-performing model achieved an F1 score of **96.5%** and an accuracy of **96.9%**, demonstrating highly promising results for automating data extraction from German unit certificates, with the potential to replace human involvement in the process.



## Results
### LiLT(OCR-based) Results: Best performing model
Below is an example of the entitys recongintion using the **LiLT** model:
<p align="center">
<img width="353" alt="test_lilt" src="https://github.com/user-attachments/assets/ae1fffcc-a2e6-4968-84ac-0fc8dafd6991">
<br />

### LayoutXLM(OCR-based) Results: Second best performing model
Below is an example of the entitys recongintion using the **LayoutXLM** model:
<p align="center">
<img width="316" alt="test_layoutxlm" src="https://github.com/user-attachments/assets/3ecbbc18-44eb-4478-803e-e4094a61e91c">
<br />

### Donut(OCR-free) Results
Below is an example of bounding box detection using the **Donut** model (image placeholder):
<img src="link_to_image1" alt="Image 1" width="300"/> <img src="link_to_image2" alt="Image 2" width="300"/>

---
This repository serves as a demonstration of the capabilities of these models on real-world document processing tasks.
