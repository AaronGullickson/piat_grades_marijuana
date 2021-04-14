# Data Source Description

For this project, we will use data extracted from the [National Longitudinal Survey of Youth 1997](https://www.bls.gov/nls/nlsy97.htm) (NLSY97). The NLSY97 is a nationall representative sample of Americans who were first surveyed as adolescents in 1997. The NLSY97 has done a follow-up survey of these respondents each year, which is why it is "longitudinal." The survey is conducted by the US Bureau of Labor Statistics. 

We are going to use data the NLSY97 collected on the college transcripts of these respondents that allows us to calculate their college GPA. Because our sample is restricted to only those respondents who completed  and provided transcripts, it is smaller than the full NLSY97 sample. We are also only working with a small extract of the full number of variables available in the NLSY97.

From the full data, I have extracted and recoded the following variables for our use as an analytical dataset. To load this dataset in R, you just need to run the setup code chunk in the full_report.Rmd R Markdown document. The name of the dataset in R is `NAME`. 

* **gpa_college**: The overall cumulative GPA of the respondents in undergraduate courses (including those taken towards an associate's degree). This is the key dependent variable.
* **marijuana_use**: In each wave, the respondent was asked how many days out of the previous 30 days that they had smoked marijuana. I take the average response to this question from the period when the respondent was 18-23. This is the key independent variable.
* **gender**: The gender of the respondent, recorded as male or female. This is the key contextual variable.
* **hh_income**: The household income of the respondent's household in 1997 (when they were an adolescent). This is measured in 1000s of dollars. 
* **highest_parent_grade**: The highest years of education among the respondent's residential parents (which could include step-parents) and biological parents. 
