# Accenture-Dashboard

### DESCRIPTION

Social Buzz is a new social media with modern technologies. The company was established by two former engineers, one from London and the other from San Francisco. This platform emphasizes content by keeping all users anonymous, only tracking user reactions to every piece of content.

Over the past 5 years, Social Buzz has reached over 500 Million active users each month and they can’t handle this volume of information internally because they are still a small company. This is where I come in because I thrive at the intersection of data and strategy to help my clients manage and understand their big data.

### PROBLEM STATEMENT

The client has reached a massive scale within recent years and does not have the resources internally to handle it. So they need an analyst to provide an in-depth understanding of the company’s big data. An audit of their big data practice and recommendations for a successful IPO has to be done. The problem this analysis addresses is identifying content categories that highlight the top 5 categories with the largest aggregate popularity.

### OBJECTIVES

To give a background on how much data the platform has been creating, I was told that the platform receives over 100,000 posts per day which amounts to 36,500,000 posts every year, of which, this is all unstructured data making it very hard to make sense of.

In this day and age, content is king. Just look at some of the biggest platforms in the world, for example; YouTube, Facebook, and Netflix etc… they are all content businesses.

But how to capitalize on it when there is so much? It’s not just all about harvesting as much content as possible. The real value is in understanding and crunching this content to gain a deeper understanding of your audience and to therefore provide a more personalized and enjoyable experience. And this is where my data analytics expertise comes in.

### DATA OVERVIEW

The dataset used in this analysis contains detailed information about social Buzz. Here’s an overview of the key columns in the dataset:

* Reaction Type: The different types of reactions across the platform.

* DateTime: The date and time of when each content was posted, useful for identifying trends over time or by season.

* Content ID: Unique identifier for each content posted on the platform.

* Content Type: The types of content that can be posted on the platform.

* Category: The various posts across the platform which include; Animals, Dogs, Food, Science, Soccer, Tennis, Travel, etc.

* Sentiment: User’s view about a particular content.

* Scores: Rates each reaction type.

* Day Name: The days of the week each content was posted on the platform.

* Month Name: The month of the year each content was posted on the platform.

* Year: The year each content was posted on the platform.

### DATA CLEANING

In preparing the social buzz dataset for analysis, a few essential data-cleaning steps were taken to ensure accuracy and consistency.

* Duplicate Data: Using content ID, I checked to ensure that no content was repeated since each content has a unique ID. Duplicate rows might indicate data entry errors or system issues.

* Null Values: I examined to check for missing values and I observed that some rows had missing values. So I removed those rows since they didn’t tamper with the data.

* Data Format: Some columns didn’t have their correct data type, so I ensured that each column used its authentic data format.

* Data Extraction: I used Power Query Editor to extract the Day Name, Month Name, and Year from the date timestamp useful for identifying trends over time or by season.

* Data Consistency: I deleted the user ID column in both the content and reaction table. I also took out the URL column because they weren’t relevant to our analysis.

### DATA MODELING

I merged the content table to the reaction table because they had content type in common and merged the reaction type table to the reaction table because they had reaction type in common. After this was done I was left with only one cleaned dataset to use for my analysis.

*NOTE: I used the Reaction table as my base table because it had correlating columns with the content and reaction type table.

*Hint: Power Query makes Data Cleaning & Modeling less tasking.

### DATA ANALYSIS

KPIs

In the data analysis phase, I focused on key performance indicators (KPIs) that provide insight into Social Buzz’s platform. These KPIs highlight the unique category, total reactions, top category, and top month, offering more valuable insights into the platform. Here are the main KPIs derived from the dataset, and there are explained below:

* Unique Category: This represents the number of individual categories contained in the dataset. So this means that we have 16 unique categories across the platform.

* Total Reaction: A total of 24,573 reactions were registered across the platform by users.

* Top Category: The Animals category was the highest category by popularity using the reaction type score to calculate this.

* Top Month: The month of May is the month with the most number of contents per month with about 2,138 number of contents.

### COMPONENTS OF THE DASHBOARD

* Sentiment by Category: This effectively visualizes sentiment distribution across categories. It shows how users viewed their content on the platform.

* Content Type by Reaction: This breakdown helps our client understand which content type has the most reactions from users on the platform.

* Daily Reactions: This helps us to identify trends across the week. It presents the number of daily reactions across days of the week.

* Top 5 Reaction by Score: This represents only 5 out of the 16 reaction types on the platform. I decided to show just 5 because it would be easier to draw insights from the top 5 most used reactions.

* Category by Score: In this radar chart, each category represents a dimension of data performance, with values plotted along their respective axis. We decided to refer to only the Top 5.

* Content by Month: This line graph displays monthly content data for a year. This pattern shows two major peaks (January and May), with moderate fluctuations across the months.

### INSIGHTS

I extracted the Day Name, Month Name, and Year using the date timestamp to draw more insights into daily, monthly, and yearly analysis. This helped me identify the month of “May” as the month with the most number of contents throughout the year and I observed that “Mondays” have the highest number of reactions on the platform.

Based on my analysis, I could deduce that photos have more reactions than any other content type on the platform. I was able to extract the top 5 reactions used by users on the platform, and they are; super love, adore, want, cherish, love.

The data set provides more insights into sentiments. I observed that the most number of sentiments across the platform by category are positive. This means that users viewed most of the content on the platform positively.

### CONCLUSION

In conclusion, the project highlights the top 5 categories with the largest popularity. From my analysis, I found out that “Animals” and “Science” are the two most popular categories, suggesting that users like “real-life” and “factual” content.

I also discovered that food was a common theme amongst popular content and the most popular food category was healthy eating. This could be a signal to show the types of people who are using the platform, and you could use this insight to boost engagement even further. For example, you could run a campaign with content focused on this category or work with healthy eating brands to promote content.
