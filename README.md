# Movielens-Case-Study

## Background of Problem Statement :

The GroupLens Research Project is a research group in the Department of Computer Science and Engineering at the University of Minnesota. Members of the GroupLens Research Project are involved in many research projects related to the fields of information filtering, collaborative filtering, and recommender systems. The project is led by professors John Riedl and Joseph Konstan. The project began to explore automated collaborative filtering in 1992 but is most well known for its worldwide trial of an automated collaborative filtering system for Usenet news in 1996. Since then the project has expanded its scope to research overall information by filtering solutions, integrating into content-based methods, as well as, improving current collaborative filtering technology.

## Problem Objective :

Here, we ask you to perform the analysis using the Exploratory Data Analysis technique. You need to find features affecting the ratings of any particular movie and build a model to predict the movie ratings.

## Domain :
Entertainment

## Analysis Tasks to be performed:

1.  Import the three datasets
2.  Create a new dataset [Master_Data] with the following columns MovieID Title UserID Age Gender Occupation Rating. (Hint: (i) Merge two tables at a time. (ii) Merge the tables using two primary keys MovieID & UserId)
3.  Explore the datasets using visual representations (graphs or tables), also include your comments on the following:
    a.    User Age Distribution
    
    b.    User rating of the movie “Toy Story”
    
    c.    Top 25 movies by viewership rating
    
    d.    Find the ratings for all the movies reviewed by for a particular user of user id = 2696
    
4.  Feature Engineering:
            Use column genres:


    a.  Find out all the unique genres (Hint: split the data in column genre making a list and then process the data to find out only the unique categories of genres)
    
    b.  Create a separate column for each genre category with a one-hot encoding ( 1 and 0) whether or not the movie belongs to that genre. 
    
    c.  Determine the features affecting the ratings of any particular movie.
    
    d.  Develop an appropriate model to predict the movie ratings
    
    
## Dataset Description :
There are three datasets names user.dat, ratings.dat, movies.dat
These files contain 1,000,209 anonymous ratings of approximately 3,900 movies made by 6,040 MovieLens users who joined MovieLens in 2000.

### Ratings.dat
 Format - UserID::MovieID::Rating::Timestamp

Field     	Description


UserID :	Unique identification for each user

MovieID :	Unique identification for each movie

Rating :	User rating for each movie

Timestamp: 	Timestamp generated while adding user review


UserIDs range between 1 and 6040 

The MovieIDs range between 1 and 3952

Ratings are made on a 5-star scale (whole-star ratings only)

A timestamp is represented in seconds since the epoch is returned by time(2)

Each user has at least 20 ratings

### users.dat

Format -  UserID::Gender::Age::Occupation::Zip-code


Field 	Description

UserID :	Unique identification for each user

Genere :	Category of each movie

Age :	User’s age

Occupation :	User’s Occupation

Zip-code :	Zip Code for the user’s location

All demographic information is provided voluntarily by the users and is not checked for accuracy. Only users who have provided demographic information are included in this data set.

Gender is denoted by an "M" for male and "F" for female


Age is chosen from the following ranges:

Value	Description

1	"Under 18"

18	"18-24"

25	"25-34"

35	"35-44"

45	"45-49"

50	"50-55"

56	"56+"


Occupation is chosen from the following choices:

Value 	Description


0 	"other" or not specified

1   "academic/educator"

2    "artist”

3	  "clerical/admin"

4	  "college/grad student"

5	  "customer service"

6	  "doctor/health care"

7	  "executive/managerial"

8	  "farmer"

9	  "homemaker"

10	"K-12 student"

11	"lawyer"

12	"programmer"

13	"retired"

14	 "sales/marketing"

15	"scientist"

16	 "self-employed"

17	"technician/engineer"

18	"tradesman/craftsman"

19	"unemployed"

20	"writer”


### movies.dat

Format - MovieID::Title::Genres

Field 	Description

MovieID:  Unique identification for each movie

Title : A title for each movie

Genres: Category of each movie


Genres are pipe-separated and are selected from the following genres:
1.Action
  
2.dventure

3.Animation
  
4.ildren's
  
5.Comedy
  
6.Crime
  
7.Documentary
  
8.Drama
  
9.Fantasy
  
10.Film-Noir
  
11.Horror
  
12.Musical
  
13.ystery
  
14.Romance
  
15.Sci-Fi
  
16.Thriller
  
17.War
  
18.Western


Some MovieIDs do not correspond to a movie due to accidental duplicate entries and/or test entries

Movies are mostly entered by hand, so errors and inconsistencies may exist
