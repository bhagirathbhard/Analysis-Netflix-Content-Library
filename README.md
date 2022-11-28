# **<span style="color:#023e8a;font-size:200%"><center>Analysis of Netflix Content Library</center></span>**

## <center>By: Bhagirath Bhardwaj, Jinisha Kande, Paulin Jesintha Mariadoss, Renata Halim, Sohil Jain, and Sonal Kaur</center>

# **<span id="Project-Overview" style="color:#023e8a;">Project and Dataset Overview</span>**

**Netflix Content Analysis**

Netflix is the pioneer of internet media and entertainment streaming. Over the years it has faced several challenges and also overcome a shift in demographics, changing viewership styles and choices.

Netflix’s content library and their recommendations engine play a big role in influencing the content consumed by people worldwide. Research from Netflix shares that over 80% of the content watched on their platform came from
their recommendations engine. 

As Netflix has over 100 million users worldwide, it becomes crucial for Netflix to implement a strong data-driven algorithm to recommend customized movies and TV shows to its audience.

The following project is interested in studying the changes in Netflix’s content strategy over the years. We are curious to know if or to what extent these changes resulted from cultural and target audience changes in Netflix's subscriber base.

*   Perform Exploratory Data Analysis, Data cleanup on the dataset using Python.
*   Analyze variables in our dataset such as actors, genres, directors, ratings etc.
*  Find answers to key questions and trends around Netflix’s investment into various kinds of media content.

# **<span id="Data-Sources" style="color:#023e8a;">Data Sources</span>**


Our dataset was captured using a combination of tools and methods; scraping, API calls, and manual validation. Using these techniques, the author of the original dataset, Shivam Bansal, was able to capture information on a myriad of topics, namely on Netflix shows, movie titles, directors, casts, countries, release dates, ratings, and more. In total, our dataset has `12` columns and `8807` rows.

*   [Netflix-Shows by Shivam Bansal](https://www.kaggle.com/datasets/shivamb/netflix-shows)
*  [Clarification of Source of dataset by Author](https://twitter.com/shivamshaz/status/1452642649442172931?s=20&t=OSh8EM8VNMZhmXSi6aBgtA)

* [Scraped Data - Netflix Original Programming](https://en.wikipedia.org/wiki/List_of_ended_Netflix_original_programming)


In this project we utlize multiple datasets, a brief summary of all of them are as follows -

| Table/Dataset Name     | Brief Description | Characteristic, Data type|
| ----------- | ----------- |-------- |
| `netflix_ds` | Dataset containing a list of all tv shows and movies hosted on Netflix over the years.       |    Some data cleanup necessary.      |
| `netflix_originals_drama_ds`   | Dataset scraped from Wikipedia for all **Drama** Genre Shows **produced** by Netflix as a "Netflix Originals".        |  The reason we looked into this data is because of Netflix's recent success and weightage on this genre.        |


**I. netflix_ds**

| Column      | Brief Description |  Characteristic, Data type   | 
| ----------- | ----------- | ------- |
| `show_id`      | Unique `IDs` of each Movie and TV Show. Follows the syntax of `Sn` where `n` is the sr. number. (e.g. `S432`)      |  String, Unique, Primary Key, Not Null       |
| `type`   | Catagorical Variable defining if the row is for a `Movie` or `TV Show`        |   String, Not Null     |
| `title` | Title of the Movie or TV Show    | String, Not Null  |
| `director` |  Name of the Director of the Movie or TV Show   |    String    |
| `cast`     |  List of names of the Cast     |     String    |
| `country`   |    Country where the movie / show was produced    |     String   |
| `date_added`   |   Date it was added on Netflix   | Date Format     |
| `release_year`  |   Actual Release year of the move / show    |    Date Format |
| `rating`     |   TV Rating of the movie / show       |  Date Format    |
| `duration` |  Total Duration - in minutes or number of seasons| String  | 
| `listed_in` |   List of Genres under which the content was hosted by Netflix     |  String | 
| `description` |  The summary description     |  String   |

![image](https://user-images.githubusercontent.com/13074725/204328121-358c0afa-0467-4a9a-906f-d390d870feaa.png)

**II. netflix_originals_drama_ds**

| Column      | Brief Description |  Characteristic, Data type   | 
| ----------- | ----------- | ------- |
| `title`      | Title of the TV Show      |  String, Unique, Primary Key, Not Null       |
| `Genre`   | Specific Genre under the Drama Category of Netflix        |   String, Not Null     |
| `Premiere` | Date of Premiere of the TV Show   | Date Format  |
| `Finale` |  Date of the Finale of the TV Show   |    Date Format    |
| `Seasons` | Seasons and Episodes of the TV Show | String |
| `Runtime` | Duration | String |
| `Seasons_Only` | Manually split from `Seasons` column to only contain Seasons length | String |
| `Episodes` | Manually split from `Seasons` column to only contain total episodes | String |

![image (2)](https://user-images.githubusercontent.com/13074725/204328176-bbf3e189-cf6e-44a2-982a-6199775dc6ba.png)
