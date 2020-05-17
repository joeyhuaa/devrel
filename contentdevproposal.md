**[Step-By-Step Technical Blog Guide](https://hq.bitproject.org/how-to-write-a-technical-blog/)**

### :pushpin: Step 1
**TITLE:**    
Intro to Supervised Learning

**TOPIC:**    
Regression and Classification models for Supervised Learning

**DESCRIPTION (5-7+ sentences):**    
This blog will teach the audience on the basics of learning how to train and test labeled data. The appropriate model to use depend on what type of data that you're working with. If you're working purely on quantitative values, you're best would be to create a regression model. If you're working with qualitative values, then using the classification model will be your best bet. The main goal is to see how the type of model that you'll use will actually predict the outcomes that you want to achieve.

### :pushpin: Step 2
:family: **TARGET AUDIENCE (3-5+ sentences):**    
The target audience will be undergraduate college students (Freshman or older) and older who have a basic backgorund on statistics. The reason as to why I picked this audience is because a fair amount of quantitative majors at university will have some basic exposure to probability and linear regression, so this knowledge in mind will be a descent prerequisite towards understanding some of the math behind these models. The amount of programming knowledge that the audience should have in python should be at a basic level for understandng syntax since we're not building functions, but rather introducing them to the applied techniques from the documentation of the packages.

### :pushpin: Step 3
> Outline your learning/teaching structure: 
- Differentiate the concepts between Regression and Classification
- Explain the necessary packages to use for the models (pandas, numpy, scikitlearn, and matplotlib)
- Explain how the function calls work for code snippets
- Give techniques to manipulate structure of data (for example, categorical data should be converted to numbers using scikitlearn's LabelEncoder since the machine learning packages don't really work very well with non-numerical values
- Give basic mathematical bacjground for what's happening under the hood
- Give context towards the outcome of our results from each model

**Beginning (2-3+ sentences):**    
This is where I explain the differences bewteen Regression and Classification based on what seems appropriate based on a specific metric that we're looking for. I also explain how the flexibility of a model can affect how accurate the model might be (less flexible = more up to interpretation (precision); more flexible = high level of accuracy).

**Middle (2-3+ sentences):**    
This is where I'll give the examples of using Regression and Classification models. A major component of it is creating the code snippets and explaining how the written functions in those snippets are manipulating our data in some way. This is also where I explain the mathematics for each chosen model (explaing the fundamentals of the linear regression formula and how the Root Mean Square Error (RMSE) is the measure of how far off the trained data is from the correct value (for regression); will also talk about how logistic regression (a type of classification model) will represent how our data corresponds to a binary variable (i.e. yes/no, male/female, etc...) and also measure how true (meaning accurate) positive/negative and false (meaning predicted) positive/negative values are calculated as in 4 proportions).

**End (2-3+ sentences):**    
I will reiterate the importance of knowing the 2 supervised learning methods for labeled data. I would remind them of the problem solving technique that the audience will gain from this such as if the type of the metric they want to measure is quantitative grwoth (you would use linear regression for that) or if their metric is based on binary categories (you would use logistic regression for that).