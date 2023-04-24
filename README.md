
# Finding The Golden Age of Video Games Using SQL

<img src="https://cdn-icons-png.flaticon.com/512/4021/4021738.png" alt="" style="width: 25%; margin: 0 auto; height: auto; display: block;" />

## Introduction

The video game industry is a rapidly growing industry that has seen significant success over the years. The industry has evolved from simple, pixelated games to complex, high-definition games that are immersive and engaging. According to  Mordor Intelligence, the global gaming industry is expected to be worth more than $300 billion by 2027. 
<br>
The success of the industry can be attributed to several factors, including the rise of mobile gaming, the growth of esports, and the increasing popularity of streaming platforms like Twitch and YouTube Gaming. In addition, the COVID-19 pandemic has led to a surge in demand for gaming as people spend more time at home.  

Although the video game industry has achieved remarkable success, there is a debate about whether the present time is considered the 'golden age' of video games, or if that period has already passed.

The goal of this project is to explore the evolution of video games and their quality over time to determine when the video game industry was at its peak. 

## The Data

The [dataset](https://www.kaggle.com/datasets/holmjason2/videogamedata?resource=download) was downloaded from kaggle and contains over 13,000 games ranging from 1977 to the middle of 2020. The data contains 2 tables listed below.
    
<h3 id="game_sales"><code>game_sales</code></h3>
<table>
<thead>
<tr>
<th style="text-align:left;">column</th>
<th>type</th>
<th>meaning</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;"><code>Name</code></td>
<td>varchar</td>
<td>Name of the video game</td>
</tr>
<tr>
<td style="text-align:left;"><code>Platform</code></td>
<td>varchar</td>
<td>Gaming platform</td>
</tr>
<tr>
<td style="text-align:left;"><code>Publisher</code></td>
<td>varchar</td>
<td>Game publisher</td>
</tr>
<tr>
<td style="text-align:left;"><code>Developer</code></td>
<td>varchar</td>
<td>Game developer</td>
</tr>
<tr>
<td style="text-align:left;"><code>Games_Sold</code></td>
<td>float</td>
<td>Number of copies sold (millions)</td>
</tr>
<tr>
<td style="text-align:left;"><code>Year</code></td>
<td>int</td>
<td>Release year</td>
</tr>
</tbody>
</table>
<h3 id="reviews"><code>reviews</code></h3>
<table>
<thead>
<tr>
<th style="text-align:left;">column</th>
<th>type</th>
<th>meaning</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;"><code>Name</code></td>
<td>varchar</td>
<td>Name of the video game</td>
</tr>
<tr>
<td style="text-align:left;"><code>Critic_Score</code></td>
<td>float</td>
<td>Critic score according to Metacritic</td>
</tr>
  
## Approach
I will look to answer this question by comparing game sales to both critic and user reviews to determine which years had the highest quality video games, and explore whether the overall quality of video games has improved as the gaming market has grown.
<tr>
<td style="text-align:left;"><code>User_Score</code></td>
<td>float</td>
<td>User score according to Metacritic</td>
</tr>
</tbody>
</table>
