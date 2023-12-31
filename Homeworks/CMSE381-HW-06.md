# Homework 6

## CMSE 381 - Fall 2023

## Due Weds, Nov 8, 2023

### Instructions

This homework covers five classes.

- Fri 10/27, we covered 6.3 PCA/PCR
- Mon 10/30, we covered 6.3-6.4 PLS, High dimensions
- Wed 11/1, we covered 7.1 polynomial and step functions
- Fri 11/3, we covered 7.2-7.3 Step functions, basis functions and also started splines (7.4)
- Mon 11/6, we finished splines (7.4)

Problems listed below are from [the textbook](https://www.statlearning.com/).

- 6.6.9 (e,f,g)
- 7.9.3
- 7.9.6 (a,b). Modified version of part (a) (that is, don't do the part about hypothesis testing and ANOVA):
  - (a) Perform polynomial regression to predict wage using age. Use cross-validation to select the optimal degree $d$ for the polynomial. What degree was chosen, ~~and how does this compare to the results of hypothesis testing using ANOVA~~? Make a plot of the resulting polynomial fit to the data.
  - Additional part (call it c): Fit a cubic spline to predict `wage` using `age`. How does this function compare to the polynomial (particularly, the degree $d=3$ polynomial) found in part (a)?
- *Added question 4*
  - Part A. I am learning a step function of some data, and I'm using knots $c_1 = 3$ and $c_2 = 7$.
    - (i) Write equations for each of the basis functions $C_0(X)$, $C_1(X)$, and $C_2(X)$. Sketch the three functions.
    - (ii) If the model learned was

```math
f(X) = \beta_0 + \beta_1C_1(X) + \beta_2C_2(X)
```

with $\beta_0 = 2$, $\beta_1 = 3$, and $\beta_2 = -1$, sketch the graph learned.

- Part B.
  - I am learning a cubic spline of some data with a single knot at $z_1 = 4$. As noted in class and in Sec 7.4.3, we have a basis for learning cubic spline data. *(As a side note, my lectures have knots as $`z_1,\cdots,z_K`$ and the book uses $`\xi_1, \cdots, \xi_K`$ but you should treat them as the same thing.)* I'm going to build a cubic spline with basis functions
    - $b_1(X) = X$  
    - $b_2(X) = X^2$  
    - $b_3(X) = X^3$  
    - $`b_4(X) =h(x,4)= \begin{cases} (x-4)^3 & x >4 \\ 0 & \text{else} \end{cases}`$  
  - Assume the learned model was $`f(X) = 3 + b_1(X) - 2 b_2(X) + 3 b_3(X) - 4b_4(X)`$
  - (i) Write the equation for the piecewise polynomial that this function represents. Draw a graph of the function.
  - (ii) What are the requirements for a piecewise polynomial function to be a cubic spline?
  - (iii) Check that your piecewise polynomial from (i) fits these requirements.

### Submit homework to Crowdmark

You will upload your homework to the Crowdmark website. The main changes are:

- You will be emailed a link to the assessment and will upload your solutions to that page. [Here is a link to the Crowdmark help page with information on submitting the homework.](https://crowdmark.com/help/completing-and-submitting-an-assessment/)
- Answers to each question will need to be uploaded separately.  So this will basically require taking portions of the PDF you were generating before and separating them when uploading.  
- Feedback on the homework will be posted via the Crowdmark website
- Your overall grades will still be visible on D2L when they are posted.

### Important Reminders

- Homeworks must be typed. Some options for this include word, overleaf/latex, or by including a PDF of a Jupyter notebook (not the `.ipynb` file please!). Some students have had more success in the Jupyter case of printing from the browser window.  The "convert to PDF" option requires you to have latex installed.
- Including figures when explaining your reasoning is highly encouraged.  This can be done as easily as taking a picture of a hand-drawn sketch and including it in your file. Please be sure to include all figures in the main file so that we only have to look at one uploaded PDF or document.
- I strongly encourage collaboration.  In the case that you work with others in the class, please include an acknowledgement section in your homework, mentioning people and resources you used in completing the assignment. While utilizing resources such as the internet and the textbook are encouraged, direct copy-paste is not.  You should always be able to explain any of your solutions to me after the fact.
- The late homework policy is:
  - Full credit if submitted on D2L by midnight Wednesday.
  - 5% penalty if submitted by midnight Thursday.
  - 15% penalty if submitted by midnight Friday.
  - No credit after Wednesday.
  - At the end of the semester, the two lowest homework scores will be dropped.
