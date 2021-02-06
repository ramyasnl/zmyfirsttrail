  # **Overview of Project**  
  We are going to analyze the data to help Louise understand and uncover hidden trends to make her crowed funding project a success.  
  ##**Purpose of the Project** 
  Louise’s play Fever came close to its fundraising goal in a short duration of time. We want to analyze and visualize  how different campaigns fared in relation to,<br/>
    1.The launch dates and outcome of the play,<br/>
    2.The funding goals and percentage of outcome<br/>
    ## **Challenges and Analysis**<br/>
    1.The launch dates and outcome of the play<br/>
     For this analysis the data we need 	are outcomes of the sub category “plays”and the “launch dates”,
     Both the data we need are in the “kickstarter_challenge” but in a different form ,<br/>
     **Step1:**  To separate the Parent category and sub category,
                 Which is done by separating the column" Category and Sub category”, since we are interested only in the data of “ plays”.<br/>
     **Step2:**  Converting the launch date in Unix time stamps to readable format by using the formula ,
                 (((J2/60)/60)/24)+DATE(1970,1,1) where J2 is the column of Launch Date unix time stamps in the “kickstarter_challenge”.
         

