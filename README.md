# Movies-ETL

## Challenge Assignment 8:

Challenge was to write a Python script that performs all three ETL steps on the Wikipedia and Kaggle data. Utilize the code you created in your Jupyter Notebook but leave out any code that performs exploratory data analysis, and you may need to add code to handle potentially unforeseen errors due to changes in the underlying data.

### GOALS

- Create an automated ETL pipeline.
- Extract data from multiple sources.
- Clean and transform the data automatically using Pandas and regular expressions.
- Load new data into PostgreSQL.

### Assumptions

Using data from open sources such as wikepedia and kaggle may have inconsistent data.  In an effort to standardize, the following assumptions have been included:

- Data needs to be cleaned.  After an initial test to develop the program, there was inconsistent data and missing values.  
- Wikepedia does not have strict standards on how data is presented.
- Data included is restricted to only entries with a director and IMDB link.
- Filtered out TV shows by determining number of episodes.
- Combined alternate titles for the movie by reviewing existing data.
- Combined similar column types for Director (Example:  Directed By and Director).
- Removed null columns that stored no reference data.



### Column Name Renaming (original path data)
- ('Adaptation by', 'Writer(s)')
- ('Country of origin', 'Country')
- ('Directed by', 'Director')
- ('Distributed by', 'Distributor')
- ('Edited by', 'Editor(s)')
- ('Length', 'Running time')
- ('Original release', 'Release date')
- ('Music by', 'Composer(s)')
- ('Produced by', 'Producer(s)')
- ('Producer', 'Producer(s)')
- ('Productioncompanies ', 'Production company(s)')
- ('Productioncompany ', 'Production company(s)')
- ('Released', 'Release Date')
- ('Release Date', 'Release date')
- ('Screen story by', 'Writer(s)')
- ('Screenplay by', 'Writer(s)')
- ('Story by', 'Writer(s)')
- ('Theme music composer', 'Composer(s)')
- ('Written by', 'Writer(s)')
