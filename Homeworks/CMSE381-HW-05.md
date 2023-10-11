# Homework 5

## CMSE 381 - Fall 2023

## Due Weds, Oct 18, 2023

### Instructions

This homework covers four classes. Problems listed below are from [the textbook](https://www.statlearning.com/).

- Weds 10/11, we covered 5.2 (Bootstrapping)
  - In this problem you will estimate the accuracy of the coefficients of a linear regression model using bootstrapping.
    - Using the `auto` data set, we will be using `horsepower`, `weight`, and `acceleration` to predict `mpg`. Be sure to do our usual loading and clearning on this data set prior to starting the next step.
    - Generate a bootstrap sample, fit a linear regression model, and find the coefficients of the model $\beta_0$, $\beta_{\texttt{horsepower}}$, $\beta_{\texttt{weight}}$, and $\beta_{\texttt{acceleration}}$
    - Repeat this process $B=100$ times and draw a histogram of each of the four coefficients.
    - Compute the standard error for each as discussed in class, also in Equation 5.8 in the book.
    - Which coefficient are you most confident in and why? Which are you least confident in?
- Fri 10/13, we covered 6.1 (Subset selction)
  - 6.6.1. Note that for part (c) you need to justify your choice of True/False.
- Mon 10/17, we covered 6.2.1 Ridge Regression, and Weds 10/19, we covered 6.2.2 Lasso
  - 6.6.9 (a-d, g)

### Submit homework to crowdmark

You will upload your homework to the crowdmark website. The main changes are:

- You will be emailed a link to the assessment and will upload your solutions to that page. [Here is a link to the Crowdmark help page with information on submitting the homework.](https://crowdmark.com/help/completing-and-submitting-an-assessment/)
- Answers to each question will need to be uploaded separately.  So this will basically require taking portions of the pdf you were generating before and separating them when uploading.  
- Feedback on the homework will be posted via the Crowdmark website
- Your overall grades will still be visible on D2L when they are posted.

### Important Reminders

- Homeworks must be typed. Some options for this include word, overleaf/latex, or by including a pdf of a jupyter notebook (not the .ipynb file please!). Some students have had more success in the jupyter case of printing from the browser window.  The "convert to pdf" option requires you to have latex installed.
- Including figures when explaining your reasoning is highly encouraged.  This can be done as easily as taking a picture of a hand-drawn sketch and including it in your file. Please be sure to include all figures in the main file so we only have to look at one uploaded pdf or document.
- I strongly encourage collaboration.  In the case that you work with others in the class, please include an acknowledgement section in your homework, mentioning people and resources you used in completing the assignment. While utilizing resources such as the internet and the textbook are encouraged, direct copy-paste is not.  You should always be able to explain any of your solutions to me after the fact.
- The late homework policy is:
  - Full credit if submitted on D2L by midnight Wednesday.
  - 5% penalty if submitted by midnight Thursday.
  - 15% penalty if submitted by midnight Friday.
  - No credit after Friday.
  - At the end of the semester, the two lowest homework scores will be dropped.
