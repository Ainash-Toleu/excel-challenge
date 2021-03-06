# Kickstarter analysis using Excel

Kickstarter – is a crowdfunding service that launched more than 300,000 projects and raised over $2 billion.
For this project, I analyzed a selected database of 4,000 projects from launched campaigns on Kickstarter.
---

## Analysis performed at the end of the Project

1.	Given the provided data, what are three conclusions I can draw about Kickstarter campaigns?
* From the Pivot_Table_1 tab I created, it is evident that compared to others,
    - “Theater”,
    - “Music” and
    - “Film & Video” 
categories had more successful launched campaigns,

where the “Music” category was the most successful in all the countries one with 540 successful (120 failed) out of total 700 launches.

and the least successful campaigns were in the “Food” category with 140 failed campaigns (34 successful) out of total 200.
![Screenshot](image/Picture1.png)

* Analyzing the information on a sub-category level (Pivot_Table_2), I can see that 

    -	within the successful “Music” category:
        + “classical music”, 
        + “electronic music”, 
        + “metal”, 
        + “pop”, 
        + “rock” subcategories had 100% success, 
    
    the “jazz” subcategory failed all 60 out of its launched campaigns and 

    the “faith” subcategory had 40 failed campaigns with another 20 still live. If previous performance is any indication of past success, I would expect these 20 faith campaigns to also fail.
    ![Screenshot](image/Picture2.png)


    - from the least successful “Food” category:

        + “restaurants” subcategory was 100% failed and 

        + “food trucks” subcategory was failed with 120 campaigns out of 140 (20 campaigns are still live). Again, if previous performance is any indication, I would expect these 20 live 'food trucks' campaigns to also fail. 

        + the “Small batch” subcategory showed 34 successful campaigns out of 40 (6 are live).
        ![Screenshot](image/Picture3.png)

    -	by analyzing all subcategories, I can see that:
        
        100% success in launches had subcategories: 
        + “classical music”,
        + “documentary”, 
        + “electronic music”, 
        + “hardware”, 
        + “metal”, 
        + “nonfiction”, 
        + “pop”, 
        + “radio & podcasts”, 
        + “rock”, 
        + “shorts”, 
        + “tabletop games”, 
        + “television”

        100% failed campaigns had subcategories:
        + “animation”, 
        + “children’s books”, 
        + “drama”, 
        + “fiction”, 
        + “gadgets”, 
        + “jazz”, 
        + “mobile games”, 
        + “nature”, 
        + “people”, 
        + “places”, 
        + “restaurants”, 
        + “video games” 
        ![Screenshot](image/Picture4.png)

* Analyzing the campaigns by the month (Pivot_Table_3),
    -   I can see that campaigns launched in the month of May had the highest count of successful campaigns during the year, at 234. The month with the highest count of failed campaigns were July (150), closely followed by January (149), and October (149).
    ![Screenshot](image/Picture5.png)

    -   looking at the most and least successful categories (“Music” and “Food”),
        + I can see that for “Music”:
            + the most successful months were January and May (54 successful campaigns each)
            + the least successful month was October with 16 failed campaigns
            ![Screenshot](image/Picture6.png)

        + for “Food” category:
            + the most successful month was May, with 6 successful campaigns
            + the least successful month was January, with 22 failed campaigns
            ![Screenshot](image/Picture7.png)
            
        Across the various categories, it seems that campaigns launched in the month of May had the most success. 

2. What are some limitations of this dataset?

When looking at the "state" column, there are 4 different types of campaigns: campaigns that were successful, failed, canceled, or is currently live. The "canceled" category raises some questions, because it is not determined why those campaigns were canceled. Would cancellation mean a failure because the campaign organizer lost determination, or perhaps a success because the organizer was able to meet their financial goals with donations outside of Kickstarter? Additional information would be needed to better analyze this data.

The launch and deadline dates provided were unix timestamps and not very user friendly. Providing the dates in a standard MM/DD/YYYY format would have been more straightforward and avoid additional calculations. 

The category and sub-category would ideally be separated, and we wouldn't have to perform additional work to separate those using the "/" sign. The situation would have been more complex if the "/" sign wasn't used consistently to separate the categories and sub-categories. 

Individual donation-level data would add a new perspective and complexity to the results, since we could then determine if the campaigns were successful because of a few individuals' large donations, or a 'team-effort' approach with most of the donations falling within a small range.

3. What are some other possible tables and/or graphs that we could create?

    * When analyzing campaigns by month, we could analyze the data by % of successful and failed campaigns in each month. 
    
    It would then be evident that the most successful launch months were May (61%) and April (60%). The worst month was December with 47% of campaigns launched failed.
    ![Screenshot](image/Picture8.png)

    * Looking at the data on relative, rather than absolute terms (Pivot_Table_3) adds additional analysis opportunities.
    
    Furthermore, we could analyze successful and failed campaigns by country.
    
    Then we would see that “Music” (for example) category had success performance not only in overall countries, but almost in all of the countries:
    
    IT, AT, AU, DK, SE, ES had 100% success,
    FR, CA, GB and US had overall success over 70%,
    and only DE had 50%
    ![Screenshot](image/Picture9.png)

    * Data given by year was not analyzed, were there any successful years compared to others or not? Presumably, campaign success and the overall economic conditions would correlate positively, and campaigns launched in 2009 would have less favorable outcomes than campaigns launched more recently. 
    * In analysis, we don’t consider the actual amount of money that was raised for the campaigns. Since the amounts were in currencies other than $USD, additional calculations to convert these amounts to $USD would have helped analyze the data from a different perspective. Additionally, we calculate, but don't analyze how many people participated in the campaigns including the average donation per person, per campaign. 
    * Analysis could be performed on the date period between the launch and the end date of the campaign. Presumably, campaigns with longer periods of time between the launch and deadline date would have higher success rates than those with shorter dates. A longer period to allow donations would allow for more time and people to donate.

### Bonus Statistical Analysis
1.	Use your data to determine whether the mean or the median summarizes the data more meaningfully.

Mean – average, take all the values, add them up and divide by the number of values we have.
Median – this is the value in the middle, takes all the values, sort them from smallest to largest and then find the value in the middle of the list.

According to Bonus Statistical Analysis table:
* average number of backers for a successful campaign: 194.43;
* average number of backers for a failed campaign: 17.71;

* the median number of backers for a successful campaign: 62;
* median number of backers for a failed campaign: 4

By given data I can say that Median summarizes the data more meaningfully. It shows us the average of backers in all the campaigns.










    



        




    



