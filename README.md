<div style="text-align: center; color: white; background-color: #559cff; font-weight: bold; padding: 20px" >
<p style="font-size: 30px">️💻 PROGRAMMING FOR DATA SCIENCE - FIT - HCMUS ️💻</p>
</div>

<div style="text-align: center; color: white; background-color: #FB8B24; font-weight: bold; padding: 20px" >
<p style="font-size: 25px">️🎶 Final Project - Analysis of Most Streamed Spotify Songs 2023 ️🎶</p>
</div>



### I. Group Information: 📝

- Class ID: 21KHDL1
- Group name: Double N

| ID        | Name            |
| -------- | ----------------- |
| 21127664 | Tran Dai Nien     |
| 21127657     | Nguyen Khanh Nhan |

### II. Project Information: 📝

#### **_01. Dataset:_** 📖

- **Link**: [Most Streamed Spotify Songs 2023](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023/code?datasetId=3668746&sortBy=voteCount)
- **Description**: This dataset contains a comprehensive list of the most famous songs of 2023 as listed on Spotify. The dataset offers a wealth of features beyond what is typically available in similar datasets. It provides insights into each song's attributes, popularity, and presence on various music platforms.
- **License**: The owner stated `"Other (specified in description)"` but did not mention it in the description section. However, this dataset is a `general public data set` on Kaggle, and below the description, the author expressed gratitude for support through upvotes. Therefore, this dataset is provided to the community for `research and learning purposes`, and within the scope of our course, we can use this dataset for our final project.

#### **_02. Project Structure:_** 📂

#### **_03. Data exploration and Preprocessing:_** 🕵️🔧

- Understand basic information about dataset
- Understand the meaning of each column
- Preprocessing data: handle missing values, outliers, incorrect values.
    - With missing values: we use `KNN Imputer` to fill missing values.
    - With outliers: we use `IQR` to detect and remove outliers if necessary.
    - For incorrect values: we will remove artist's name or track's name that contains special characters.
- We divide the dataset into 2 parts: `numerical data` and `categorical data`.
    - For `numerical` data: we will observe the distribution of each column and their descriptive statistics. We also check if there is any missing value in these columns.
    - For `categorical` data: we will also observe the distribution of values in these columns. We also check if there is any missing value in these columns.
- Finally, we will check the `correlation` between columns in the dataset to see if there is any relationship between them. We will use `heatmap` to visualize the correlation matrix. For more details, we also use `joint plot` and `scatter plot` to visualize the relationship between 2 most correlated columns.
- In this project, our group use many different kinds of chart for visualization to get insights about the dataset: `bar chart`, `histogram`, `KDE plot`, `box plot`, `scatter plot`, `joint plot`, `3D plot`, `pie chart`, `line chart`,...

#### **_04. Meaningful questions:_** ❓

❓ Question 1: What makes song popular? 📈 <br>
✅**ANSWER:** <br>
❓ Question 2: Which makes Taylor Swift's songs become well-known and attract billions of people around the world? ️🎤 <br>
✅**ANSWER:** <br>
❓ Question 3: How has music evolved over the years? 📈 <br>
✅**ANSWER:** <br>
❓ Question 4:In the top 5 artists with the highest number of streams on Spotify, what are the similarities and differences in the features of their songs?🔝 <br>
✅**ANSWER:** <br>
### **III. Planning:_** 📅
Our group will use `Trello` to manage the process of the project: `assign tasks`, `track progress` and `ensure that the project is completed on time`.
- Trello: https://trello.com/b/q4LXHImb/21khdlfinalprojectdoublen

### **IV. Detail Implementation_** 👀

- Github: https://github.com/khanhnhan1512/Final-Project-DS-Programming/tree/main

### **V. Reflection:_** 📝

### **VI. References:_** 📚
- [Use `Spotify` to find missing keys](https://www.kaggle.com/code/dreygaen/investigating-the-most-popular-spotify-songs#%F0%9F%8F%86-What-Does-It-Take-To-Top-the-Spotify-Charts-?)
