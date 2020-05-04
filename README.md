Introduction
	
Speed dating has been a way to meet a potential romantic partner for many years. In 2002-2004, a speed dating experiment was conducted on graduate students from Columbia University by researchers to find out if there are certain traits and attributes that a person desires for a potential mate based on gender differences. Using the data from this survey, I aimed to predict the likelihood that two speed daters, based on certain attributes, would both agree to a second date.

Format of Survey

Pre-Survey: Subjects were made to fill out a pre-survey based on their profile (i.e. race, degree, gender, etc.), desired attributes they wanted in a partner, and their preferences for a date (e.g. movie, museums, hiking, etc.)
Speed Dating scorecard: Subjects scored the partner based on 6 attributes: Intelligence, Ambition, Sincerity, Attractiveness, Shared Interests, and Fun. The subjects also scored how much they generally liked the partner and if they would go on a second date with them.

Source of Dataset: (http://www.stat.columbia.edu/~gelman/arm/examples/speed.dating/)

The dataset was taken from Kaggle. Reference for the study conducted can be found here: https://faculty.chicagobooth.edu/emir.kamenica/documents/genderDifferences.pdf.
This dataset has 8379 rows and 195 columns.

Data Cleaning

The first step that I did was to get a summary of my data and figure out if there were any duplicates. Then, I decided to remove the variables that contained more than 900 missing values.


Exploratory Data Analysis: Data Visualization

Plots were made to see the different characteristics of the subjects who joined the experiment.
Majority of speed daters were Caucasian for both genders.
Majority of males were pursuing business degrees while majority of females were pursuing Education.
Majority of males were in banking, consulting, finance, and business.
Majority of females were in academia and research

Gender Differences

Males desired Attractiveness in a partner more than females.
Females desired Intelligence and Ambition in a partner more than males.

Correlation Heatmap: none of the 6 attributes seemed to have a correlation with the variable ‘match’.
More males get more rejections than females for a second date.


Data Modeling
 
Logistic Regression: I then performed a logistic regression to predict whether a match could be made just knowing the decision of the subject (to see the partner for a second date) and if the subject generally liked the partner.
Without knowing the partner’s decision, if the subject liked the partner and decided on a second date, there is an 83% chance that the partner thought the same and there is a match!

Validating the Model

I performed cross-validation in order to validate the model.
