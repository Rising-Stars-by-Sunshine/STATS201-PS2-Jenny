# Research Question Formulation

## 1.1 Objective

**Objective:** To investigate the correlation between public perception of climate change discussions on Twitter and the occurrences of extreme weather events and the release of environmental policy over time during the impactful year of 2022.

**Significance:** Understanding the intricate relationship between real-world events, environmental policies, and public discourse on social media is paramount. This research seeks to shed light on how external factors influence public perceptions of climate change, contributing valuable insights for policymakers, researchers, and the broader public.

## 1.2 Operational Measures

### 1.2.1 Variables

**Dependent Variable (Y):** Public perception of climate change discussions on Twitter (measured by tweet frequency).

**Independent Variables (X):**
- The occurrence of extreme weather events.
- Release of environmental policy.

### 1.2.2 Data Type

Time-series data was collected by filtering the top daily tweets based on the hashtag 'Climate Change'. The duration of the time-series analysis will be 6 months, in the first half of 2022. This approach ensures a focused examination of the immediate impact of the incident on public discourse.

## 1.3 Hypothesis Development

### 1.3.1 Prediction Hypothesis

The hypothesis asserts that, within the timeframe of 01/01/2022 to 19/07/2022, a positive correlation exists between the frequency of extreme weather events, significant environmental policy releases, and the public perception of climate change discussions on Twitter. Anticipated peaks in tweet frequency during significant events and policy releases signify heightened public engagement, aligning with the profound impact of climate change observed globally during this period.

### 1.3.2 Justification

Grounded in recent findings (Chen, Zou, and Zhao 2019), this hypothesis posits that external events, particularly extreme weather incidents, stimulate increased discussions about climate change on social media. Furthermore, the release of environmental policies is expected to act as a catalyst, fostering elevated public awareness and discourse around climate-related issues (Hamed et al. 2015). This aligns with the established notion that significant real-world events and policy actions play a pivotal role in shaping public engagement with climate change discussions on Twitter, especially in the context of the impactful year 2022.

## 1.4 Machine Learning Algorithm Selection

### 1.4.1 Sentiment Analysis

**Algorithm:** OpenAI's GPT-3.5 model

**Justification:** GPT-3.5 is employed for sentiment analysis due to its advanced natural language processing capabilities, allowing for nuanced classification of sentiments expressed in tweets.

### 1.4.2 Topic Modeling

**Algorithm:** BERTopic

**Justification:** BERTopic is chosen for its efficacy in uncovering thematic clusters within text data. Its application to stance-specific datasets enables a detailed exploration of prevalent themes within each stance, contributing to a comprehensive overview of shifts in climate change discussions.

### 1.4.3 Linear Regression Analysis

**Algorithm:** Linear Regression

**Justification:** Linear regression analysis is selected for investigating the correlation between sentiments towards economic and environmental policies and public perceptions of climate change. It is a suitable statistical method for exploring relationships between variables, providing valuable insights into the correlation between sentiments related to policies and public perceptions of climate change.

# 2. The Machine Learning Workflow

## 2.1 Model Development

### 2.1.1 Data Processing

**Dataset Collection:** Gather a comprehensive dataset from Twitter, encompassing over a million tweets from January to July 2022.

**Tweet Classification:** Employ OpenAI's GPT-3.5 model for tweet classification based on stances (believers, neutrals, deniers) and sentiments (positive, negative). Classify tweets receiving the top 1000 likes to ensure relevance and significance.

**Topic Modeling:** Apply the BERTopic technique to identify thematic clusters within the entire dataset and stance-specific sub-datasets. This method allows for the extraction of prevalent topics within the broader conversation about climate change.

**Sentiment Analysis:** Utilize sentiment analysis methods to discern emotional inclinations and attitudes expressed within tweets discussing economic and environmental policies in the context of climate change.

**Linear Regression Analysis:** Employ linear regression analysis to investigate the correlation between sentiments towards economic and environmental policies and public perceptions of climate change.

## 2.2 Results Presentation

