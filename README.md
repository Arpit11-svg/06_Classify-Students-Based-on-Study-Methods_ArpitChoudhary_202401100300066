# 06_Classify-Students-Based-on-Study-Methods_ArpitChoudhary_66
Classify Students Based on Study Methods
First 5 rows:
visual_score	auditory_score	kinesthetic_score	learning_style
0	8.000301	1.389837	9.686887	visual
1	8.401052	7.294055	4.853655	visual
2	9.124874	3.975049	6.688173	auditory
3	5.724100	7.702631	7.535001	auditory
4	5.060739	4.711628	4.302653	kinesthetic

Missing values per column:
 visual_score         0
auditory_score       0
kinesthetic_score    0
learning_style       0
dtype: int64 

After dropna: 100 rows remain

No 'LearningStyle' column found → skipping classification

Cluster sizes:
 Cluster
1    41
0    31
2    28
Name: count, dtype: int64 
![download](https://github.com/user-attachments/assets/51ef181a-0e08-40fe-8ec8-3c618cafe709)
About the Project
This project is focused on analyzing and classifying students based on their preferred study methods. The goal is to understand how students learn best — whether they are Visual, Auditory, or Kinesthetic learners — using their responses from a questionnaire.

By using both classification and clustering algorithms, the project helps:

Predict a student's learning style based on scores

Group similar learners together using patterns in the data

This kind of analysis can be useful in educational planning, personalized teaching, and adaptive learning platforms.

🤖 Algorithm Used
🔹 Random Forest Classifier (Supervised Learning)
Purpose: To predict the student’s learning style (Visual, Auditory, Kinesthetic).

Why Used: It’s accurate, handles mixed types of data, and reduces overfitting using multiple decision trees.

Evaluation Metrics:

Accuracy: Overall correctness

Precision: How precise the model is when it says a student is a particular type

Recall: How many actual students of a type the model found

F1-Score: Balance between precision and recall

Confusion Matrix: To visualize correct vs. incorrect predictions

🔹 K-Means Clustering (Unsupervised Learning)
Purpose: To group students into clusters based on their study method scores, even without knowing their actual learning styles.

Why Used: It helps discover natural groupings and hidden patterns in the data.

Process:

Data was scaled using StandardScaler

Clustering was done with 3 clusters (based on 3 learning styles)

