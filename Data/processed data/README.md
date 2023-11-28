*Here is a general guide to help you understand how I clean the data:*

**Data Cleaning and Processing Guide:**

**1. Duplicate Removal:**
   - **Objective:** Ensure each tweet is unique.
   - **Step:** Identify and remove duplicate tweets based on their unique 'Tweet URL.'

**2. Tweet Text Cleaning:**
   - **Objective:** Enhance text quality and readability.
   - **Steps:**
      - **Full Cleaning:**
         - Remove unnecessary elements like URLs, emojis, mentions, smileys, and numbers from the entire tweet.
         - Create a new column 'cleaned_text' containing fully cleaned tweets.
      - **Partial Cleaning:**
         - Remove URLs and mentions, creating a 'partial_clean' column.

**3. Additional Cleaning:**
   - **Objective:** Standardize and improve text consistency.
   - **Steps:**
      - Remove '#' symbols from the 'cleaned_text' column.
      - Convert all text to lowercase.
      - Remove non-alphanumeric characters and extra whitespaces.


 
<img width="377" alt="image" src="https://github.com/Rising-Stars-by-Sunshine/STATS201-PS2-Jenny/assets/125801773/2f8c5961-35d0-4cbb-a0ea-d5f9e77fb31c">

