# Task4_Level2_Restaurant_Chains_Analysis

<html>
  <body>

<h2>🔹Project Overview:</h2>

In this project, I analyzed a given restaurant dataset to explore insights on:
1. Identify if there are any restaurant chains present in the dataset.
2. Analyze the ratings and popularity of different restaurant chains.

<h2>🔹 Key Insights: </h2>
After performing a thorough analysis, here are the findings:<br>
1. Restaurant chains are identified:
['Cafe Coffee Day', 'Domino's Pizza', 'Subway', 'Green Chick Chop',
       'McDonald's', 'Keventers', 'Pizza Hut', 'Giani', 'Baskin Robbins',
       'Barbeque Nation',
       ...
       'Nazeer Delicacies', 'Embassy', 'Delhi Biryani Hut',
       'Qureshi Kabab Corner', 'KC Bakers', 'Zaika Kathi Rolls',
       'The Night Owl', 'The Cheesecake Factory', 'New Kadimi',
       'Ceviche Tapas Bar & Restaurant'],
      dtype='object', length=734)
    <br>
    by applying the code:<br> <em>chain_counts = df['Restaurant Name'].value_counts()<br>
rest_chains = chain_counts[chain_counts > 1].index<br>
rest_chains</em><br><br>
<br> After finding the  average rating and total votes by using the code <br>
<em>analysis_of_chain = df_chains.groupby('Restaurant Name').agg({<br>
    'Aggregate rating': 'mean',<br>
    'Votes': 'sum',<br>
    'Restaurant ID': 'count'<br>
}).rename(columns={'Restaurant ID': 'Branch Count'}).sort_values(by='Votes', ascending=False)</em><br> <br>
  2. The ratings and popularity of different top 10 restaurant chains are given below:<br>
  <table>
    <thead>
      <tr>
        <th>Restaurant Name</th>
        <th>Aggregate Rating</th>
        <th>Votes</th>
        <th>Branch Count</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>Barbeque Nation</td><td>4.353846</td><td>28142</td><td>26</td></tr>
      <tr><td>AB's - Absolute Barbecues</td><td>4.825000</td><td>13400</td><td>4</td></tr>
      <tr><td>Big Chill</td><td>4.475000</td><td>10853</td><td>4</td></tr>
      <tr><td>Farzi Cafe</td><td>4.366667</td><td>10098</td><td>6</td></tr>
      <tr><td>Truffles</td><td>3.950000</td><td>9682</td><td>2</td></tr>
      <tr><td>Chili's</td><td>4.580000</td><td>8156</td><td>5</td></tr>
      <tr><td>Joey's Pizza</td><td>4.250000</td><td>7807</td><td>2</td></tr>
      <tr><td>Big Yellow Door</td><td>4.266667</td><td>7511</td><td>3</td></tr>
      <tr><td>Saravana Bhavan</td><td>4.133333</td><td>7238</td><td>3</td></tr>
      <tr><td>Starbucks</td><td>3.805556</td><td>7139</td><td>18</td></tr>
    </tbody>
  </table>
  <p> For More Understanding I plot a bar plot</p>
  <p align="left">
  <img src="download.png" alt="bar plot" width="600"><br>
  

<h2>🛠️Tools & Technologies Used:</h2><br>

To achieve this Task4 of level 2, I used the following tools and technologies:<br>

1. Python – used as a programming language for data analysis
2. NumPy – used for efficient numerical computations
3. Pandas – used for data cleaning, manipulation, and analysis
4. Matplotlib – used for creating visualizations like charts and plots
5. Seaborn – used for advanced statistical data visualization
6.  Jupyter Notebook (Primary IDE) - used for writing and executing code.

These tools enabled me to effectively extract insights and meaning from the data.<br><br>
🎉 I'm grateful for the opportunity to work on this project and sharpen my data analysis skills. <br>Thank you to Cognifyz Technologies for this amazing learning experience! I'm excited to continue growing and taking on new challenges.<br><br>
Explore the full project on LinkedIn and GitHub:<br>
▶️ [(https://www.linkedin.com/feed/update/urn:li:activity:7316539760322191360/)<br>](https://www.linkedin.com/feed/update/urn:li:activity:7317217856398446592/)<br>

<p>I hope this will be very helpful to new learners and students. <br>
And I'd love to hear your thoughts and feedback! <br>
Let's connect and explore more data-driven insights together. <br><br>
Thank you all!

  <b>(YUMNAM PREMKUMAR SINGH)</b>
</p>
</body>
</html>
