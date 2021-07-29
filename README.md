  # **Overview of Project**  
  We are going to analyze the data to help Louise understand and uncover hidden trends to make her crowed funding project a success.<br/>  
  ##**Purpose of the Project** <br/>
  Louise’s play Fever came close to its fundraising goal in a short duration of time. We want to analyze and visualize  how different campaigns fared in relation to,<br/>
    1.The launch dates and outcome of the play,<br/>
    2.The funding goals and percentage of outcome<br/>
    ## **Challenges and Analysis** <br/>
        ## 1.The launch dates and outcome of the play ##<br/>
                For this analysis the data we need 	are outcomes of the sub category “plays”and the “launch dates”,
         Both the data we need are in the “kickstarter_challenge” but in a different form ,<br/>
     **Step1:**  To separate the Parent category and sub category,
                 Which is done by separating the column" Category and Sub category”, since we are interested only in the data of “ plays”.<br/>                 
                 ![](https://github.com/ramyasnl/Kickstarter_Challenge/blob/main/subcatseparation.png) <br/>                 
     **Step2:**  Converting the launch date in Unix time stamps to readable format by using the formula ,
                 (((J2/60)/60)/24)+DATE(1970,1,1) where J2 is the column of Launch Date unix time stamps in the “kickstarter_challenge”.<br/>
          
   **ANALYSIS**<br/>
   **Step1:** Create a Pivot table  “Theater Outcomes vs Launch date” taking Outcomes in y axis and Date Created Conversion in x axis using 
               “parent category”and  “years” as Filter and “count of outcomes”in values,In the filter we select only “successful”,”Failure”,”Cancelled”
                And in the “parent category” we select only the “Theater” since we need that particular data.<br/>
    **Step2:** Visualizing the data . Done by  pivot table analysis line chart.<br/>
     ![](https://github.com/ramyasnl/Kickstarter_Challenge/blob/main/D1months%20vs%20theateroutcomes.png)<br/>
     **RESULTS**<br/>
     1.The month that launched the most successful Kickstarter campaigns was May . However, January, February , March 
      all had roughly the same number of failed campaigns launched.<br/>               
     2.The funding goals and percentage of outcome.<br/>
      For the ease of analyzing the data we are classifying the Goal  in to ranges mapping it to the outcomes which can give a clear picture to visualize.<br/>
     **Step1:** <br/>
      We need to use countifs() to classify the outcomes according to the range of goal amount ,<br/>
     **Step2:** <br/>
     Framing the function to each and every cell for the selected range for the corresponding outcome. 
     And calculating the percentage of outcomes <br/>
     **ANALYSIS** <br/>
     We did the analysis by doing a line chart with Goal range on X axis and Outcomes on Y axis .<br/>     
     Which gives us percentage of success is inversely proportional  to the goal range and percentage of failure is directly proportional to the goal range .<br/>
     **RESULT**<br/>
From this analysis we visualize that when the Goal range is minimum the percentage of success is more.
And when the Goal range is maximumum the percentage of success is low.<br/>
## Goal range Vs Percentage of Success.
 ![](https://github.com/ramyasnl/Kickstarter_Challenge/blob/main/Outcomes_vs_GoalD2.png)<br/>
