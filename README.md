# Kickstarter-Analysis

**Overview of Project**

In this project we reviewed an excel document that contained the names of different campaigns related to performing arts such as tv, film, and theater and more. With this data we are to demonstrate the ability to use excel formulas and formatting. We were asked to analyze the data and make conclusions based on the different parameters requestested. The excel tools in focus are pivot tables creation, basic functions implementation, data visualization, and cell formatting.

**Purpose**

The purpose of this analysis is to compare different campaigns based on their launch dates and funding goals. The first part of the challenge asked to determine how many were successful, how many failed, and how many were canceled. With the help of visualizations using excel we can determine the outcomes of all the campaigns. The next part of the challenge, we were asked to create a summary table specifically for the subcategory "plays" in which we would need to use a nested "countifs" function to determine the number of successful, failed, and canceled campaigns. With this information we then determined the percentage for each based on the total number of projects. Lastly, we would then graph the results to aid our audience understand and easily digestible the results given.

**Analysis and Challenges**

In the first part of the challenge we are asked to extract the date from the date the campaign was created. This was initially a little confusing to me because the way that the task described the campaign's "launch date" was as "created date". It took me some time to realize that they are the same. It was extra challenging because the launch at and due date columns in the data set were formatted in unix timestamp. This was something I have not seen before. With the help of a few Google searches I was able to make the connection and was able to format the unix timestamps to the standard date format of "mm/dd/yy". The next functions to extract the year only and the feature to split a column in two, are tools I have used in my day to day job before, so this was not a great challenge to me. Creating the graphs was also very straightforward, this was particularly easy to me although I found it challenging because I did this project on a Mac computer when I am used to working on a Microsoft computer. For the last part of the challenge in which we had to create the summary table for the "plays" category, I did have to do some research on how to properly use the "countifs" function but overall it was not very difficult. Here are the three websites that helped me which find the solution to my challenges:

How to convert unix timestamp to standard date format: https://exceljet.net/formula/convert-unix-time-stamp-to-excel-date

How to use the "countifs" function in excel: https://exceljet.net/excel-functions/excel-countifs-function

How to count cells between two values: https://www.extendoffice.com/documents/excel/2412-excel-count-cells-between-two-values.html

**Analysis of Outcomes Based on Launch Date**

With the help of pivot tables I was able to filter the date by month of the year classifying it in successful, failed, and canceled categories. This data was only for the theater parent category as requested in the challenge. After graphing the data we can determine that the theater category had more overall successful campaigns than failed and canceled ones. We can see the blue line, "successful", has a higher count month over month. Most campaigns are successful when they are launched in the month of may, this is indicated by the spike in the blue line in the month of May with a total of about 111 successful campaigns. The orange line shows the campaigns that failed, we can see that is a very steady line. The lowest number of failed campaigns was 31 in the month of November and the highest number in the month of may with 52. The gray line shows us the campaigns that had to be canceled. This was also a very steady line but in the lower numbers with October having the least canceled campaigns with a total of 0, and January being the highest with a total of 7. Even though May had the highest number of failed campaigns it had a very low number of cancellations and is most likely to have the most number of campaigns for any month in the year.

**Analysis of Outcomes Based on Goals**

With the table I created using the "countifs" functions I was able to determine the number of successful, failed, and canceled projects and also classifying them by the dollar goal amount. By calculating the total number of projects, and cultivating the percentage for each outcome I was able to create a chart that easily visualized the results. First looking at the blue line, the percentage of success, we can initially see it start declining as the goal amount increases but then we see a spike between the 30k to 45k, between 45k and 49k there is a drop and then a sudden spike again above the 50k mark. When we look at the orange line, the percentage of failed, we can see an interesting pattern; the lines are inversely proportional to each other. The lines mirror each other but in the opposite directions. This could have been influenced by the fact that there are no can led campaigns, but the data does not explain what could have caused this. But we can determine which ranges have a better chance of success and which ranges have a more likely chance of failure.

**Challenges and Difficulties Encountered**

The challenge I faced was converting the unix timestamp to standard date format. This was not a known format for me and I did not know how to convert them initially. But doing a little bit of research helps tremendously. As stated before I use Excel on a daily basis at my current job so some of the tasks were straight forward for me. The only difficult part was that I am using a Mac computer for this assignment and and at work I use a Microsoft, and some of the tools and features in excel may look different but overall have the same functionality.

**Results**

What are two conclusions you can draw about the Outcomes based on Launch Date? 
- Conclusion #1 : The number of successful campaigns are greater in every month except December where it matches the number of failed.
- Conclusion # 2: The highest number of successful campaigns are the ones launched in the month May but also have the highest number of failed ones.

What can you conclude about the Outcomes based on Goals? 
- Campaigns are successful if their goal range is less than 1000 to 14999, between 35000 and 44999, and greater than 50000.

What are some limitations of this dataset? 
- We compared the goal amounts of all the campaigns but many were from different countries and with different currencies. I believe that if we convert the currency to a single currency type the funding goal amounts would have been different.

What are some other possible tables and/or graphs that we could create? 
- Other ideas for analyzing this data would be comparing the campaign outcomes by the countries. We could also create a table that converts the currencies to a single currency to determine which campaign had the most funding.


![image](https://user-images.githubusercontent.com/95899763/181157178-3d7db1a3-420c-4a55-abb5-cf9240672a3b.png)

![image](https://user-images.githubusercontent.com/95899763/181157268-efa31ace-b1db-4f82-bdfa-1269d8101b9b.png)

