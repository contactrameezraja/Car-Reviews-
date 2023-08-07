Here is my assignment for the module, Applications of AI as part of my MS in Artificial Intelligence
---

### Car Review Assignment: Summary of Instructions

1. **Introduction to `CountVectorizer`:**
    - `CountVectorizer` from sklearn is employed to vectorize the reviews.
    - This module selects frequently occurring words/features/terms.
    - It produces a vector the size of the vocabulary. Each element represents the count of how many times a word appears in a review.
    - By setting the `binary` parameter to `False`, the actual counts of words are stored.

2. **Bag-of-Words Model Transformation:**
    - Use `fit_transform` to convert the texts in the training set to Bag-of-Words (BOW) form.
    - For the test set, only the `transform` function is used, indicating the vocabulary is only formed from the training set.

3. **Vector Creation for Test Set:**
    - Vectors for reviews in the test set must be of the same length as those in the training set.
  
4. **Vector Dimensions:**
    - Both training and test vectors share the same dimensions.

5. **Review Vectorization Example:**
    - Demonstrates how a review is turned into a vector showcasing the frequency of each word.

6. **Training the Model:**
    - For classification, the `MultinomialNB` classifier from sklearn is used.
    - This classifier operates on discrete features like the distinct words in the vocabulary.

7. **Evaluation Metrics and Visualization:**
    - The metrics used to understand the model's performance include the confusion matrix, precision, and recall.
    - A visual representation of the confusion matrix for the Naive Bayes classifier is provided.

8. **Changes for Task 2:**
    - For Task 2, two models are compared. Given the small dataset size, complex classifiers are avoided.
    - Improvements over Task 1 include:
      - Switching from Bag-of-Words to TF-IDF Vectorizer.
      - Implementing the concept of n-grams (unigrams and bigrams).
      - Changing the classifier from Naive Bayes to Logistic Regression.

9. **Text Cleaning:**
    - Further refine the text by eliminating tokens of length 1 or 2.
    
10. **Data Splitting:**
    - Dataset is divided into training (80%) and testing (20%) sets.
  
11. **TF-IDF Vectorization:**
    - Create the TF-IDF Vectorizer, considering both unigrams and bigrams.
    - The vector dimensions are expanded due to the inclusion of bigrams.

12. **Logistic Regression Model Definition:**
    - Parameters used:
        - `penalty`: L2
        - `max_iter`: Specified maximum iterations
        - `C`: Inverse of regularization strength
  
13. **Performance Comparison:**
    - The model for Task 2 shows improved performance compared to Task 1.
    - Improvements are observed in metrics like True Positives, True Negatives, precision, recall, and accuracy.

---
