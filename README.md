<div style="text-align: center; color: white; background-color: #559cff; font-weight: bold; padding: 20px" >
<p style="font-size: 30px">️💻 PROGRAMMING FOR DATA SCIENCE - FIT - HCMUS ️💻</p>
</div>

<div style="text-align: center; color: white; background-color: #FB8B24; font-weight: bold; padding: 20px" >
<p style="font-size: 25px">️🎶 Final Project - Analysis of Most Streamed Spotify Songs 2023 ️🎶</p>
</div>

### I. Group Information: 📝

- Class ID: 21KHDL1
- Group name: Double N

| ID       | Name              |
| -------- | ----------------- |
| 21127664 | Tran Dai Nien     |
| 21127657 | Nguyen Khanh Nhan |

### II. Project Information: 📝

#### **_01. Dataset:_** 📖

- **Link**: [Most Streamed Spotify Songs 2023](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023/code?datasetId=3668746&sortBy=voteCount)
- **Description**: This dataset contains a comprehensive list of the most famous songs of 2023 as listed on Spotify. The dataset offers a wealth of features beyond what is typically available in similar datasets. It provides insights into each song's attributes, popularity, and presence on various music platforms.
- **License**: The owner stated `"Other (specified in description)"` but did not mention it in the description section. However, this dataset is a `general public data set` on Kaggle, and below the description, the author expressed gratitude for support through upvotes. Therefore, this dataset is provided to the community for `research and learning purposes`, and within the scope of our course, we can use this dataset for our final project.

#### **_02. Project Structure:_** 📂

```
data
├── processed_spotify-2023.csv
└── spotify-2023.csv
img
└── owner_expressed.jpg
notebook
├── 01_Data_Collection.ipynb
├── 02_Data_Exploration_and_Preprocessing.ipynb
├── 03-Question_1.ipynb
├── 04-Question_2.ipynb
├── 05-Question_3.ipynb
└── 06-Question_4.ipynb
```

#### **_03. Data exploration and Preprocessing:_** 🕵️🔧

- Understand basic information about dataset
- Understand the meaning of each column
- Preprocessing data: handle missing values, outliers, incorrect values.
  - With missing values: we use `KNN Imputer` to fill missing values.
  - With outliers: we use `IQR` to detect and remove outliers if necessary.
  - For incorrect values: we will remove artist's name or track's name that contains special characters.
- We divide the dataset into 2 parts: `numerical data` and `categorical data`.
  - For `numerical` data: we will observe the distribution of each column and their descriptive statistics. Then we will check if there is any missing value in these columns.
  - For `categorical` data: we will also observe the distribution of values in these columns. We also check if there is any missing value in these columns.
- Finally, we will check the `correlation` between columns in the dataset to see if there is any relationship between them. We will use `heatmap` to visualize the correlation matrix. For more details, we also use `joint plot` and `scatter plot` to visualize the relationship between 2 most correlated columns.
- In this project, our group use many different kinds of chart for visualization to get insights about the dataset: `bar chart`, `histogram`, `KDE plot`, `box plot`, `scatter plot`, `joint plot`, `3D plot`, `pie chart`, `line chart`,...

#### **_04. Meaningful questions:_** ❓

❓ Question 1: What makes song popular? 📈 <br>
✅**ANSWER:** <br>

- 📑 After all the efforts to analyze dataset and make some valuable insights from it. we come to a conclusion:

  - 📌 The best value of each attributes of a best song that we have found:

  | Best factors       | Value |
  | ------------------ | ----- |
  | bpm                | 171   |
  | key                | C#    |
  | mode               | Major |
  | danceability\_%    | 50    |
  | valence\_%         | 38    |
  | energy\_%          | 80    |
  | acousticness\_%    | 0     |
  | intrumentalness\_% | 0     |
  | liveness\_%        | 9     |
  | speechiness\_%     | 4     |

- 📝 From many figures that we have analysed and comment, there are some noticeable notes:

          1. Some songs are the best songs of a year but the streams are not very high
          2. The average streams of a song is a measure for us to have a general insight in a dataset. For further investigate, we have to use different statistics to work with(Ex: median,...)
          3. Each platforms have different users with various taste of music. The best songs from a platform may or may not be the best one in another platform
          4. There are some phases that the streams increase significantly(the changing rate is very high)
          5. Some platforms have the users that are very high compare to the others(the number of songs included in a playlist are very remarkable)
          6. When we are trying to find the best value of a good song, we see that many best songs have quite similar music properties(key, bpm,...)

- 😊 With the best values that our team have found. We hope that this can help the composers/artists out there to be able to make their new songs become hits and top trending songs.

❓ Question 2: Which makes Taylor Swift's songs become well-known and attract billions of people around the world? ️🎤 <br>
✅**ANSWER:** <br>

    - 📝 After investigate by plotting and analyzing her songs, we come to the conclusion:

        1. Taylor Swift is **versatile artist**: perform several genres of music and perform them well.

        2. `Blank Space` is the most popular songs of her.

        3. The **average streams** of her songs is remarkable compare to other famous artists.

        4. The `released day`, `released month` are factor that we need to consider as many artists choosed this date to released his/her song (include Taylor).

        5. The way Taylor compose her songs is diverse, some songs are high in one properties but low other properties. However, that song still can reach us in some way.

        6. Her songs' rank are very high in multiple platform (Spotify, Apple, Deezer). Most of them are in top 10 and some of them are in Top 1.

        7. Average song of playlists of all of her songs are also very high (in Top 5 songs).

