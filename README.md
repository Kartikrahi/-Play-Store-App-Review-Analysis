# -Play-Store-App-Review-Analysis
# OBJECTIVE
we were provided dataset of playstore apps and our main objective is perform EDA and draw usefull conclusion out of it.
# DATASET
We're given a playstore app dataset, this dataset contains information of apps
it contains the following features.

-App = Name of app.

-Category = category of app.  

-Rating = Rating out of 5. 

-Reviews = Total no. of reviews.

-Size = Size of app in mb and kb

-Installs = Total no. of installs

-Type = Weather app is free or paid

-Price = price of paid apps

-Content Rating = Who can rate this app (Everyone, Teen, Adult, etc)

-Genres = Category of app with some more info about app.

-Last Updated = ddate of app last updated.

-Current Ver = Current version of app

-Android Ver = Android version in app will work.
- Total no. of rows are 10841
- Total no. of columns are 13
# DATA CLEANING
## (1) Handling null values
- nul values in column Rating replaced by mean of Rating.
- nul value in column Current Ver replaced by mode of Current Ver.
- nul value in Android Ver replaced by mode of Android Ver.
- nul value in Content Rating replaced by mode of Content Rating.
- nul value in Type is replaced by mode of Type.
## (2) Checking Outliners
- there is a outliner in rating, deleting the row of outliner.
## (3) changing some data type of columns to appropriate data type.
- changing Price column to float data type.
- changing installs  column to int data type.
- changing Size column to float data type.
- changing Reviews column data type to int datatype.
## (4) Remove duplicate rows if any.
##(5) finding out WHICH CATEGORY OF APP HAS HIGHEST AND LOWEST RATING.
- making sns.barplot to show the graph.
##(6) Finding out  WHICH CATEGORY HAS MAXIMUM AND MINIMUM APPS.
- using sns.countplot to make the bar graph.
##(7) Finding PERSENTAGE OF PAID APPS AND FREE APPS.
- Using sns.countplot to make the graph.
##(8) Finding WHAT CATEGORY OF SIZED APP HAS HIGHEST INSTALLS.
- Making a new column naming it size_category.
- putiing two values in it 'Below 50' and 'Above 50'.
-Using sns.countplot to make the bar graph.
##(9) Finding HIGHEST NO OF APP WORKS IN WHICH ANDROID VERSION.
- Using plt.bar to amke the garph.
## (10) Finding WHICH CATEGORY OF APPS HAS HIGHEST INSTALLS.
-  Using sns.barplot to amke the graph.
##(11) Finding WHICH PAID APP HAS HIGHEST REVENUE.
- Making a new column and naming it 'Revenue' by multiplying 'price' and 'installs'
- sorting revenue and slicing top 4 
- Using sns.barplot to make the graph. 
##(12) Making the coorelation heat map.
- Using sns.heatmap to amp the heat map.

