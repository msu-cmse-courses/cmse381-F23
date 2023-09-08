# Homework 2

## CMSE 381 - Fall 2023

## Due Monday, Sept 11, 2023

### Instructions

<span style="color:violet">Note that the problems in the text often specifically talk about the `statsmodels` package. Most of my examples in class do the same thing but with the `sklearn` package. Throughout the course, if a problem asks you to do something, you can always answer by using either package.</span>

This homework covers three classes. Problems listed below are from [the textbook](https://www.statlearning.com/).

- Fri 9/1, we covered Ch 2.2.1 - 2.2.2
  - 2.4.3 (*Note we have only done irreduceable error, not Bayes error since that has to do with classification*)
  - 2.4.8
    - Note that there is a typo in 2.4.8f, at least with respect to the verson of the data set we have. The information in the `Top10perc` column is a percentage 0-100 rather than a value between 0 and 1. So use the following replacement code instead.

    ```python
    college['Elite'] = pd.cut(college['Top10perc'],
    [0,50,100],
    labels=['No', 'Yes'])
    ```

- Wed 9/6 and Fri 9/8, we covered Sec 3.1 - Simple linear Regression
  - 3.7.8 (a) and (b)
    - Note: 3.7.8 (a).iv: we haven't talked about prediction intervals, just do the confidence interval for the coefficients for the horsepower regression ($\beta_0$ and $\beta_1$).
    - A note on code. The book's use of the `statsmodels` package is slightly different than the examples provided in the jupyter notebooks in class. In particular, in the book's lab examples and in the homework statement they implicitly use
  
      ```python
      import statsmodels.api as sm
      ```

      while we use

      ```python
      import statsmodels.formula.api as smf
      ```

      This results in slight diferences in code, in particular whether the funciton call you use is `OLS` or `ols`. You may use whichever works for you, the answers should be the same.

- Fri 9/8, we covered Sec 3.2 - Multiple Linear Regression
  - 3.7.1

*Note: the content from Mon 9/11, will be included on HW3 due next week.*

### Crowdmark info

- You will be emailed a link to the assessment and will upload your solutions to that page. [Here is a link to the Crowdmark help page with information on submitting the homework.](https://crowdmark.com/help/completing-and-submitting-an-assessment/)
- Answers to each question will need to be uploaded separately.  So this will basically require taking portions of the pdf you were generating before and separating them when uploading.  
- Feedback on the homework will be posted via the Crowdmark website.
- Your overall grades will still be visible on D2L when they are posted.

### Important Reminders

- Homeworks must be typed. Some options for this include word, overleaf/latex, or by including a pdf of a jupyter notebook (not the .ipynb file please!). Some students have had more success in the jupyter case of printing from the browser window.  The "convert to pdf" option requires you to have latex installed.
- Including figures when explaining your reasoning is highly encouraged.  This can be done as easily as taking a picture of a hand-drawn sketch and including it in your file. Please be sure to include all figures in the main file so we only have to look at one uploaded pdf or document.
- I strongly encourage collaboration.  In the case that you work with others in the class, please include an acknowledgement section in your homework, mentioning people and resources you used in completing the assignment. While utilizing resources such as the internet and the textbook are encouraged, direct copy-paste is not.  You should always be able to explain any of your solutions to me after the fact.
- The late homework policy is:
  - Full credit if submitted on D2L by midnight Monday.
  - 5% penalty if submitted by midnight Tuesday.
  - 15% penalty if submitted by midnight Wednesday.
  - No credit after Wednesday.
  - At the end of the semester, the two lowest homework scores will be dropped.
