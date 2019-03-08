# LinearModelwithR
Using R programming language is excellent for linear model. 

I am a fan of Python rather than R. But I have to admit that for linear regression and linear models, R is much better than Python.

Unfortunately there are very limited "complete" references in Chinese for this field. Some of the documents are even wrong. 

A complete linear model with R should compose these parts:
1. Linear Regression(Single linear regression or Multi linear regression). 
For here, that is just a problem of solving linear equation systems. We could use theories from linear algebra(From Cramer's rule to Gauss elimination, there are a lot of methods) or Newton's Method from optimization theory(Not from physics) to calculate it.

Then you need to implement t-test for signle feature and F-test for the whole system. If it really works(p-value is less than 0.05) you could continue.

2. Model Diagnostics.
All the linear models are based on the coming five hypothesis:
• Normal i.i.d. errors
• Constant error variance
• Absence of influential cases
• Linear relationship between predictors and outcome variable
• Collinearity
So you need to test it. You could start from Diagnostics-plot(This article is written by me in Chinese, for English version, refer to the book of Julian Faraway, former professor of Univ Michigan and now UBath in England, Linear Model with R or something related).

In this project I will give you another detailed summary on this! It is hard, but don't worry, this is a well-established field.

My summary:
https://blog.csdn.net/qq_35837578/article/details/88357551

Link to Julian Faraway's book:
http://www.utstat.toronto.edu/~brunner/books/LinearModelsWithR.pdf

3. Model Transformation
You could use a lot of model transformation to improve the model. 

That may include but not exclude to:
1. Box-Cox(Model Transformation)
2. Log-Transformation(Model Transformation)
3. AIC/BIC/Cp/Adjusted-R^2(Model Selection)
4. LASSO
5. Ridge Regression
6. Elastic Net
...

But beware of the overfitting problem!

If it does not work, just don't worry, try other non-parametric statistics and/or machine learning algorithms!

If you feel it helps you or still have questions, please feel free to connect with me via linkedin(Ruimeng Wang, alumni of UIUC and Sichuan University) or send me emails: brianrwangmsecs@gmail.com 
