# Machine Learning - Compulsory Task

## 1. Input and Output Descriptions

|      | Input(s)                                                    | Output                                                      |
| ---- | ----------------------------------------------------------- | ------------------------------------------------------------ |
| 1.1  | Sensor data from cameras, Lidar, radar, and GPS               | Control commands for the car (e.g., steering angle, acceleration, braking) |
| 1.2  | User viewing history, ratings, genre preferences, watch time, and browsing behavior | Recommended movies or TV shows ranked by predicted user preference |
| 1.3  | Images of signatures captured through a scanner or camera    | Binary result indicating whether the signature is authentic or not |
| 1.4  | Patient's medical history, symptoms, diagnostic test results | Diagnosis or likelihood of having a particular disease       |

## 2. Regression or Classification

* **2.1 Classifying emails as promotion or social based on their content and metadata.**
  - Appropriate Algorithm: Classification
  - Justification: Categorizing emails into distinct classes (promotion or social) aligns with the use of classification algorithms designed for discrete outcomes.

* **2.2 Forecasting the stock price of a company based on historical data and market trends.**
  - Appropriate Algorithm: Regression
  - Justification: The task involves predicting a continuous variable (stock price), making regression models suitable for numeric value prediction.

* **2.3 Sorting images of animals into different species based on their visual features.**
  - Appropriate Algorithm: Classification
  - Justification: Assigning images to specific classes (animal species) fits the use of classification algorithms designed for categorizing data.

* **2.4 Predicting the likelihood of a patient having a particular disease based on medical history and diagnostic test results.**
  - Appropriate Algorithm: Classification
  - Justification: The binary outcome (having the disease or not) aligns with classification models designed for discrete class prediction, fitting medical diagnosis tasks.

## 3. Supervised or Unsupervised Learning

* **3.1 Detecting anomalies in a manufacturing process using sensor data without prior knowledge of specific anomaly patterns.**
  - Appropriate Algorithm: Unsupervised
  - Justification: Unsupervised learning is suitable for anomaly detection when there is no prior knowledge of specific anomaly patterns.

* **3.2 Predicting customer lifetime value based on historical transaction data and customer demographics.**
  - Appropriate Algorithm: Supervised
  - Justification: Predicting customer lifetime value involves learning from historical data with known outcomes.

* **3.3 Segmenting customer demographics based on their purchase history, browsing behaviour, and preferences.**
  - Appropriate Algorithm: Unsupervised
  - Justification: Unsupervised learning is suitable for segmenting customers when the goal is to discover patterns and group similar individuals without predefined labels.

* **3.4 Analysing social media posts to categorise them into different themes.**
  - Appropriate Algorithm: Unsupervised (or possibly semi-supervised)
  - Justification: Unsupervised learning can be used for theme categorization when there is no labeled data. A semi-supervised approach may enhance accuracy if some labeled examples are available.

## 4. Semi-Supervised Learning

* **4.1 Predicting fraudulent financial transactions using a dataset where most transactions are labelled as fraudulent or legitimate.**
  - Appropriate: Not Appropriate for Semi-Supervised Learning
  - Justification: Predicting fraudulent financial transactions using a dataset where most transactions are already labeled as fraudulent or legitimate doesn't necessitate the use of semi-supervised learning. A supervised approach would be more appropriate, focusing on the available labeled data for training.

* **4.2 Analysing customer satisfaction surveys where only a small portion of the data is labelled with satisfaction ratings.**
  - Appropriate: Appropriate for Semi-Supervised Learning
  - Justification: Analyzing customer satisfaction surveys with only a small portion of labeled data is suitable for semi-supervised learning. This approach can effectively utilize both labeled (satisfaction ratings) and unlabeled data to improve model performance.

* **4.3 Identifying spam emails in a dataset where the majority of emails are labelled.**
  - Appropriate: Not Appropriate for Semi-Supervised Learning
  - Justification: Identifying spam emails in a dataset where the majority of emails are already labeled doesn't require semi-supervised learning. A supervised approach is more suitable, leveraging the abundance of labeled data for training.

* **4.4 Predicting the probability of default for credit card applicants based on their complete financial and credit-related information.**
  - Appropriate: Not Appropriate for Semi-Supervised Learning
  - Justification: Predicting the probability of default for credit card applicants based on their complete financial and credit-related information can be effectively addressed with supervised learning. The availability of labeled data supports the use of a traditional supervised approach without the need for semi-supervised techniques.