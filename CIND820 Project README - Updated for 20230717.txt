1. Title: CIND820 Project

2. Purpose: 
	Using machine learning techinques and a given dataset accesible throught the link in the report, 
	the purpose of this paper is to understand if certain features of a mushroom can be used to determine if it is poisonous or edible.

3. Dataset Info (no miss file):
	(c: categorical, n: numerical) 
	a. class			p = poisonous, e= edible
	b. cap-diameter (n):		float number in cm
	c. cap-shape (c):       	b = bell, c = conical, x = convex, f = flat, s = sunken, p = spherical, o = others
	d. cap-surface (c):     	i = fibrous, g = grooves, y = scaly, s = smooth, d = dry, h = shiny, l = leathery, k = silky, t = sticky, w = wrinkled, e = fleshy
	e. cap-color (c):            	n = brown, b = buff, g = gray, r = green, p = pink, u = purple, e = red, w = white, y = yellow, l = blue, o = orange, k = black
	f. does-bruise-bleed (c):	t = bruises or bleeds, f = does not bruise or bleed
	g. gill-attachment (c):      	a = adnate, x = adnexed, d = decurrent, e = free, s = sinuate, p = pores, f = none
	h. gill-spacing (c):         	c = close, d = distant, f = none
	i. gill-color (c):           	see cap-color + f = none
	j. stem-height (n):		float number in cm
	k. stem-width (n):		float number in mm   
	n. stem-color (c):		see cap-color + f = none
	q. has-ring (c):            	t = has ring, f = does not have ring
	r. ring-type (c):           	c = cobwebby, e = evanescent, r = flaring, g = grooved, l = large, p = pendant, s = sheathing, z = zone,
						y = scaly, m = movable, f = none
	s. habitat (c):             	g = grasses, l = leaves, m = meadows, p = paths, h = heaths, u = urban, w = waste, d = woods
	t. season (c):			s = spring, u = summer, a = autumn, w = winter

4. Literature Review:
	This portion of the report dives into into the significance of the project. It details mushroom use and covers serveral forms of machine learning on similar projects.
	Additionally, there is some detail on the methodology of how the project will be performed including the preperation and cleaning of data, exploratory data 
	analysis (EDA), data visualization, modeling and validation of those results.

5. Exploratory Data Analysis:
	In this section, steps are taken to clean and preprocess the data. This includes checking the dataset for null variables, feature engineering, identifying influential
	predictors, Hypothesis testing, dimensionality reduction and data visualization.
	This step aslo defines our key questions we want to answer:
		a. What are the key characteristics that differentiate a toxic mushroom from a non-toxic one?
		b. Are there specific patterns or variations that serve as strong indicators of mushroom toxicity?
		c. Are there geographic features that can be incorporated into identification protocols?
		d. Can machine learning or AI algorithms assist in the automated identification of toxic mushrooms?

6. Initial Results:
	This step calculates the accuracy of each of the four selected models: logistic regression, naive bayes, decision tree and random forest.

7. Evaluation:
	This portion further looks into validity metrics of each model and selects the most appropriate model to answer each question.

8. Final Results:
	Questions are answered and disadvantgeous points are identified.