# Background:

The central question for this project is: What is the physicochemical component that influences wine quality the greatest? Each of the components alter the quality, but there could possibly be a component that stands out and plays a heavy role in determining a wine’s quality. Additionally, we would like to see what a wine’s input component values look like at each quality level and if certain elements of wine have a “relationship” (tendencies to use more or less of one component when a different component is added).

# About the data:

Our data is related to the red and white variants of the Portuguese “Vinho Verde” wine data collected by a team of scientists utilizing machine learning in an attempt to predict human wine taste preferences based on the contents of the wine. The data set includes the physicochemical (inputs) and sensory (the output) variables. The input variables are:

*fixed acidity* - most acids involved with wine or fixed or nonvolatile (do not evaporate readily)
*volatile acidity* - the amount of acetic acid in wine, which at too high of levels can lead to an unpleasant, vinegar taste
*citric acid* - found in small quantities, citric acid can add ‘freshness’ and flavor to wines
*residual sugar* - the amount of sugar remaining after fermentation stops, it’s rare to find wines with less than 1 gram/liter and wines with greater than 45 grams/liter are considered sweet
*chlorides* - the amount of salt in the wine
*free sulfur dioxide* - the free form of SO2 exists in equilibrium between molecular SO2 (as a dissolved gas) and bisulfite ion; it prevents microbial growth and the oxidation of wine
*total sulfur dioxide* - amount of free and bound forms of S02; in low concentrations, SO2 is mostly undetectable in wine, but at free SO2 concentrations over 50 ppm, SO2 becomes evident in the nose and taste of wine
*density* - the density of water is close to that of water depending on the percent alcohol and sugar content;
*pH* - describes how acidic or basic a wine is on a scale from 0 (very acidic) to 14 (very basic); most wine are between 3-4 on the pH scale;
*sulphates* - a wine additive which can contribute to sulfur dioxide gas (S02) levels, wich acts as an antimicrobial and antioxidant
*alcohol* - the percent alcohol content of the wine
The output variable is:
*quality* - output variable (based on sensory data, score between 0 and 10)

# Data modifications:

We first created a new data set, mutated_data, that mutated the original data set by changing the quality values to character values. Secondly, we created another data set, wine2, that summarized the original data set with the mean and standard deviation values for each input variable. Lastly, the third data set created, wine3, takes the original data set, groups by the quality value, and again summarizes with the mean and standard deviation of each input component. Wine3 is also used to create smaller data sets that are filtered by quality level for later use.

# Data citiation:

Learning, UCI Machine. “Red Wine Quality.” Kaggle, 27 Nov. 2017, www.kaggle.com/uciml/red-wine-quality-cortez-et-al-2009.

# Mission:

We started by examining the output component, quality, using various methods. Then, each of the input components were examined individually to show various features. A correlation chart was then created to determine if there are any relationships between the components. Lastly, a linear regression is used to determine the variables that influence the quality of wine the most.
