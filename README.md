# **Food Delivery Sentiment Analysis**

## **Project Overview**
This repository contains a comprehensive analysis of customer sentiment for a food delivery service. The project leverages Natural Language Processing (NLP) and emotion lexicon techniques to extract valuable insights from customer reviews, guiding strategic recommendations for service improvement [file:1].

## **Full Workflow**

### **Step 1: Import Essential Libraries**
Imports all necessary Python libraries for data handling, preprocessing, sentiment analysis, and visualization:
- pandas, numpy
- nltk (for tokenization and stopwords)
- re (for text cleanup)
- matplotlib, seaborn
- NRCLex (for emotion analysis)

### **Step 2: Data Acquisition**
Reads reviews from Excel files (`reviews1000fooddelivery.xlsx` and `REVIEWSPRO.xlsx`). The structure ensures all subsequent steps operate on a clean, unified dataset [file:1].

### **Step 3: Text Preprocessing**
- Converts review text to lowercase.
- Removes non-alphabetic characters.
- Tokenizes sentences into words.
- Removes stopwords to focus analysis on impactful words.
- Recombines tokens into processed review text.

### **Step 4: Emotion and Sentiment Extraction**
- Utilizes NRCLex to extract emotion scores (joy, trust, anticipation, surprise, anger, fear, sadness, disgust) for each review.
- Determines the dominant emotion in every review via frequency analysis.
- Maps complex emotion profiles into clear sentiment classes: **Positive**, **Negative**, or **Neutral**.

### **Step 5: Sentiment Classification**
Defines custom logic for sentiment assignment:
- If positive emotion counts exceed negatives, label as *Positive*.
- If negatives dominate, label as *Negative*.
- If both counts are balanced, default to *Neutral* [file:1].

### **Step 6: Results and Visualization**
- Produces summary statistics and distribution charts for dominant emotions and sentiment classes.
- Outputs sample reviews alongside predicted sentiment for validation.
- Uses matplotlib and seaborn to visualize sentiment trends and identify common topics/themes impacting customer experience.

## **Installation**

**Prerequisites:**  
- Python 3.7 or higher
- Jupyter Notebook or compatible IDE

**Dependencies:**  
pip install pandas numpy nltk matplotlib seaborn nrclex


## **Usage Guide**
1. Download and place all relevant Excel files into the working directory.
2. Launch the notebook:
    ```
    jupyter notebook Food-Delivery-Sentiment.ipynb
    ```
3. Run cells sequentially to reproduce the workflow and inspect results.
4. Examine visualizations and summary tables for actionable insights.

## **Business Analyst Recommendations**
As a business analyst, below are strategic recommendations for the food delivery manager based on sentiment findings:

- **Prioritize Delivery Speed and Food Quality:** Positive sentiments are most frequent when delivery is fast and food is hot and flavorful. Maintain high standards in these areas to maximize customer satisfaction [file:1].
- **Address Consistency Issues:** Negative reviews tend to focus on late deliveries and missing items. Invest in operational tracking and driver training to minimize these pain points [file:1].
- **Enhance Communication:** Trust and anticipation are strong positive emotions. Frequent updates and confirmations with customers (e.g., notification when food is on its way) increase positive impressions.
- **Resolve Complaints Promptly:** Demonstrate responsiveness to negative experiences. A process for fast complaint resolution will improve neutral and negative sentiments.
- **Monitor and Innovate:** Use ongoing sentiment analysis to identify trends in customer feedback, allowing for early detection of new issues or opportunities.

Implementing these recommendations will foster sustained improvements in customer experience, loyalty, and competitive advantage for the food delivery business [file:1].
