
# Data Extraction for the Automation of the Validation Process of German Unit Certificates Using Deep Neural Networks

## Abstract

Efficiently extracting information from structured documents is a multidisciplinary task that requires a comprehensive understanding of both document layout and text. Visually rich document understanding techniques have the potential to increase organizational productivity by accelerating processes that rely on document-based information. In this work, I developed an artificial intelligence-based method to extract data from German unit certificates, with the goal of automating the crucial step of data extraction within a larger project. This project aims to streamline the process for photovoltaic (PV) owners to connect their systems to the grid and sell surplus electricity, contributing to reduced global energy costs and the promotion of clean energy. During this work, I gathered and labeled new data representing German unit certificates. To the best of my knowledge, no dataset containing German certificates has been explored in the context of visual document understanding. These newly collected documents have a complex tabular layout and are written in German. For data extraction from the certificates, three state-of-the-art transformer-based machine learning models for visually rich document understanding were fine-tuned using the newly compiled dataset. In this Thesis, the results of the fine-tuning on the three models were analyzed, and the best-performing model was optimized for further effectiveness. Additionally, two visual document understanding paradigms were compared: the OCR-based approach, which requires an external OCR engine, and the OCR-free approach, which does not rely on OCR. The results showed that the two OCR-based models outperformed the OCR-free model on the German unit certificates. The best-performing model achieved an F1 score of **96.5%** and an accuracy of **96.9%**, demonstrating highly promising results for automating data extraction from German unit certificates, with the potential to replace human involvement in the process.

## Dataset Characteristics

- **Number of certificates**: 89  
- **Number of samples**: 160 (due to multiple pages per certificate)  
- **Number of features to be extracted**: 14  




## Results
### LiLT(OCR-based) Results
**Performance**: Best performing model
<br />
Below is an example of entity recognition using the **LiLT** model:
<p align="center">
<img width="353" alt="test_lilt" src="https://github.com/user-attachments/assets/ae1fffcc-a2e6-4968-84ac-0fc8dafd6991">
<br />

### LayoutXLM(OCR-based) Results: 
- **Performance**: Second best performing model
  <br />
Below is an example of entity recognition using the **LayoutXLM** model:
<p align="center">
<img width="316" alt="test_layoutxlm" src="https://github.com/user-attachments/assets/3ecbbc18-44eb-4478-803e-e4094a61e91c"> 
<br />

### Donut(OCR-free) Results
- **Performance**: The least performing model
  <br />
Below is an example of entity recognition using the **Donut** model:
<p align="center">
<img width="316" alt="[156]"src="https://github.com/user-attachments/assets/b6d3dd57-75e8-497d-9696-4f6f20d062e0"> <img width="548" alt="r_donut" src="https://github.com/user-attachments/assets/34d009c5-47fc-4b49-bddb-bb8ee9cd0916">


---
This repository serves as a demonstration of the capabilities of these models on real-world document processing tasks.
