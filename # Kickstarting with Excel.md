# Kickstarting with Excel

## Overview of Project
### Purpose
	
	The purpose of this analysis was to sort through several kickstarted campaigns across various categories to uncover hidden trends in our data. Towards the end, our client requested that we discover common trends with data related to kickstarted campaigns that involved theater.
	
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
	In this analysis we wanted to look at particular campaign outcomes based on a given date. To do this we needed to convert our raw data date that was in the epoch format, to a more readable format, to do this we used the formula =((("cell number"/60)/60)/24)+DATE(1970,1,1). With that we extracted the year and created a pivot table in order to organize multiple columns of data into 1 centralized location. With our pivot table we were able to filter by year, and month for successful, canceled and failed campaigns.


### Analysis of Outcomes Based on Goals
	In this analysis we looked at the specific goals that each play expected to hit in dollars. We calculated the number of successful, failed, and canceled campaigns, using the COUNTIFS(Kickstarter!$D2:$D4115,"<=1000",Kickstarter!$F2:$F4115,"successful",Kickstarter!$R2:$R4115,"plays") formula, that was filtered based on our criteria of what goal we wanted to look at. For this exercise we wanted to look at all campaigns ranging from less than 1000 to campaigns that had a goal of larger than 50000.

    We also calculated a percentage by taking the total number of projects divided by the number of failed, successful or canceled projects. Then to showcase the distribution, we added the data to a plot chart.
	

### Challenges and Difficulties Encountered
	The only challenge I experienced when working with this data set was when building out the counts of successful, failed, and canceled campaigns. At times my script was wrong, so my chart did not look like the example. I found myself going through each cell in order to find my issue. This had come about because I copied over my formula too early, instead of verifying that it was a good formula before copying and pasting.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	Some common trends that can be scene from the data was that most of the kickstarted campaigns occured during the summer months from May - July.
	The most canceled kickstarted campaigns occurs in the late 
    winter months from Jan - Mar.


- What can you conclude about the Outcomes based on Goals?
	Some common trends regarding plays are that none of the play campaigns were canceled. I can also see that the number of successful campaigns occurs when a lower goal is set. On the flip side, the higher the goal, the more likely it is to fail.

- What are some limitations of this dataset?
    I would say that some limitations of this dataset is that we are only focusing on campaigns that were pledged through kickstarter. What about the campaigns that are funded through facebook or through gofundme? There also may be a huge sample size of local campaigns that we could be missing out on. 

- What are some other possible tables and/or graphs that we could create?
    If i were to create more tables around this data it would be related to the spotlight, or perhaps related to the backers. With this information i think i would try to find out why a particular campaign may have been in the spotlight.
    I also could see a pie chart being created for the total amount pledged, and comparing it to the subcategory that had the most amount of kickstarted pledged.