# Text-and-Geospatial-visualization
Report of Project 2 Data Visualization<br>
The second course project for Data Visualization consists of Text and Geospatial visualization of 
data collected from political blog “Wikinews” for a time span of 2006-2015. 
The data “Wikinews” consisted of words for four different categories that 
are : person, location, organization and miscellaneous. 
Each category contained information relative to the topic such as person contained 
names example: barack obama, eduardo campos, luiz inacio di silva etc and so on.
The project is divided into two distinct categories:<br>
1. Time Series Visualization of top 50 words occurring the most frequently over time.<br>
2. Relationship between words or input terms.<br>

Time Series Visualization exploring frequency of top 50 popular words over time is shown below:<br>
<img width="1262" alt="screen shot 2016-11-11 at 8 09 51 am" src="https://cloud.githubusercontent.com/assets/20443585/20222386/baa8f9d6-a7fa-11e6-9b12-0ceb2a29e286.png">

The data was used in this visualization is called “Wikinews.tsv”. The preprocessing of the data required the count of the words occurring at a particular time. That data processing is done dynamically in javascript.<br>
The Box A in the figure below is the Wordle visualization of the top 50 words occurring for that particular time that can be selected from a dropdown in our application:<br>
<img width="648" alt="screen shot 2016-11-11 at 10 40 20 am" src="https://cloud.githubusercontent.com/assets/20443585/20222537/4909c818-a7fb-11e6-8fcf-0fd165152a6b.png">
<br>
A click on the word displayed in the wordle displays the time series in the graph between the x and the y-axis as labelled in the figure below as Box B.<br>
<img width="823" alt="screen shot 2016-11-11 at 8 35 14 am" src="https://cloud.githubusercontent.com/assets/20443585/20222564/6b1e9ff0-a7fb-11e6-9ab9-d06472cc3769.png">
Interesting finds from the Dataset:  
A click on the year 2008 reveals that barack obama was a popular term as barack obama won the election for presidency on Nov 4, 2008.<br>
<img width="1259" alt="screen shot 2016-11-11 at 8 51 56 am" src="https://cloud.githubusercontent.com/assets/20443585/20222613/9ba32240-a7fb-11e6-8914-8769f86e0f1e.png">
A click on the year 2012 reveals that olympics was a popular term as the summer olympics was held in the year 2012.
<br>
<img width="1259" alt="screen shot 2016-11-11 at 8 50 49 am" src="https://cloud.githubusercontent.com/assets/20443585/20222709/fc9ffb54-a7fb-11e6-82e7-945a0db35aca.png">
The second part is the visualization of the relationship between the various terms in the provided dataset.<br>
The preprocessing of the relationship dataset was done as follows:<br>
Each line was taken as a row with multiple possible relationships hence, there could be multiple permutations of the words in the same rows. Each row in the dataset contains 6 categories with a null “source” category hence each category was combined using a “|” and then split into individual words with the “|” itself.<br> 
A snippet of the first row of the dataset is given below:<br>
<img width="846" alt="screen shot 2016-11-11 at 9 08 12 am" src="https://cloud.githubusercontent.com/assets/20443585/20222760/2a6d8cea-a7fc-11e6-89c6-8a24349b12bf.png">
