## Portfolio management

### Business Overview
- Create a CLTV scoring algorithm for measuring health of a portfolio
- Maximise customer value and deliver profitability
- Understand clinical progression of health risk

### CLTV

Scoring formula is

![CLTV scoring](https://c1.staticflickr.com/5/4350/36262342373_81f5ba6982_c.jpg)

- **Written premium** is the amount a consumer pays for health insurance
- **Claim risk** is the amount the company has to pay for the claim if a member claims. Build two models for _frequency_ and _severity_ to predict claim cost. _Frequency_ is total number of claims made by a person in a year, _severity_ is the average cost per claim. _Claim cost_ is _Frequency_ * _Severity_. Predictions are made for the 10 years using acturial assumptions
- For frequency model we used Generalized linear models (Logistic regression) and severity model we used Generalized linear models with Gamma distribution
- **Retention probability** is the probability to continue the policy next year. We used Logistic regression

### Segmentation based on CLTV scoring

![CLTV segmentation](https://c1.staticflickr.com/5/4399/36887937456_07e253f3c7.jpg)


Categorized the entire portfolio into 4 groups and developed strategies based on these categorizations.

### Clinical progression
To understand clinical progression, we have used JHMC ACG system to calculate predicted claim costs for chronically ill patients. What is the patient's most likely disease and how much is it going to cost the insurance company?

You can use the [editor on GitHub](https://github.com/sivakon/hinsurance/edit/master/README.md) to maintain and preview the content for your website in Markdown files
