# Airline Review Sentiment & Topic Analysis

## Project Overview
This project analyses 50,000 airline passenger reviews using Python, sentiment analysis, and topic modelling to uncover customer satisfaction trends, service quality issues, and major passenger concerns.

The project was developed as part of a business analytics assignment and demonstrates an end-to-end analytics workflow including data cleaning, exploratory data analysis, natural language processing, sentiment analysis, topic modelling, and business insight generation.

## Business Problem
Airlines receive large amounts of customer feedback through written reviews, ratings, and recommendations. While this data is valuable, it is difficult to interpret at scale because much of it is unstructured text.

This project addresses that problem by analysing airline reviews to answer key business questions such as:

- Which airlines perform best based on customer ratings?
- How does Qantas Airways compare to major competitors?
- Which airlines receive the most positive customer sentiment?
- What are the most common passenger concerns?
- What differences exist between high-performing and low-performing airlines?

The goal is to transform raw review data into insights that could support service improvement, customer experience strategy, and competitive benchmarking.


## Dataset
The analysis uses an airline review dataset containing approximately 74,000 reviews, from which a sample of 50,000 reviews was used for this project.

### Key variables include:
- **AirlineName**
- **OverallScore**
- **CabinType**
- **FoodRating**
- **EntertainmentRating**
- **GroundServiceRating**
- **Recommended**
- **Review**
- **DateFlown**

The dataset contains both structured variables (ratings, airline name, cabin type) and unstructured text data (customer reviews), making it suitable for both descriptive and NLP-based analysis.


## Project Objectives
This project was designed to:

1. Explore airline performance using customer ratings and recommendations  
2. Compare Qantas Airways and Jetstar Airways against top-performing airlines  
3. Apply sentiment analysis to understand emotional tone in reviews  
4. Use topic modelling to identify the main themes passengers discuss  
5. Generate practical business insights from customer feedback data  


## Methodology

### 1. Data Cleaning and Preparation
The dataset was first cleaned and prepared for analysis by:
- removing missing and inconsistent entries
- standardising text fields
- selecting relevant columns
- preparing review text for NLP tasks

### 2. Exploratory Data Analysis (EDA)
EDA was used to understand patterns in airline ratings and recommendations. This included:
- comparing airlines based on overall score
- examining service-related ratings such as food and entertainment
- analysing recommendation rates
- comparing cabin classes and airline performance trends

### 3. Sentiment Analysis
VADER sentiment analysis was applied to customer review text to classify emotional tone. This produced:
- compound sentiment scores
- positive, negative, and neutral sentiment measures
- airline-level sentiment comparisons
- aspect-based sentiment exploration for service-related language

### 4. Topic Modelling
Latent Dirichlet Allocation (LDA) was used to identify the major themes discussed across passenger reviews. Text preprocessing included:
- tokenisation
- stopword removal
- noun extraction / text filtering
- topic coherence evaluation

This helped uncover common discussion areas such as:
- delays
- baggage issues
- service quality
- refunds
- food and comfort
- airport and boarding experiences


## Tools and Technologies
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **NLTK**
- **Scikit-learn**
- **Gensim**
- **VADER Sentiment Analysis**


## Key Visualisations

### Airline Performance Comparison
This chart compares airlines based on overall customer scores and highlights the strongest performers in the dataset.

![Airline Performance Comparison](images/airline_performance_comparison.png)

### Qantas vs Jetstar Recommendation Analysis
This visual compares recommendation rates between Qantas Airways and Jetstar Airways across customer segments.

![Qantas vs Jetstar Recommendation Analysis](images/qantas_jetstar_recommendation.png)

### Sentiment Analysis by Airline
This graph shows average sentiment scores by airline, helping identify which airlines receive the most positive review language.

![Sentiment Analysis by Airline](images/sentiment_by_airline.png)

### Common Passenger Concerns
This visual highlights the most frequent concerns identified through topic modelling and review text analysis.

![Common Passenger Concerns](images/passenger_concerns_topics.png)

### Word Cloud / Topic Keywords
This visual summarises prominent terms that appear across customer reviews.

![Topic Keywords](images/topic_keywords_wordcloud.png)


## Key Findings

### 1. Top-performing airlines achieved stronger customer ratings
Some airlines consistently outperformed others across overall score and service-related metrics, indicating stronger customer satisfaction and service delivery.

### 2. Qantas underperformed compared to leading airlines
While Qantas remains a major airline, the analysis found that it lagged behind top-rated airlines in several performance dimensions, including customer sentiment and selected rating categories.

### 3. Jetstar showed weaker recommendation outcomes
Jetstar received relatively lower recommendation rates, particularly in Economy class, suggesting greater dissatisfaction among budget passengers.

### 4. Service quality strongly influenced customer sentiment
Review sentiment was closely tied to customer experiences involving staff behaviour, delays, support quality, and operational reliability.

### 5. Topic modelling revealed recurring pain points
Passenger concerns most commonly focused on:
- delays and cancellations
- baggage and luggage handling
- customer service interactions
- food quality and onboard experience
- refund and support processes

These findings suggest that operational efficiency and service responsiveness play a critical role in customer satisfaction.


## Business Insights
The findings from this project could support real airline decision-making in several ways:

- **Customer experience improvement:** identify recurring service failures
- **Competitive benchmarking:** compare airline performance against industry leaders
- **Operational focus:** prioritise delay reduction, baggage processes, and support response
- **Reputation management:** track sentiment trends to monitor brand perception
- **Segment analysis:** understand where dissatisfaction is strongest, such as Economy class customers


## Repository Structure
```bash
airline-review-sentiment-analysis/
│
├── data/
│   └── dataset.csv
│
├── notebooks/
│   └── airline_review_analysis.ipynb
│
├── images/
│   ├── airline_performance_comparison.png
│   ├── qantas_jetstar_recommendation.png
│   ├── sentiment_by_airline.png
│   ├── passenger_concerns_topics.png
│   └── topic_keywords_wordcloud.png
│
├── reports/
│   └── Nishant_Jawa_MIS780A1.pdf
│
├── requirements.txt
└── README.md
