# National_Warfighting_Capability
Dataset:
Power At Sea: A Naval Power Dataset, 1865-2011 by Brian Crisher and Mark Souva.
Shape: 8842 rows, 19 columns
Data organized temporary and by country

Cleaning
● Country names were made to be consistent
● Dropped all data before 1906 as none of it had ship data
● Dropped all columns not related to national capacity
● Dropped all missing values Training preparation
● One-hot encoded the country column
● Removed the labels from the data
● Split the data 80/20 for training/testing

Classifiers
● We used both the Decision Tree classifier and the K-Nearest Neighbors classifier
● Target was national capability

Decision Tree classifier:
● Train set accuracy: 100%
● Test set accuracy: 90.03%
● Confusion Matrix:
[279 8]
[8 283]
K-Nearest Neighbors classifier (k=4)
● Train set accuracy: 78.38%
● Test set accuracy: 64.30%
● Confusion Matrix:
[239 45]
[ 54 219]

The results tell us that given the nine variables we selected, one can somewhat accurately predict a nation’s naval capabilities. For our data, the decision tree classifier was clearly the superior choice, as it was 90% accurate, whereas the KNN classifier was only 64% accurate. Possible Sources of Error
● Differences in ship capability over time and by ship, along with maintenance and procurement.
● Small nations biasing data due to low ship counts.
● Different regional concerns biasing navy's towards maritime law enforcement rather than warfighting.
● Countries with navies being land based powers, and over focusing on land capabilities.

Implications: Nations naval capabilities can be determined by analysis from very few easily available inputs, even for nations that have very small navies. Such a tool can be used for rapid assessment of capabilities and projected force structure.
