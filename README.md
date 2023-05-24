# Spam-detection

Chose F1 score as the evaluation metric for the spam detection model due to the highly imbalanced nature of the data. Accuracy can be misleading in imbalanced datasets, where predicting the majority class dominates. F1 score considers both precision and recall, making it more suitable for evaluating the model's performance in identifying spam messages.

- Implemented different methods to create features for the spam detection model.
- Utilized Sparse Embeddings (TF-IDF) for feature representation, considering appropriate parameters such as min_df, max_df, max_features, and n-grams.
- Conducted Feature Engineering, focusing on distinguishing features between spam and regular emails. Examples include the count of words, characters, digits, exclamation marks, numbers, nouns, proper nouns, auxiliary verbs, adjectives, named entities, and spelling mistakes. Various techniques like counting and named entity recognition were applied to extract these features.
- Explored different combinations of Sparse Embeddings (TF-IDF) and Feature Engineering to find the best performing approach.
- Employed machine learning models such as Logistic Regression and XGBoost, with special attention given to handling the imbalanced dataset. Referenced the XGBoost tutorial for imbalanced classification to learn about appropriate techniques for model tuning and addressing the class imbalance.
- Used GridSearchCV for hyperparameter tuning to optimize model performance effectively.
- Observed that the Sparse Embeddings (TF-IDF) + Feature Engineering approach yielded the best F1 score compared to other feature combinations.
