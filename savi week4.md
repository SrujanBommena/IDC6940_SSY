# LITERATURE REVIEW 
## ANALYTICS USING MACHINE LEARNING AND BAYES INFERENCE 


### BACKGROUND / MOTIVATION :
#### CONTEXT

Predictive analytics has become one of the cornerstone domains of data science, particularly in applications like business intelligence, finance, and dynamic pricing. Businesses rely on forecasting models in optimizing pricing strategies, product-level inventory control, market movements, and improvement in decision-making processes. Traditional time-series forecasting models, like ARIMA and Holt-Winters, thrive on stationary data, which can sometimes be very tedious for their implementation when working with non-linear, high-dimensional, and complex datasets. The research will narrow this gap by employing machine learning techniques, reinforcement learning, and Bayesian inference in order to enhance predictive accuracy. 

#### PROBLEM OR GAP IN THE EXISTING LITERATURE 

Not only do time-series models provide a starting point for forecasting, but the statistical models for such time-series forecasting have certain drawbacks:

- Assumption of Linearity : There are several models that are linear that establish the relationship between a number of variables. However, these often have very little intricacy to them.

- Limited Handling of Non-Stationarity : Certain data in the world such as financial and sales data have a number of trends and seasonality. Thus, most of those data are usually non-stationary.

- Inability to Capture Uncertainty : Most classical point of statistical does not have a prediction that factors uncertainty.

As is, classical statistical point estimation models are often inadequate for capturing uncertainty. Ensemble methods and deep learning techniques can, however, capture uncertainty robustly. Nonetheless, a coherent approach towards such and model accuracy or interpretability is still not there.


#### SIGNIFICANCE OF RESEARCH QUESTION

The main goal of this study is: How can machine learning, Bayesian inference, and reinforcement learning change the accuracy and reliability of predictive analytics for sales forecasting, financial modeling and pricing optimization? 
This question is relevant because: 

1. Data based decision making is growing rapidly; thus accurate forecasting is vital for business competition.
2. Models are needed that account for uncertainty because financial markets are unstable.
3. Retailers need to adapt to dynamic changes in demand with their pricing policies.
4. A coherent synthesis of several forecasting paradigms is yet to be developed. 

The objective of the research is to design a hybrid framework integrating supervised learning, probabilistic modeling, and reinforcement learning for overcoming these issues.



### METHODS USED
#### METHODS AND USES

The study employs machine learning, Bayesian inference, and reinforcement learning techniques to handle non-linearity, uncertainty, and dynamic decision-making, focusing on their ability to handle non-linearity.
1. SUPERVISED LEARNING FOR TIME-FORECASTING :

The model performs out of sample validation to check its generalization performance. It implements Random Forest, LASSO Regression, and Gradient Boosting models, employing lag features for temporal dependencies alongside one-hot encoding for categorical variables.

2. BAYES INFERENCE:

Bayesian regression models are applied for the estimation of confidence intervals of the predictions, while for forecasting of financial markets and Covid-19 impacts, probabilistic modeling is employed.

