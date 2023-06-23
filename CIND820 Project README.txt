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

5. Modeling:
	a. Logistic Regression
		The logistic regression method on a test size of 30% resulted in an accuracy of 62.71%.
	b. Naïve Bayes
		The naïve bayes method on a test size of 30% resulted in an accuracy of 59.20%.
	c. Decision Tree
		The decision tree method on a test size of 30% resulted in an accuracy of 99.61%.
	d. Random Forest
		The random forest method on a test size of 30% resulted in an accuracy of 99.98%.

6. Model Results/Evaluation:
	a. Logistic Regression
		i. Accuracy: Accuracy: 	0.6270945909066099
		ii. Precision: 		0.6419166666666667
		iii. Recall: 		0.7523930455167025
		iv. F1 Score: 		0.6927781275294541
		v. AUC-ROC: 		0.6103917473036933
	b. Naïve Bayes
		i. Accuracy: 		0.5919982533704492
		ii. Precision: 		0.6099657725065669
		iii. Recall: 		0.7484860324282087
		iv. F1 Score: 		0.6721635016008071
		v. AUC-ROC: 		0.5711377335220346	
	c. Decision Tree
		i. Accuracy: 		0.9961246656841876
		ii. Precision: 		0.9961932650073206
		iii. Recall: 		0.9968743895292049
		iv. F1 Score: 		0.996533710882195
		v. AUC-ROC: 		0.9960247241472574
	d. Random Forest
		i. Accuracy: 		0.9998362534796136
		ii. Precision: 		0.9997070598574358
		iii. Recall: 		1.0
		iv. F1 Score: 		0.9998535084720933
		v. AUC-ROC: 		0.9998144253371273
	Based on the evaluation metrics of the above models, the random forest classifier has determined as the most appropriate model.

7. Key Feature Result:
	By utilizing the random forest classifier, we determinged the following features' importance in descending order:
		stem-height: 		0.14461048274262384
		cap-shape: 		0.09375286337359055
		gill-color: 		0.0931666003096277
		stem-width: 		0.08621129050950947
		gill-spacing: 		0.0857581742937454
		does-bruise-or-bleed: 	0.08555877947749156
		class: 			0.08281663617605152
		cap-surface: 		0.06088281845765875
		cap-diameter: 		0.05913975764133062
		gill-attachment: 	0.05024421674573872
		has-ring: 		0.0480585368006724
		cap-color: 		0.03520634643354958
		ring-type: 		0.03351114892828478
		stem-color: 		0.026130500969542034
		habitat: 		0.01495184714058319
	