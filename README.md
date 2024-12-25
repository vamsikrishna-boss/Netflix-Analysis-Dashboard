# Netflix-Analysis-Dashboard
The Netflix Analysis Dashboard provides insights into Netflix's catalog, including the distribution of movies and TV shows, popular genres, ratings, and their release trends over the years. Built using Tableau, this dashboard helps stakeholders understand content patterns and make data-driven decisions.

## Key Objectives

1. Analyze the distribution of movies and TV shows by country.
2. Understand content ratings and their popularity.
3. Explore top genres and their distribution.
4. Identify trends in content release over time.
5. Visualize the proportion of movies vs. TV shows in the catalog.

## Dashboard Features and Instructions

1. Total Movies and TV Shows by Country:

       Purpose: Visualizes the geographic distribution of Netflix content.
       Visualization: Interactive map using Tableau's Mapbox integration.
    Steps to Create:
      Use country as a dimension.
   
      Add a measure for distinct count of "Show ID."

      Use color to represent the number of titles (gradient scale).

3. Ratings Distribution:

       Purpose: Shows the count of titles under each rating category (e.g., TV-MA, TV-14).
       Visualization: Vertical bar chart.
   Steps to Create:
     Use "Rating" as the dimension.
   
     Add a measure for distinct count of "Show ID."
   
     Sort bars in descending order of count.

5. Top 10 Genres:
   
       Purpose: Displays the most popular genres on Netflix.
       Visualization: Horizontal bar chart.
    Steps to Create:
     Use "Genre" as the dimension.
   
     Filter to display the top 10 genres by distinct count of "Show ID."
   
     Use color coding for better differentiation.
     
7. Movies and TV Shows Distribution:
   
        Purpose: Highlights the proportion of movies vs. TV shows.
        Visualization: Bubble chart.
    Steps to Create:
     Use "Type" (Movie/TV Show) as the dimension.
    
     Add distinct count of "Show ID" as the measure.
   
     Adjust the size of bubbles based on counts.
    
9. Total Movies and TV Shows by Year:
    
       Purpose: Tracks the addition of content to Netflix over time.
       Visualization: Area chart.
   Steps to Create:
     Use "Date Added" as the dimension.
   
     Add distinct count of "Show ID" as the measure.
   
     Split by "Type" (Movie/TV Show) for layered visualization.
   
11. Description and Filters:
    
        Description: Displays metadata about selected content, including title, duration, release year, and a brief description.
        Filters: Enable interactive exploration by type, title, and release year.
    Steps to Create:
      Add a text box or tooltip for the description field.

      Create filters for "Type," "Title," and "Release Year" using Tableau’s filter functionality.

    Technical Configuration:
    
         Tool: Tableau Desktop
         Data Source: Netflix dataset (CSV, database, or API integration)
    
    Key Metrics:

          Count of Movies and TV Shows
          Genre Popularity
          Ratings Distribution
          Content Addition Over Time

    Calculated Fields:
    
         Content Proportion = Movies Count / Total Titles
         Year Extract = YEAR([Date Added])

    Filters:

         Type (Movie/TV Show)
         Country
         Release Year

## Future Enhancements:

1. Incorporate user engagement metrics (e.g., views, watch time).
2. Add filters for regional preferences or language.
3. Integrate real-time data from Netflix APIs for up-to-date analysis.

## Conclusion

This Netflix Analysis Dashboard provides a comprehensive view of Netflix’s content library. It enables stakeholders to analyze trends and patterns for strategic decision-making. For further customization or additional insights, enhancements can be implemented based on business requirements.

