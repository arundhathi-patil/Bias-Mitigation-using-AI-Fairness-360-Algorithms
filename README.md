# Bias-Mitigation-using-AI-Fairness-360-Algorithms
Mitigating Bias in the data using AI Fairness 360 state-of-the-art bias mitigating algorithms 


Machine learning and AI is being used more and more nowadays in processes or scenarios which involve high stake decisions about people. 
Some of the examples are :
1. Credit decisions about Loans
2. Court decisions on cases - Ex: COMPAS Algorithm 
3. Gender Classification based on Face images
4. University admissions decisions
The Machine learning models built to make decisions like these have to be accurate and clear of any systematic bias. 
Although machine learning, by its very nature, is always a form of statistical discrimination, the discrimination becomes objectionable
when it places certain privileged groups at systematic advantage and certain unprivileged groups at systematic disadvantage. Biases in 
training data, due to either prejudice in labels or under-/over-sampling, yields models with unwanted bias.

The AI Fairness 360 is a Python package that includes a comprehensive set of metrics for datasets and models to test for biases, 
explanations for these metrics, and algorithms to mitigate bias in datasets and models. Bias mitigation algorithms attempt to improve the
fairness metrics by modifying the training data, the learning algorithm, or the predictions. These algorithm can be classified to three
categories: pre-processing, in-processing, and post-processing. 

COMPAS (Correctional Offender Management Profiling for Alternative Sanctions) is a popular commercial algorithm used by judges and
parole officers for scoring criminal defendant’s likelihood of reoffending (recidivism).It has been shown that the algorithm is biased 
in favor of white defendants, and against black inmates, based on a 2 year follow up study(i.e who actually committed crimes or violent 
crimes after 2 years).In this project I have used the Compas Dataset. This Dataset contains variables used by the COMPAS algorithm in 
scoring defendants,along with their outcomes within 2 years of the decision, for over 10,000 criminal defendants in Broward County, Florida.
I have used the pre-processing algorithm "Disparate Impact Remover" from AI Fairness 360 to remove the bias from the dataset and then applied
Machine learning algorithm to predict the risk of recidivism(which is the decile score variable) and see if there is any improvement with
the prediction being nearer to the ground truth.
