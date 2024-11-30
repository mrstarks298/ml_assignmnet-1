# Machine Learning Algorithm Analysis for Question Categorization

## Project Objective
To analyze and compare multiple machine learning algorithms for categorizing university-related questions using different classification techniques.

## Algorithms Implemented

### 1. Naive Bayes Classifier
- **Approach**: Bag-of-words model
- **Key Characteristics**:
  * Assumes independence between features (words)
  * Calculates probability of category based on word frequencies
- **Performance**: 
  * Accuracy: 50%
  * Strengths: Simple, works well with large datasets
  * Limitations: Struggles with overlapping keywords

### 2. Logistic Regression
- **Approach**: TF-IDF Vectorization
- **Key Characteristics**:
  * Estimates probability of category membership
  * Handles more complex word relationships
- **Performance**:
  * Accuracy: 68%
  * Strengths: Better handling of diverse language
  * Potential for improvement through hyperparameter tuning

### 3. K-means Clustering (Unsupervised)
- **Approach**: Unsupervised learning
- **Key Characteristics**:
  * Groups questions based on content similarity
  * No predefined labels required
- **Insights**:
  * Identified natural question clusters
  * Useful for exploratory data analysis
  * Example Clusters:
    1. Admissions, fees, courses
    2. University history, campus info
    3. Facilities (hostels, mess)
    4. Faculty and academic staff

## Data Preparation
- **Source**: questions_answers.csv
- **Preprocessing**:
  * Lowercase standardization
  * Tokenization
- **Categories**:
  1. Admission Process
  2. Academics
  3. Facilities
  4. Placements and Internships
  5. University Details
  6. Student Life and Clubs
  7. Scholarship
  8. Policies and Rules
  9. Others

## Comparative Analysis

| Algorithm         | Accuracy | Strengths                      | Limitations                     |
|-------------------|----------|--------------------------------|---------------------------------|
| Naive Bayes       | 50%      | Simple, fast, works with large datasets | Poor with overlapping categories |
| Logistic Regression | 68%    | Handles complex language, more accurate | Requires careful feature engineering |
| K-means Clustering | Exploratory | Identifies natural groupings | Not supervised, lacks precise categorization |

## Future Work
1. Data Augmentation
   * Add more labeled data
   * Balance dataset across categories

2. Feature Engineering
   * Explore bigrams and trigrams
   * Capture more nuanced meaning

3. Advanced Techniques
   * Hyperparameter tuning
   * Deep learning models (BERT, Transformers)

## Conclusion
The Logistic Regression model demonstrated the best performance, providing a solid foundation for question categorization. K-means clustering offered valuable insights into question similarities, while Naive Bayes served as a baseline comparison.

## Research Insights
- Different machine learning algorithms show varying effectiveness in question categorization
- Logistic Regression outperformed Naive Bayes by capturing more complex language patterns
- Unsupervised learning (K-means) provides valuable insights into natural question groupings
- Further improvements can be achieved through advanced feature engineering and model tuning