### 2.2.1 Training and Testing

**Cross-Validation:** Apply cross-validation techniques, such as k-fold cross-validation, to enhance the robustness of the model evaluation process. This approach involves partitioning the dataset into multiple folds, training the model on different subsets, and assessing performance across various configurations.

**Model Evaluation Metrics:** Utilize accuracy, precision, recall, F1 score, and confusion matrix as evaluation metrics, specifically tailored to the sentiment analysis model (OpenAI's GPT-3.5) to ensure a comprehensive assessment of its performance in stance classification.

### 2.2.2 Data Visualization

**Thematic Clusters:** Visualize thematic clusters derived from BERTopic analysis using interactive visualizations, such as cluster heatmaps or dendrograms. This provides a clear representation of prevalent topics within the climate change discourse.

**Sentiment Trends:** Create line charts or time series plots to illustrate sentiment trends over the specified temporal domain. Highlight key points, such as extreme weather events and policy releases, to showcase their impact on sentiment.

**Linear Regression Results:** Present linear regression results through scatter plots, regression lines, or residual plots, demonstrating the correlation between sentiments towards economic and environmental policies and public perceptions of climate change.

**Comparative Analysis:** Visualize the results of stance classification by comparing the model's predictions with tweets from representative accounts embodying each stance (believers, neutrals, deniers). This can be presented through stacked bar charts or confusion matrices.

## 2.3 Model Evaluation

### 2.3.1 Evaluation Criteria

**Evaluation Criteria (OpenAI's GPT-3.5 for sentiment analysis):**

- **Precision:** Evaluate the precision of stance classification, examining the proportion of accurately identified believers, neutrals, and deniers among all predicted instances.

**Comparison with Representative Accounts:**

- Validate the model's stance classification by comparing its results with tweets from representative accounts known to embody each stance—believers, neutrals, and deniers. This comparative analysis ensures the model's outputs align with human-defined stances and diverse perspectives.

- **F1 Score:** Utilize the F1 score to balance precision and recall, providing a comprehensive measure of the model's performance in stance classification.

## 2.4 Iterative Improvement

**For OpenAI's GPT-3.5 for sentiment analysis:**

- **Feedback Mechanism:** Establish a user feedback mechanism to gather input on model predictions, especially in cases involving nuanced expressions and multi-sentence contexts related to climate change discussions.

- **Bias Mitigation:** Implement strategies to mitigate biases in the model, focusing on the specific context of climate change discussions. Regularly assess and adjust the model to minimize biases and ensure fair representation across different perspectives.

**For BERTopic:**

- **Cross-Validation with Diverse Data:** Enhance cross-validation techniques by ensuring diversity in the dataset, encompassing a wide range of expressions and perspectives specific to climate change discourse. This approach improves the model's ability to generalize across varied user behaviors in this domain.

# Mindmap created by Whimscal
<img width="606" alt="image" src="https://github.com/Rising-Stars-by-Sunshine/STATS201-PS2-Jenny/assets/125801773/be7851f2-763b-4170-b296-852967e5cd8c">

# References
Chen, Xingyu, Lei Zou, and Bo Zhao. 2019. “Detecting Climate Change Deniers on Twitter Using a Deep Neural Network.” Proceedings of the 2019 11th International Conference on Machine Learning and Computing - ICMLC ’19. https://doi.org/10.1145/3318299.3318382.

Mildenberger, Matto, and Anthony Leiserowitz. 2017. “Public Opinion on Climate Change: Is There an Economy–Environment Tradeoff?” Environmental Politics 26 (5): 801–24. https://doi.org/10.1080/09644016.2017.1322275.

‌Hamed, Ahmed Abdeen, Alexa A. Ayer, Eric M. Clark, Erin A. Irons, Grant T. Taylor, and Asim Zia. 2015. “Measuring Climate Change on Twitter Using Google’s Algorithm: Perception and Events.” International Journal of Web Information Systems 11 (4): 527–44. https://doi.org/10.1108/ijwis-08-2015-0025.
