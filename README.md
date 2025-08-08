# 📱 Application Review Comments Sentiment Analysis

This project performs **sentiment analysis** on mobile application reviews to understand user opinions, detect trends, and extract actionable business insights.  
It uses **Natural Language Processing (NLP)** and **data visualization techniques** to transform raw user feedback into meaningful sentiment metrics.

---

## 📊 Project Overview

Mobile applications receive thousands of reviews daily. These reviews are a goldmine for:
- Understanding **user satisfaction**.
- Detecting **product pain points**.
- Identifying **feature requests** and **positive highlights**.
- Tracking **brand reputation trends** over time.

In this project, we:
1. **Collected application review data.**
2. **Cleaned & transformed** the text data.
3. Performed **sentiment scoring** (positive, negative, neutral).
4. Conducted **EDA (Exploratory Data Analysis)**.
5. Created **visualizations** for key insights.
6. Interpreted results from a **business perspective**.

---

## 📂 Dataset Details

The dataset contains **user reviews** of a mobile application with the following key columns:
- `Review` → The actual text of the user's feedback.
- `Rating` → User-given rating (1–5 stars).
- `Date` → Review date.
- `Sentiment` → Predicted sentiment (Positive, Negative, Neutral).
- `Polarity` → Numeric score from -1 (negative) to +1 (positive).
- `Subjectivity` → How subjective or opinion-based the review is.

**Sample Data:**
| Review                              | Rating | Date       | Sentiment | Polarity | Subjectivity |
|--------------------------------------|--------|-----------|-----------|----------|--------------|
| "The app is amazing and very useful" | 5      | 2025-07-15| Positive  | 0.85     | 0.70         |
| "Crashes often. Very disappointed"  | 1      | 2025-06-22| Negative  | -0.90    | 0.80         |

---

## 🛠 Data Cleaning & Transformation

The raw data underwent several preprocessing steps:

1. **Text Cleaning**
   - Removed special characters, numbers, and punctuation.
   - Converted all text to lowercase.
   - Removed extra whitespaces.

2. **Stopword Removal**
   - Eliminated common words (`the`, `is`, `and`, etc.) that do not add sentiment value.

3. **Tokenization & Lemmatization**
   - Tokenized the reviews into words.
   - Converted words to their base form (e.g., "running" → "run").

4. **Sentiment Scoring**
   - Used **TextBlob** to calculate:
     - **Polarity** → Range (-1 to +1)
     - **Subjectivity** → Range (0 to 1)
   - Classified sentiment:
     - Polarity > 0 → Positive
     - Polarity < 0 → Negative
     - Polarity = 0 → Neutral

---

## 📈 Exploratory Data Analysis (EDA)

We explored:
- **Distribution of ratings**.
- **Sentiment distribution**.
- **Most frequent words** in each sentiment category.
- **Trends over time** (sentiment vs. date).

**Key Findings:**
- Majority of reviews were **positive**, but **negative reviews highlighted performance issues** like crashes and slow loading.
- **Neutral reviews** often requested small feature improvements.
- Peak review activity happened around **major app updates**.

---

## 📊 Visualizations

We used **Matplotlib & Seaborn** to create:
1. **Rating Distribution Bar Chart** – Shows user rating spread.
2. **Sentiment Count Plot** – Displays count of positive, negative, neutral reviews.
3. **Word Clouds** – Highlights frequent keywords per sentiment:
   - Positive → "love", "easy", "great", "amazing".
   - Negative → "crash", "error", "slow", "bug".
4. **Time Series Sentiment Trend** – Shows changes in sentiment over months.
5. **Boxplot of Ratings vs. Polarity** – Detects correlation between star rating & sentiment score.

---

## 💼 Business Insights

From a business perspective:
- **Positive themes** → Users love ease of use and design.
- **Negative themes** → Technical issues like crashes impact ratings heavily.
- **Opportunities**:
  - Fixing performance bugs could significantly improve ratings.
  - Adding most-requested features could increase engagement.
- **Trend analysis** shows a sentiment drop after specific updates — indicates possible **update-related issues**.

---

## 🛠 Tech Stack

- **Python**
- **Libraries**:
  - `pandas` → Data manipulation
  - `numpy` → Numerical computation
  - `matplotlib`, `seaborn` → Data visualization
  - `wordcloud` → Keyword visualization
  - `textblob` → Sentiment analysis

---