- 📌 Best factors that we can find from Taylor Swift's best songs:

| Best factors       | Value |
| ------------------ | ----- |
| bpm                | 96    |
| key                | D     |
| mode               | Major |
| danceability\_%    | 75    |
| valence\_%         | 40    |
| energy\_%          | 47    |
| acousticness\_%    | 71    |
| intrumentalness\_% | 0     |
| liveness\_%        | 13    |
| speechiness\_%     | 4     |

❓ Question 3: How has music evolved over the years? 📈 <br>
✅**ANSWER:** <br>

📌 Analyzing how the music evolved will help us understand the trend of music and the taste of listeners, based on this we can make songs that are more suitable for the listeners. After analyzing, we come up with some conclusions about the trend of music over the years:
- The average `BPM` of songs has fluctuated over the years. But in the last 10 years, it has generally remained stable at around `110-130`.
- `Danceability`, `valence` and `energy` have shown a upward trend over the years. This means that songs are becoming more and more `danceable`, `happy` and `energetic`.
- On the other hand, `acousticness`, `instrumentalness`, `liveness` and `speechiness` have shown a downward trend over the years or not changed much. This means that songs are becoming less and less `acoustic`, `instrumental`, `live` and `spoken`. <br>

❓ Question 4: In the top 5 artists with the highest number of streams on Spotify, what are the similarities and differences in the features of their songs?🔝 <br>

✅**ANSWER:** <br>

📌 After analyzing, we found the similarities and differences in the features of the songs of the top 5 artists with the highest number of streams on `Spotify`. Based on these similarities and differences, it will be very helpful when you want to create a song and want it to be the most popular possible, here are some guidelines you should follow to maximize your chances of success: 
- The `C#` key is the most popular and most successful one for listeners. But not all artists prefer to use this key in their songs. `The Weeknd` and `Bad Bunny` have the same high proportion of `C#` in their key songs. `Ed Sheeran` `Taylor Swift` and `Harry Styles` seem not to prefer `C#` in their key songs.
- Using the Major mode is preferable, as it is the most popular and most successful mode on Spotify. All 5 artists have a high proportion of `major` in their `mode` songs.
- `BPM` of all 5 artists' songs is around `120`. This is indicated that songs with `bpm` around `120` will be more popular.
- All the song of these 5 artists have a very high average `danceability` (more than `60%`). So your song needs to share a minimum of `danceability` to be among the most popular ones. A minimum of `60%` is recommended.
- Not like what we think `Positivity is the key, be positive in the song and it will have a higher chance of success`. `Valence` in these 5 artists' songs is not very high but their songs are still very popular. So `valence` is not a very important factor to make a song popular.
- The average `energy` of all 5 artists is around `60%`. So this means that songs with more `energy` will be more popular.
- The `speechiness` of all 5 artists' songs is very low (less than `10%`). It is indicated that nowadays people prefer songs with less `speechiness`, they prefer songs with more `rhythm` and `melody`.



### **III. Planning:\_** 📅

Our group will use `Trello` to manage the process of the project: `assign tasks`, `track progress` and `ensure that the project is completed on time`.

- Trello: https://trello.com/b/q4LXHImb/21khdlfinalprojectdoublen

### **IV. Detail Implementation\_** 👀

- Github: https://github.com/khanhnhan1512/Final-Project-DS-Programming/tree/main

### **V. Reflection:\_** 📝
❌ Difficulties:
- Nien:
  - Find hard to find the attributes that contribute to the most meaning for plotting the chart
  - The analysing process is not very detail enough, need to learn more
- Nhan:
  - Having difficulty coming up with interesting and meaningful questions to answer.
  - In terms of handling incorrect data, I have only been able to handle it in the simplest way, without finding a specific approach to thoroughly solve the problem. I haven't found a way to fix incorrect data instead of just deleting it. <br>

✅ What we have learned:
- Nien:
  - Learn how to use `KNN Imputer` to fill missing values.
  - Learn how to implement `exploration and preprocessing data` in a `data science project`.
- Nhan:
  - Learn many plotting techniques and how to use them to visualize data.
  - Learn how to use many important libraries for `data science` such as `numpy`, `pandas`, `matplotlib`, `seaborn`,...

⌛ What we will do in the future:
- Use more advanced techniques to handle incorrect data.
- Using machine learning algorithms to predict the popularity of a song based on its attributes.
- Make recommendations for artists to make their songs more popular.


### **VI. References:\_** 📚

- [Use `Spotify` to find missing keys](https://www.kaggle.com/code/dreygaen/investigating-the-most-popular-spotify-songs#%F0%9F%8F%86-What-Does-It-Take-To-Top-the-Spotify-Charts-?)
- [Refer to graph plotting and implementation ideas](https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023/code?datasetId=3668746&sortBy=voteCount&fbclid=IwAR0N7HijDpvV7bWlNifDgK5Rq6cO_idYx-puZl3xSm-OK11AVGoQNduESBM)
- [How to use Joint Plot](https://www.javatpoint.com/joint-plot-in-python)