# Fake News Detection Using Text Mining

This repository contains a comprehensive text mining project focused on the automatic classification of fake and real news articles. The analysis integrates natural language processing (NLP), traditional machine learning, and deep learning methodologies to identify linguistic patterns and contextual signals associated with deceptive content.

## Objective
The primary goal of this project is to develop and evaluate classification models that accurately distinguish between real and fake news using text data. This work addresses the growing need for automated solutions to mitigate the spread of misinformation across digital platforms.

## Tools & Technologies
- **KNIME Analytics Platform** – for data preprocessing, feature engineering, and labeling
- **RapidMiner AI Studio** – for model training, evaluation, and comparison
- **Text Mining Techniques** – including tokenization, stopword removal, stemming, TF-IDF, and n-gram extraction
- **Machine Learning Models**:
  - Naïve Bayes
  - Deep Learning (Multilayer Perceptron)
  - Random Forest
  - Gradient Boosted Trees

## Dataset
- Source: [Kaggle – Fake and Real News Dataset](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset)
- Contents: News articles labeled as either **fake** or **real**
- Format: Combined CSV file after merging, cleaning, and labeling using KNIME

## Methodology
1. **Data Preprocessing** in KNIME:
   - Merging real and fake news datasets
   - Text cleaning: tokenization, lowercasing, stopword removal
   - Feature extraction via TF-IDF and n-grams
2. **Model Training & Evaluation** in RapidMiner:
   - Comparison across four algorithms
   - Hyperparameter tuning and stratified train-test splitting
   - Evaluation using Accuracy, Precision, Recall, and F1-Score

## Results Summary
| Model                  | Accuracy | Precision | Recall | F1-Score |
|------------------------|----------|-----------|--------|----------|
| Naïve Bayes            | 88%      | 86%       | 86%    | 85%      |
| Random Forest          | 59%      | 55%       | 52%    | 54%      |
| Deep Learning (MLP)    | 92%      | 90%       | 91%    | 91%      |
| Gradient Boosted Trees | 85%      | 83%       | 84%    | 83%      |

**Conclusion**: The Deep Learning model outperformed all others in accuracy and consistency. Naïve Bayes served as a reliable baseline. Random Forest showed limitations with high-dimensional textual data.

## Repository Contents
- `Text_Mining_Project_Report_Cha.pdf` – Full project report detailing methodology, analysis, and findings
- `Text_Mining.csv` – Preprocessed dataset used for training and testing
- `Fake_News_Detection.knwf` – KNIME workflow file

## Business Impact
This solution has potential applications in:
- **Social media monitoring**: Automated flagging of suspicious content
- **Editorial support**: Assisting newsrooms in early detection of fabricated stories
- **Government & policy**: Monitoring disinformation campaigns in real time
- **Financial sectors**: Detecting misinformation that may affect market perception

## Author
**Soyeong (Selena) Cha**  
Master’s Student in Data Analytics, Seattle Pacific University  
[LinkedIn](https://www.linkedin.com/in/selena-cha) • [Tableau Portfolio](https://public.tableau.com/app/profile/soyeong.cha/vizzes)
