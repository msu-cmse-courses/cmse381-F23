# CMSE381 - Honors Project Addendum

If you are taking CMSE381 for honors credit, you will also complete a project, but you have additional requirements.

## Getting Honors Option Set Up

Please note that prior to doing the honors version, you need to discuss and get approval from Dr. Munch. If you already have approval, you have access to the [#cmse381-f23-honors](https://cmse-courses.slack.com/archives/C05T4D8HJ2Z) channel for additional notes and announcements.

In addition, there are university paperwork requirements for getting this set up, as well as deadlines for that to happen. I will update this section when I have additional information.

## Project requirements

In place of the [CMSE381 project](ProjectDescription.md), you will complete a project which is similar, but with additional requirements. Here, I will include notes on what modifications you will submit from the [standard project](ProjectDescription.md).

- You will get a data set that is *not* from the UCI ML repository. Appropriate data sets will be generally larger in scope, more messy requiring more data cleaning.
- You will still do a regression task and a classification task. Depending on the data set chosen, this might be the same data set (unlike in the standard project, although you might still choose to use two data sets), however the tasks must be differentiated enough in the case that you use the same data set. For example, it would not be enough to do a regression on some output $Y$, and then also do classification by testing whether $Y<0$ or $Y>0$. However, if you are doing two data sets, I'd like to see them be generally in the same theme (bio, social science, etc) so that your project has overall unity.
- For each regression/classification task, you must use at least *two* different models for the task. All four of these models must include discussions of general improvements and parameter selection such as k-fold CV or subset selection.
- For each pair of models, you must also include a discussion of which one is better (e.g. with respect to the testing score, and/or with respect to running time).
- Your analysis should include an in depth discussion of interpretation of results, limitations of your work, as well as what you might do in the case of a followup project. This is the kind of thing that would go in the discussion section of a published research paper.
- Overall, I am looking for your submitted notebook to be as similar in style to a research paper as possible. It should have an introduction with broader context of the data. It should be clearly annotated and discussed for me to understand what you are doing.
