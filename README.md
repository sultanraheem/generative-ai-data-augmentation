# Generative AI for Data Generation and Augmentation

## Overview
This project was part of the IBM **Generative AI for Data Engineers** lab. The primary focus was on leveraging the AI-assisted ability to generate realistic synthetic data. The synthetic data is generated when a pretrained generative model responds to either a prompt, create new data samples, or transfers learns on a given data set. In addition, it creates samples that can augment the existing data set while maintaining the statistical distribution and interpretability of the data set.

Trained data had an overall accuracy of 88.3% (91.1% with some optimizations).

<img width="1217" height="277" alt="image" src="https://github.com/user-attachments/assets/6f1c0a44-8e39-4c84-92c4-8ab61a733726" />

<img width="1291" height="549" alt="image" src="https://github.com/user-attachments/assets/5896c3e3-1569-4d1c-a0be-592f3db48b2b" />

<img width="1273" height="882" alt="image" src="https://github.com/user-attachments/assets/461eee71-c2f2-4bcd-961a-b08f572a9682" />

<img width="1079" height="443" alt="image" src="https://github.com/user-attachments/assets/80816e41-f722-448e-92f4-493563ab678b" />

<img width="868" height="574" alt="image" src="https://github.com/user-attachments/assets/949f2efb-cde9-427f-86e8-95dd61ba7ccd" />
<img width="1283" height="161" alt="image" src="https://github.com/user-attachments/assets/3721bdb1-ee10-4999-8344-7d54398b90f9" />

<img width="1155" height="837" alt="image" src="https://github.com/user-attachments/assets/cf25e71a-2c47-4e79-a63a-e37b6793f06e" />
<img width="1284" height="154" alt="image" src="https://github.com/user-attachments/assets/7275fd3c-83f8-4115-a5f0-db2ed1fe94fd" />

<img width="1211" height="820" alt="image" src="https://github.com/user-attachments/assets/c22986c2-371f-4305-a903-98b22d759207" />
<img width="1285" height="267" alt="image" src="https://github.com/user-attachments/assets/7c16a162-d9e7-4fe9-a946-ef30c0c74064" />

The goal was to explore how generative AI can be used for **synthetic data generation** and **data augmentation**, maintaining statistical distribution and interpretability within the dataset.

## Results for the Dataset

### Accuracy
- **Overall Accuracy**: 88.3% (91.1% with some optimizations)
  - **Univariate**: 96.6% (96.8%)
  - **Bivariate**: 89.9% (92.3%)
  - **Trivariate**: 78.4% (84.3%)

### Similarity
- **Cosine Similarity**: 0.98821 (0.99610)
- **Discriminator AUC**: 63.5% (50.0%)

### Distances
- **Identical Matches**: 0.0% (0.0%)
- **Average Distances**: 0.213 (0.212)
- **DCR Share**: 52.4% (50.0%)
- **NNDR Ratio**: 1.123 (1.000)

## Introduction to Generative AI

One of the key advantages of generative AI is its ability to create **realistic synthetic data**. The synthetic data is generated when a pretrained generative model responds to a prompt, creates new data samples, or transfers learning to a given dataset. 

In this project, the goal was to create data samples that augment the existing dataset while maintaining the **statistical distribution** and **interpretability** of the original dataset.

## Learning Objectives

In this lab, you will learn how to use a popular tool, **Mostly.ai**, to:
- Generate synthetic data samples.
- Transfer learning on a given dataset.
- Augment an existing dataset (in this case, an insurance dataset) with synthetic data.

## Dataset

The dataset used in this project includes **insurance_dataset.csv**:

insurance_dataset.csv

This dataset is a cleaned-up version of the **Medical Insurance Price Prediction dataset**, available under the CC0 1.0 Universal License on **Kaggle**.

## Steps to Reproduce

### 1. Download the Dataset
First, download the dataset to your machine. You'll need to upload this file to the interface in a later step. Click the link above to download it.

### 2. Open the Mostly.ai Website
Visit the **Mostly.ai** website at the following link:

- [Mostly.ai](https://mostly.ai/)

Once the page opens, you'll be directed to a user interface where you can start the data augmentation process.

### 3. Create an Account
Create a free account or log in using your **Gmail** account. After logging in, you will be directed to the main dashboard.

### 4. Upload the Dataset
- On the left-hand side of the interface, click **Generators**.
- Upload the CSV file of your dataset using the **Upload your data** option.
- After uploading, you'll see the filename displayed on the console. Then, click **Proceed**.

### 5. Data Configuration Settings
- You can modify the attributes or add parameters to the augmentation process. 
- For this lab, leave the settings as they are.
- Click **Configure models** to move on to model configuration settings.

### 6. Model Configuration Settings
- Modify the **max training time**, **number of epochs**, **sample size**, and other settings based on your needs.
- For this lab, use the **default settings**.
- Once you've finished, click **Start training** (top-right corner).

### 7. Model Training
- After training completes, you'll see an on-screen result similar to the one below.
- Click the **Model report** hyperlink to view the **Quality Assurance Report** in a separate tab.
- On the original page, click **Generate data** to use this trained model for generating synthetic data.

### 8. Create Synthetic Data
- Choose the **number of samples** you want to generate.
- Optionally, modify the statistical properties of the generated data.
- Keep the settings at their default values for the purpose of this lab.
- Click **Start generation** to begin the synthetic data generation.

### 9. Download the Synthetic Data
- Once the synthetic data generation completes, you'll see a page with a download link.
- Click **Download synthetic data** to download the newly created dataset.
- You can choose from a variety of available formats for the download.

## Conclusion
This project demonstrates how generative AI can be utilized to create synthetic data samples, augmenting an existing dataset while preserving its statistical characteristics. This process is highly valuable for improving model performance, especially when real-world data is scarce or sensitive.
