### ***Project 2 Feedback***

***Nico Van de Bovenkamp***

***

**Overall:**  
Great work on this assignment! You made great use of various pandas, and matplotlib functionality. The only direct advice that I have is to keep on practicing and take note of some of the 'tricks' and best practices that you see in class. Please feel free to slack me if you have any questions at all! We are here to answer your questions. Also, if you would like some additional office hours, let me know and we would be happy to make a session happen.

**Some notes**  
* In *Question 3*, while it is true that certain majors will result in different biases in GPA, the reason GRE's std. dev. is higher, in absolute terms, than GPA is one of scale. The range of values that GRE can take on is much, much greater. Thus, there is much more opportunity for variation about the mean (ie. std. dev).
* In *Question 4*, nice use of a numpy function! Note, though, that you can also just use `DataFrame.dropna()` too!
* In *Question 9*, though it is true that it is not *exactly* normal, we usually would not quite say that it doesn't fit that assumption. What I would normally do is just flag that as a cause for concern or suspicion when it comes to making our model. If, for example, we were to build some form of linear regression to predict GRE score and we saw that there was some error, we could flag the non-normal distribution of the data as a cause for error.
* In *Question 13*, though I am sure you are a bit familiar given our most recent classes on classification, note that you would not use an OLS for this problem. You would want to use some form of classification model to solve this supervised learning task.
* Try out the imputation technique next time! When you have missing values, you might not want to impute a value like 0. For example, you could actually by saying that there exists students out there with a 700 GRE, Prestige 1.0 school, that was admitted to grad school, but they have a 0.0 GPA. This only imputes 'bad' noise into our model. What you could do is impute something like the median or mean to retain the value without disturbing the underlying distribution too much.
