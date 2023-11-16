# deltadataanalysisproject
Analyze the range of social acceptance of people of different cultures and categories across LSR and identify their impact on the student body.
Problem Statement:
Analyze the range of social acceptance of people of different cultures and categories across LSR and identify their impact on the student body.

Reason to choose the topic:
LSR is a diverse space, and compared to other DU colleges, it is a unique space that accepts different people from different cultural and social backgrounds. However, as someone who comes from a border town, which is a melting pot of different cultures, I struggled with my cultural identity a lot. I dreaded the “Where are you from?” question so badly, knowing I had no one-word answer. Answering that question required me to have a map handy and hope the person asking knows geography. 
One of the first friends I made here came from a different social world, and hearing about it caught me off guard. I grew up shielded and protected from even learning about the trauma these people went through. A teacher strangled a student for drinking water from the same spot as him because he didn’t fit an imaginary circle. 
Since then, I have always wanted to” unshield” myself, learn more about the experiences of others, and tell my own. The aim of this project is to learn about the silent struggles faced by students of LSR every day.  This project also attempts to analyze whether LSR is one, and if not, where do we fall short?

Data collection:
A Google form was circulated amongst the student body
The responses were from students across all departments
The number of responses received was 29
The questionnaire featured one drop-down question and all other yes/no and 1-5 scale questions
Here’s the link to the form: https://forms.gle/XWa1DBG4uaM2gtFr6
Here’s my dataset: https://drive.google.com/file/d/1g22d5N2pCzh-rO9kOWK-kATdI08Gmotz/view?usp=sharing (created from the google form responses)
Here’s my code file: https://drive.google.com/file/d/1pgCT4BYtO_89Hl3ouiOnbWPsMBJPWNu8/view?usp=sharing


Analysis & Visualization:

Data Cleaning
From the raw data collected by the google form, I created a dataset fit for analysis using various Python libraries like pandas, scipy and seaborn. After data cleaning, I read the dataset into a panas dataframe of 30 columns and 17 rows.

Data Visualization & Analysis
In my dataset, I had 17 variables in total, and the plots below represent three of those which I found interesting and representative of what the project aims to explore. As can be seen in Figure (a), almost half of the people who answered possess cultural identities that differ from their regional identities. These people are at high risk of being singled out. Next, in Figure (b), we notice that quite a few people feel accepted to a great extent on campus, but there is a good number who do not. Lastly, in (c), we notice diverse answers about how accepted people feel in their own cultural communities on campus.
This image shows how many people have cultural identities that differ from their regional identities 
This image shows how accepted do people feel on the LSR campus


c. This image showcases how accepted people feel in their own cultural communities on the LSR Campus


The processes were carried out in Jupyter Notebook. 

 To get an insight into the relationship among the 17 variables in the database, I created a heatmap using Seaborn. The heatmap represents the linear correlation between the variables calculated using the Pearson correlation coefficient. The extent of correlation can be determined using the scale on the right. The values on the scale range from -0.4 to 1.0, and the colors range from black to very light pink. The cooler the color, the higher the correlation. Here’s the figure:


Fig (d) - Seaborn heatmap depicting the correlation between 17 variables present in the database

From the figure, we can observe 8 significant correlations. I used the scipy.stats.pearson function is a correlation test that tells us about the level of association between two variables. It outputs two values, i.e., a statistic representing correlation and a p-value. The statistic is called the Pearson coefficient of correlation. It is represented by r, and the statistical formula is as follows:


The value of the Pearson coefficient is between -1 and 1. The closer the value is to 1, the higher the probability. 

The p-value in statistics is the probability that the results of the statistical hypothesis test will be at least as strong as the observed results (with the assumption that the null hypothesis is true). A lower p-value indicates that there is a higher probability of the correlation coefficient being relevant.

As a thumb rule, a p-value less than 0.05 is an indicator of the correlation being significant. The table below presents the 8 noteworthy correlations I observed, along with the correlation statistic and p-value.


S.N.
Variable 1
Variable 2
Pearson correlation coefficient
P Value
1
acceptance_genLSR
MH_diff
0.49736
0.00605
2
acceptance_genLSR
cult_rep
0.00604
0.02673
3
cult_rep
cultfood_rep
0.41012
0.02712
4
extent_disc
catg_disc_scale
0.57127
0.00121
5
disc_effect_grades
extent_disc
0.49453
0.00639
6
disc_effect_grades
catg_disc_scale
0.46026
0.01199
7
catg_disc_scale
catg_judgement
0.64695
0.00015


Table 1: This table depicts the Pearson correlation coefficients and p values for some noteworthy correlation among some variables in the dataset.

Observations as per this table
People’s acceptance by the LSR student body is directly proportional to the difference in their mental health after joining college. People less accepted experience worsened mental health as compared to before joining college.
People’s acceptance by the LSR student body is directly related to their cultural representation on campus. If a culture is represented on campus through various activities or events, the student body is likelier to accept the student and vice versa.
The representation of a particular culture is also reflected by the availability of the culture’s food offerings in the cafeteria. 
The discrimination that people face based on their cultural identities is greatly related to the level of discrimination they endure because of their category
The difference in people’s grades after entering college is related to the level of discrimination faced by them on the basis of their diverse cultures and categories
The feeling of constantly being put down by people coming from minority categories comes from a place of discrimination faced by them in college

Summary/Inference:
Students at LSR come from diverse regions, and amongst that, too, many of them have different cultural identities. While we should be proud that our institution hosts such a wide set of people, it becomes our responsibility to make them feel at home. It is not an easy task, but it is what’s necessary. 

The project took a deep dive into the mental health and academic struggles faced by students as a result of the discrimination they face on campus. It is important to note here that academic struggle at the undergraduate level may cripple a person for life since it is where one’s career basics are to be strengthened. Here, we are forced to ask ourselves, what did these people do to deserve this treatment? They didn’t fit a particular circle.

Now, the answer to the question of whether or not LSR is a safe space or not is in the negative. But based on my observations, the gap is not that large. If few changes are made in the way the campus operates, we could come a long way to being that inclusive space we so much desire to be. Students at LSR are bright and intelligent, and if just some ways of understanding and kindness are adopted into our campus culture, it will do wonders to boost the college lives of people belonging to minorities and/or other diverse communities.

There are a lot of silent battles in college among people who need to be addressed. People do not start from the same starting points. Everyone struggles in college, but for some people, the struggle starts from the first time they enter through these prestigious gates, while the struggle for some has started since they were born. As we transform into adults, I think it is important to understand the true concept of equality and be kind to everyone.

Here are a few suggestions, as per my observation, as to how LSR can be a safe space:
Onam is celebrated on campus, but is Lohri? We should discover ways to celebrate and inculcate more festivals and cultures in campus life.
The food options in the cafe should be expanded to include some northeastern food, among other cultural diets. More people will learn about different cultures and be less judgemental.
Sensitization sessions should be conducted across the campus to teach people how to behave in a culturally diverse setting.
Electives offering insights into cultures of different communities could be offered to the batches studying the NEP curriculum as VAC/SEC
Strong communities like the Northeast cell could be built for people from other regions, too.

These are just a few suggestions. Further studies could be done in this area to gain an even clearer insight into what exactly can be done to make LSR just as inclusive as it is diverse.