![image](https://github.com/user-attachments/assets/dbe00039-4ba9-493f-9ab1-a78ab17fed04)


As the picture shows, the probability is calculated interms as

$$ \[\log(\text{Sales}) \sim \mathcal{N}(\mu_{\text{Sales}}, \sigma^2)\] $$

$$ 
\mu = \alpha + \sum_{i} \beta_i x_i
 $$

![image](https://github.com/user-attachments/assets/0b01afb3-3b93-4878-8306-9d3ffe8e5aaa)

we will also be using mean and covariates for the analysis;

covariate : 

$$ \( z_i = \frac{x_i - \mu_i}{\sigma_i} \) $$

mean : 

$$ \( v_i = \frac{\sigma_i}{\mu_i} \) $$

 
3. SENTIMENT ANALYSIS FOR MARKET PREDICTIONS

Comprising sentiment analysis and keyword frequency time-series models, Twitter data is analyzed in tandem with graph mining techniques to determine salient communities impacting stock market trends.

$$ y_t = \alpha + k \sum_{i=1}^{\beta_j} Y_{t-1} + k \sum_{j} \lambda_j X_{t-j} + \epsilon_t $$

If the p-value is less than 0.05, we could reject the null hypothesis and conclude that variable X (sentiment) influences stock market changes and volatility. Granger's test provides insights into how much predictive information one signal has about another one over a given lagged period. Here the p-value measures the statistical significance of the causality between two variables 

#### example data visualisation for data predicted vs target


![image](https://github.com/user-attachments/assets/bb6eaade-959a-4f66-b7fb-ed55b4116f4d)


#### TECHNIQUES AND APPROACHES

The approaches implemented in predictive analytics help begin to resolve various problems. Supervised learning helps to include historical dependencies in a pattern framework making them effective in the prediction of structured data. Stacking productionizes some of the individual biases and improves prediction performance by combining diverse algorithms. Bayesian inference reflects uncertainty, increasing model’s resilience to variations in distribution of data and unseen scenarios. Reinforcement learning provides adaptive pricing and real-time decision making suitable for automated trading and personalized recommendations. Sentiment analysis draws insights into public perception, augmenting traditional data-driven models. The integrative apply of these methodologies ensures a well-rounded and reflexive density of thought in which a proper equilibrium is created between accuracy, interpretability, and adaptability in vastly complex real-world crowds. 

### SIGNIFICANCE OF THE WORK

#### KEY FINDINGS AND CONTRIBUTIONS

- The study highlights the importance of ensemble learning in improving forecasting accuracy by combining multiple models to reduce variance and bias.
- It introduces Bayesian inference to quantify prediction uncertainty, providing robust probabilistic estimates for financial risk assessment and decision-making under uncertainty.
- Reinforcement learning is applied to dynamic pricing, showcasing AI-driven decision-making that adapts to market conditions and optimizes revenue in real time.
- The study also highlights the potential of social media data in financial forecasting, demonstrating how sentiment analysis and real-time trends can enhance predictive models.
- The study proposes a stacking model framework for flexible and scalable predictive modeling across various industries, ensuring interpretability of machine learning models and evaluating computational efficiency and scalability.

These contributions advance predictive analytics by improving accuracy, reliability, and applicability across multiple domains.

#### IMPLICATIONS AND BROADER CONTEXT

The researchers argue that by integrating estimates of uncertainty into existing procedures for demand forecasting, firms can achieve reduced stock-holding costs and increased enhancements for risk models. A retailer may then adopt such price strategies as may be optimal based on an evaluation of real-time prevailing market conditions. Positive social media sentiment can augment predictions about the stock market. These models can help different governments understand economic trends and predict crises. Such an application could include resource allocation forecasting and risk mitigation within healthcare and supply chain sectors. Their paper highlights the importance of integrating diverse data sources into predictive models to enhance forecasting accuracy. 

### WORK CONNECTIONS

#### PAPAER RELEVANCE AND HOW IT IS DIFFER FROM PREVIOUS WORKS

The study combines different research domains to augment predictive analytics. It combines Breiman's Random Forests and Friedman's Gradient Boosting Machines to improve model efficiency and robustness while responding to complicated datasets. It uses Bayesian regression techniques of Gelman and Kruschke to elicit uncertainty of the prediction intervals to achieve a more systematic thinking. Reinforcement learning techniques are used to learn optimal decision strategies in uncertain environments, such as pricing tactics. Sentiment analysis frameworks from the financial forecasting literature are employed to model the effect of market sentiment on financial forecasting. The study builds on these by extending the applicability of alternative data sources such as satellite imagery, transaction data, and signals from social media. This provides a more integrated and detailed perspective of predictive modeling that informs decisions across varying fields. It shows the flexibility and effectiveness of these methods in forecasting market trends and sentiment shifts. Overall, it is contributing towards the way forward in developmental predictive analytics and decision-making approaches. 

#### NEW CONTRIBUTIONS

This research consolidates a variety of techniques of predictive analytics into an integrated framework complemented by Bayesian inference for ensemble learning, reinforcement learning for dynamic pricing, by integrating social media signals as predictive features, and by investigating hybrid modeling approaches. This offers a practical, flexible solution for various industries: healthcare analytics, climate modeling, and supply forecasting, thereby filling gaps in the existing literature. 


### MY PROJECT RELEVANCE

The capstone project focuses on Machine Learning and Predictive Analytics, aiming to develop models to predict outcomes based on historical data. Techniques include

Capstone project on machine learning and predictive analytics

- Stack methods for improving prediction accuracy;
- Quantify the uncertainty in predictions with Bayesian regression;
- Modify reinforcement learning algorithm for real-time predictive decision-making;
- Run sentiment analysis to improve the model.

Application Areas:
- Financial forecasting: Improvement in prediction accuracy;
- Sales data: Policy based on pricing strategies;
- Healthcare/Supply Chain Analytics: Improvement in forecasting accuracy;
- Macroeconomic indicators: Sharper predictive insights.

Future Work:
- A deep exploration of Transformer-based architecture;
- Explainable AI methods for improving model transparency;
- Causal inference would be included to get insights into relationships between key predictive factors. 

### REFERENCES

1. B. M. Pavlyshenko, “Machine-learning models for sales time series forecasting,” Data,
vol. 4, no. 1, p. 15, 2019.
2. B. M. Pavlyshenko, “Linear, machine learning and probabilistic approaches for time
series analysis,” in 2016 IEEE First International Conference on Data Stream Mining
& Processing (DSMP), pp. 377–381, IEEE, 2016. # https://arxiv.org/pdf/2205.12905

#### NAME : SATHWIKA BAIRI 
