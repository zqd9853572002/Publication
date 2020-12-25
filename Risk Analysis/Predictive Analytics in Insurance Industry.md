Predictive Analytics in Insurance Industry

# ABSTRACT

The insurance industry is a typical data-based industry. Under the stakeholder pressure and competitive pressure, many insurance companies have begun to explore the application of big data in the industry and hoping to achieve the major goals, which mainly focus on earning profit and meeting customer needs. The insurance industry would like to leverage the information and the big data analytics advantage into actionable insights, and then improve the operations and performance.

Decided by the business nature, the insurance industry's performance heavily depends on the accurate and timely forecast and prediction of exposure and risk-return. To make the prediction more accurate, many insurance companies have adopted predictive analytics techniques.

Predictive analytics is the technology to collect multi-sources data and to analyze data, help people to better understand and predict behavior, and extract meaningful insights and actionable information. It includes a variety of statistical techniques from data mining, predictive modeling, and machine learning. Predictive analytics investigates and analyzes the current and historical fact and pattern, and then create risk assessment models to predict the future events possible outcomes or determine the metrics development patterns.

In past years, insurance companies had collected tremendous data from different sources, such as telematics, app data, customers call and social media, and gradually used predictive analytics in daily business.

In this article, we will focus on the predictive analytics' underlying technologies and models, the business application in the insurance industry's different aspects, especially in the fields of marketing and sales, product development, underwriting, claim management, and customer service (these fields constitute the core business of the insurance industry). We will also talk about potential problems in using practicing predictive analytics.

# INTRODUCTION OF PREDICTIVE ANALYTICS

In every kind of business, we need to understand the past and current events, then we could make better business decisions. Based on the Gartner Analytic Ascendancy model, there are four different types of analytics.

![](https://miro.medium.com/max/690/0*HJfq8tD2kIbqZFF2)

Descriptive analytics and diagnostic analytics are the methodologies to look back they mainly solve the problem of letting people know what happened and why happened. The hindsight and insights obtained from descriptive analytics and diagnostic analytics provide the basics of looking forward. Instead of looking back the history, predictive analytics lets us know what is likely to happen in the future, it helps us complete the prediction process, during its development, it also defines the related decision-making process and creates the foundation of prescriptive analytics. The prescriptive analytics could tell us how we decide or perform in the current situation to achieve goals.

## Predictive Model

The core of predictive analytics is the predictive model. To simply put, the predictive model is a complex mathematical function that maps the relationships between the input variables and the response variables.

The predictive model could be supervised learning or unsupervised learning.

In supervised learning, the training data (including the input data and the desired/ defined output) was &quot;feed&quot; to the model to let the model map the function or relationship. This kind of training will continually be performed until the model finds the mapping relationship. The predictive model related supervised learning method includes neural networks, support vector machines (SVM), and decision trees.

In unsupervised learning, we only &quot;feed&quot; input data into the model, and the model will figure out how the input data are related to each other. In predictive analytics, the most used algorithm is clustering.

## The Different Type of Predictive Models

Based on the specific application function, predictive models could be categorized into different types.

### Classification Model

The main function of the classification model is to categorize data based on historical data, i.e. it solves the problem of what category something falls into. Because the different classifications are determined in advance, the classification model is a kind of supervised learning technique.

Once the classification model is built, as the new data become available, the model could be re-trained and adjust to reflect the new pattern, and then provide broader analysis and better answer questions. Based on this character, the classification model could be used in different industries, in the insurance industry, the classification model could be used in:

- sales and marking prediction, such as determining whether the specific customer will continue to subscribe to the product or service;
- supporting underwriting decision, such as determining whether specific customer belongs to the high-risk group, the answer of this question could provide information for an underwriter that whether the company should underwrite the business, or in what conditions to underwrite the business;
- supporting claim anti-fraud, such as determining whether a claim case belongs to a fraud claim.

### Clustering Model

The clustering model is to sort the records into separate groups based on similar attributes. The clusters in the clustering model are unknown in advance, this is the main difference between the clustering model and the classification model. Also, this characteristic makes the clustering model an unsupervised learning technique.

In the clustering model, each cluster could be viewed as a hidden pattern in the data set, the algorithm needs to mark the cluster by itself. Therefore, even the data set is the same, different clustering models and different selected parameters each time could all result in different conclusions.

In the insurance industry, the clustering model could be used in:

- Market segmentation. For example, to implement a marketing campaign, the insurance company could group the customers based on their common characteristics and design different strategies for different clusters;
- Supporting niche-market product development. For example, the insurance company could find the common characteristics of different groups of business and then develop tailored insurance products or services for groups;
- Supporting claim anti-fraud. By revealing the hidden pattern of different claims, the company could use a clustering model to identify the connection of potential fraud ring.

### Forecast Model

The forecast model mainly deals with in metric value prediction, which could estimate numeric value for new data based on the learned mapping relationship from historical data. One of the characteristics of the forecast model is that it can deal with multiple related parameters.

Based on the characteristics, the forecast model could be used in:

- insurance sales prediction, such as predicting the potential sales revenue in the next three months;
- distributing the workforce of the customer service department, such as predicting how many calls will be receive per hour in the call center;
- forecasting risk and return, such as predicting the underwriting profit and investment return in coming years.

### Time Series Model

In the time series model, time is a key input data in prediction. The time series model uses previous periods of' data to develop numerical metrics to predict future trends.

In the insurance industry, the time series model could be used in:

- Making underwriting decisions and suggesting health management plans. In health insurance, through predicting the customer's potential disease occurrence frequency in the next 1-3 years, the underwriter could make a tailored underwriting plan, and the health management department could develop a specific health plan for the customer;
- Supporting marketing and budget planning, such as predicting the product sales volume based on different periods in a year and other attributes, and then could distribute sales force and promotion budgets.

### Outliers Model

The outlier model deals with the outlier or anomalous data in the dataset. An outlier is the data or record that depart from the usual data range. The outlier model is useful in fraud detection.

In the insurance industry, the fraud claim's pattern usually deviates from the normal, the outlier model could predict or alert the fraud case before it occurs. For example, in identifying a potential fraud claim, the outlier model could assess the claim amount, accident address, case reporting time, and claimant previous activities, then give the result of whether the claim belongs to a potential fraud claim.

## Predictive Model Validation

After building a predictive model, but before putting it into the production environment, we need to validate the model's effectiveness and efficiency, which means we need to measure that whether the model works and how accurate the model is.

Based on different model types, different performance measurements or metrics will be used to measure the model's effectiveness and efficiency. For example, we could use classification accuracy, confusion matrix, precision and recall, F1 score, ROC, and AUC to evaluate the classification model; we could use R-squared, Mean Absolute Error, Median Absolute Error, Mean Squared Error, and Mean Absolute Percentage Error to measure the performance of time series model.

## The Process of Creating Predictive Models

When developing a predictive model, we could break down the model creating process into parts below.

### Define Scope and Scale

The predictive model is a way used to solve questions, so we need to determine the desired business outcome or the question we need to answer, and then determine the process of how to use the predictive models.

### Prepare Data

Predictive models are based on data in nature, so they are extremely data intensive. Therefore, enough well-prepared data could train the model better, and then could result in a better model result.

#### Data Profile

The organization needs to decide where the data is (where data comes and where data stored), the data's current status, and data accessibility.

Also, the organization needs to have enough data to build the model. Without enough data, the predictive model could not be trained or be tested well, and the worse case is the model overfitting, which means the model cannot be generalized, which will affect the model's usefulness eventually.

#### Data Gathering, Cleaning, and Integration

After finding the available data, the data need to be cleaned and gathered. This is an important step and may consume lots of time. This step worth putting in the efforts, because predictive models do need a strong foundation to get effective and efficient work.

### Develop a Predictive Model

According to the business situation, predictive models run different algorithms on the selected data set to obtain the prediction. This process is repetitive because it involves model training and testing. Sometimes, we may have to run multiple predictive models on the same data set.

We also validate the model's effectiveness and efficiency in this step in determining the most suitable model.

### Put Predictive Model into The Business Process

In this step, we put the selected predictive model into the business process, and in this way, the model could help the organization to obtain the best results.

### Monitor Performance, Measure Result and Make Adjustment

After the model deployment, the model needs to be measured to see if it makes genuine contributions to the business. Also, we need to measure the model result in the production environment and adjust or tune fine the model to reflect the changing business operation.

# THE PRACTICE OF PREDICTIVE ANALYTICS IN INSURANCE CORE BUSINESS

Many insurance companies have begun to explore the application of big data and leveraged the predictive analytics advantage into actionable insights, and then improve the operations and performance.

The performance of the insurance industry is heavily based on the accurate and timely forecast and prediction of exposure and risk-return.

Predictive analytics can collect data from different sources, including internal sources and external sources - to better understand the business, predict insureds' behaviors. Property and casualty insurance companies are collecting data from automobile telematics, customer interactions, smart homes (Homeowner IoT), and social media, life insurance companies are collecting data from the wristband, cellphone GPS information, hospital visiting or medical records to gain information to make decisions and then to support different functions of insurance companies.

In the below part, we will illustrate some business applications of predictive analytics in the insurance field of marketing and sales, product development, underwriting, claim management, and customer service.

## Marketing and Sales

Predictive analytics can help the insurance company to identify and target potential markets, which could provide the best opportunities for future business growth and profitability.

To achieve this goal, insurance companies need to collect data beyond the insurance system, for example, insurance companies can derive data from data brokers, partners, and social media. All these data might be relevant to the market segmentation. Through an in-depth analysis of customer information, insurance companies could acquire an understanding of customers' needs, which allows insurers to identify potential customers, recommend appropriate products, and implement precision marketing. All of these will differentiate itself from competitors.

### Customer Behavior Prediction

Predictive marketing could let insurance companies could make intelligent and forward-looking decisions. Customer behavior prediction could identify the behaviors among different groups of customers, and then create models to predict how similar customers will behave under similar circumstances.

Customer behavior prediction models are based on the data mining of customer data. If models are correct and effective, and the market follows the assumptions in modeling making, most customers in the group will make the reaction as models' prediction.

Three predictive models could be used in predicting customer behavior.

#### Clustering Model

Clustering models are mainly used for customer segmentation. The model will segment target customer groups based on the collected variable.

To implement unique marketing campaigns for different customer groups, the insurance company could group the customers based on shared characteristics, and then design and develop a different advertising strategy for each cluster.

#### Propensity Model

Propensity models are used to predict customer purchasing behavior.

In the life insurance field, each insurer losses money every year due to the customer stop &quot;subscribing&quot; the insurance (i.e. not continue to pay the annual life insurance premium and loss protection). Although some customers just forgot to pay the premium (solving this problem is easy), some customers' &quot;stop subscription&quot; are caused by other reasons, such as not satisfied with the current product or service or converting to other companies' products. For the latter situation, the insurance company could use the propensity model to identify customers who are likely to cancel or lower coverage, and then provide personalized customer service and alleviate potential issues, such as letting agent, broker, or call center to reach customers, to know customers' thoughts and intervention the potential &quot;non-subscription&quot; behavior. Without predictive analytics, insurance companies may miss these warning signs and lose business.

#### Collaborative Filtering and Association Rule

Collaborative filtering and association rule are used for recommending insurance products, services, or making advertisements to the customer based on past buying behavior.

Collaborative filtering answers the question of &quot;What are the items that users with interests similar to yours like?&quot; The answer to the question is the product or service bought by other users with similar interests.

Another method of recommendation is the association rule, it answers the question of &quot;What are the items that frequently appear together?&quot;. Association rules recommend the products that the customer will likely to buy based on the customer's shopping history, so it is a recommendation algorithm based on the independent personal profile (this is also a key difference between association rule and collaborative filtering technique). In an online insurance platform, when a customer buys homeowner insurance (HO coverage) and automobile insurance (PAP coverage) together, the insurance company may use association rule learning to recommend him/ her an umbrella policy (a kind of extra protection policy above currently selected policies).

### Identify and Prioritize Potential Customers

In the short-term business insurance field, identifying and prioritizing potential customers is more important than predicting customer behavior.

Predictive scoring, identification model, and segmentation can be used to qualify and prioritize leads. With the identified priority, insurance companies could arrange sales staff better in obtaining priority customers.

### Target Right Customers at Right Time with Right Content

The predictive analytics results could also tell the marketing department when and how to approach the customer, and what the advertisement content would be. This is the direct way to optimize the marketing effort and may get a better ROI. This also provides ideas and insights on how to deliver insurance products and related information to potential customers.

For example, the predictive analytics result could tell the insurance company whether to send the ad email or print brochures and send them to the mailbox of potential customers or combine these two ways.

When deciding the advertisement content, the marketing department should not attract different customer groups by using the same advertisement or applying the same marketing technique, they can customize the advertisement based on customer segments. Categorization of behavioral and intent data can let insurance companies understand how much a specific user group is interested in certain products, then they could select the best suitable marketing method. Insurance companies can also avoid disturbing irrelevant customers by not sending a mass advertisement to the whole group.

For example, the insurance company could promote health insurance to those customers who spend more than 5 hours a day on internet surfing; critical illness insurance might be promoted to meat lover and wine drinker; the broken screen protection product should be recommended to the large screen cellphone users and; travel insurance and emergency assistance service should be recommended to the potential customer who browses the online travel agency or airline website or online air ticket purchase website frequently. WeChat, an equivalent of WhatsApp or Telegram, is the most populated app in China. On the WeChat insurance shopping page, the app could deliver customized insurance products and services advertisements based on the detailed user portrait.

In the auto insurance field, considering the popularity of UBI (Usage-Based-Insurance), some insurance companies require the car owner to install a module or device on the car to record the car usage. Some insurance companies considering using the data of the GPS module on the car to predict the user portrait, and then deliver the advertisement accordingly. A simple example is that, GPS record shows the car stops 1-3 minutes at a local primary school every morning during the workday, the simple conclusion is the car owner is most likely has a child whose age is between 6 - 13. With this information, the insurance company could recommend accident insurance, life insurance, or college tuition saving plan to the car owner.

## Product Development

When developing new insurance products, insurance companies typically innovate new products or modify existing products based on market demand, which could enhance their competitiveness.

### Personalized Product Development

Once insurance companies have a clear understanding of what the customers want, the companies can estimate the potential losses based on relevant data (internal or external) and existing data about risks associated with the insurance coverage. Then the companies could develop personalized products to meet different actual needs of different customer groups.

PICC, the largest P&amp;C insurance company in China, initiated the customized bundled travel insurance products in 2018. On an online travel agency website, after the customer chooses the travel product, such as air tickets and hotel booking, the system will generate/ recommend a customized bundled travel insurance product (both in benefit level and insurance amount level) based on the selected travel duration, destination, potential travel activities, and other criteria. Customers could choose whether to bundle the insurance into the travel package, or they could also change the insurance plan by themselves.

in 2013, Alibaba, Tencent, and PingAn Group initiated ZhongAn P&amp;C Insurance, the first fully internet-based insurance company in China. The most famous insurance product ZhongAn developed is the insurance that covers the shipping cost due to online shopping returns. In the traditional product development method, the price of the insurance is settled by the actuary in advance, the underwriter could make some changes to the final price or underwriting condition based on their experience or judgment. However, in the fast online transaction business, this kind of method cannot reflect the changing condition of the risk in the market, so the price adjustment is lag to the business trend, also the underwriting price and condition cannot reflect the small difference of each business. To make the shopping cost insurance more customized to each business and reflect the real-time risk (instead of overall risk), ZhongAn accessed the customer portrait data from Alipay (similar to Google Pay or Apple Pay, but not only limited to payment function, it also covers its credit scoring, small amount loan service, and other daily life services), the customer purchasing, browsing history and seller and commodity review data from Taobao (an online shopping website similar as eBay originally), then predict the likelihood that whether the buyer will return the commodity and the average shipping cost (based on real-time shipping cost prediction in the local and national area). These data are all used to calculate the customized price of the shipping cost insurance. As a very cheap price insurance product (average price is 0.1 CAD dollars/ transaction) the shipping cost insurance generated 0.6 billion CAD dollars total revenue to ZhongAn from 2014 to 2016. As the predictive model development, the company also obtain tremendous profit from this single product.

In the traditional health insurance field, insurance companies relied on the general medical data to provide critical illness or medical expense coverage for those people who have pre-existing conditions, which means these people could purchase regular insurance plans just as a normal person (some restrictions or the additional premium may apply). However, this kind of method may not reflect the specific need of the pre-existing condition group, the extended insured group's higher risk might also impact the profitability of the original group without pre-existing conditions.

To solve these potential problems, some insurance companies are developing specific standalone insurance products for people with chronic diseases, such as diabetes, cardiovascular, or other pre-existing conditions. For example, in the last five years, several China insurance companies, including but not limited to China Taiping, Taikang, PingAn, and ZhongAn, introduced critical illness and complications insurance only for those who have already been diagnosed with diabetes. The covered critical illness and complication types in the insurance are different from the insurance for normal people, it covers the specific and high possibility disease for diabetes patients, such as amputation and blindness caused by diabetes. Because chronic diseases and pre-existing conditions are generally not fatal in a short time, insurance companies also introduced customized health management plans into insurance products and changed the fixed pricing structure and traditional underwriting method. In this process, the application of predictive analytics makes changing pricing and underwriting methods possible.

### Pricing

Insurance is the science of risk management, and the law of large numbers is the foundation and of traditional actuarial theory. It consists of the foundation in ensuring the adequacy and impartiality in the determination of the pure risk loss ratio. It also governs the basic operation, management, and pricing basic theory of the industry.

With more data, predictive analytics could let the insurance companies optimize the pricing model and get the &quot;right&quot; price, set the floating insurance rate (dynamic pricing) and differentiated pricing structure.

The background logic of applying predictive analytics to insurance pricing is simple. Considering the risk profile of each risk unit is changing with time, the risk shared by the insurance companies is changed, so the risk pricing and underwriting condition should also reflect the change. Because data's volume, velocity, variety, and veracity are growing, data-based technologies (such as predictive analytics) can reveal the in-depth insights of continually changing risks and coverage needs of particular groups (or a specific segment within the particular group), which empowers insurance companies to dynamic pricing (or called granular pricing) to price risk more accurately, and then reflect the actual risk the companies undertake.

The dynamic pricing and the changing product structure change some basis of traditional insurance.

Taking health insurance as an example, traditional health insurance product cannot or seldom track the insured's health or disease development after insured buying, in other words, when accepting or rejecting insurance application, the insurance companies just &quot;play the gambling&quot; based on its experience (although it did base on lots of analytics with history data). This also means the premium, payment amount, and underwriting condition are all determined at the time of making an underwriting decision, so it cannot reflect the changing risk of a particular insured.

In dynamic pricing, the insurance companies use smart products, such as wearable and wristwatches, to track the insured health condition and make risk alert in advance, also the insurance companies could use the data to recommend health management plans, adjust premium or payment condition. In 2019, PICC Financial Service (an insure-tech focused subsidiary of PICC) initiated an internal project, the project is to develop an insurance product for hypertension patients. Besides only faces pre-existing condition patients, the product plans to use the wristband to track the daily blood pressure of the insured and give the prediction of blood pressure in the next 5 - 10 days, and recommend the food, medical, or treatment plans accordingly. The plan also combines the daily activity tracking service, which will oversee the insured's medicine taking history and sports history. If the patient follows the suggested health management steps, the insurance premium and the insurance payment amount will remain at a normal level, or the premium for future health insurance get reduced as an &quot;awarding&quot;; If the patient doesn't follow the steps, the insurance payment amount might get reduced or the insurance payment conditions also get restricted as a &quot;punishment&quot; of not following. The combination of insurance and risk management method let the insurance company oversee the insured circumstance in real-time and adjust the risk burden accordingly, also the combination helps the insured control the health risk. Moreover, PICC Financial Service also uses historical medical data (not limited to the specific insured's data) to predict the disease's different development stages. To predict hypertension's frequency and severity, besides using the regular millimeters of mercury to identify the hypertension level, this plan also use the other disease symptoms, diagnostics, and medication histories, such as trichiasis (an abnormally positioned eyelashes that grow back toward the eye, sometimes may touching the cornea or conjunctiva) and the frequency of ankle bone fracture, to predict the development of hypertension.

Another example of dynamic pricing is inland marine insurance (inland transportation insurance). Some transportation companies' main business is shipping grain between seaports and inland cities or between different provinces. The grain is a special cargo that is extremely sensitive to humidity and water, especially in long-distance transportation, because a small amount of water could make the grain sprout, and then ruin the large portion of grain in the container. To avoid the raining, snowing or possible high humidity circumstance's influence to the grain in transportation, PICC Financial Service and a weather forecast company develop the dynamic pricing model, in which the weather forecast company provides future 2-3 days accurate weather information of each town in 15 minutes level, generates the risk level map (similar as a heat map) and recommends transportation route to the driver to avoid possible weather problem. The insurance company uses the actual transportation route to adjust the premium accordingly.

## Underwriting

In the insurance operation field, underwriting needs to achieve a fine balance between art and science, which need to require insights from historical trends and individual case assessment. Predictive analytics bring the insurance companies smarter and quicker decisions, further efficiency and process enhancement, decreased risk, and better customer experience.

In the underwriting process, predictive analytics models create opportunities for data-driven decisions. For example, predictive models can be used to:

- Develop better underwriting rules that meets business trend;
- Re-pricing for certain risks and help new business expansion;
- Develop a basis of rating segmentation, discounts, surcharges for special programs;
- Evaluate and monitor specific business line's underwriting performance;
- Prioritize insurance application based on the deal's particular risk characteristics; and
- Discover or identify additional or hidden variables in making underwriting decisions.

In underwriting, the use of predictive analytics does not reduce the required qualification elements or eliminate any underwriting process component, but it increases the efficiency of reviewing these elements. Besides simply automating the qualification documents reviewing process, predictive analytics' goal is to maximize the process efficiency and accuracy, while allowing companies to review the risk smarter.

There are two obvious benefits of predictive analytics: improving process automation and providing cognitive insights.

### Process Automation

Process automation allows the system to handle the process where humans are not needed. Insurance companies could obtain information from different sources and transform the information into digital data and run the classification model with a set of rules designed to test acceptability. The underwriter is then presented only with the decision, credibility score, anomalies, or discrepancies that need to be addressed.

In late 2018, Yitu Technology, a Chinese AI start-up, introduced a cancer screening tool and imaging system for chest CT scans, which was featuring real-time imaging of lungs for detection of nodules and other lesions (including cystic, strip, and patchy shadows). These tools are designed as a &quot;clinical assistant&quot; to reduce the workload of doctors and improve the diagnostic capabilities of radiologists. Yitu Healthcare also cooperated with multiple departments of West China Hospital, such as Information Center, Radiology, Pathology, Respiratory Medicine, etc., integrated HIS, LIC, PACS and RIS systems, and created the AI scientific research database of lung cancer, which includes multi-dimensional clinical indicators covering clinical text data, imaging, and pathological data. As a further application of the technology, some health insurance companies are approaching Yitu to develop an automated underwriting model based on the result of CT scans, which means after the network built and databases connected, insurance applicant doesn't need to submit the medical report or medical-related questionnaire to the insurance company, instead, the insurance company can automatically access to the detailed medical records from hospitals or clinics to assess applicant's lung cancer risk, develop the underwriting conditions and make the underwriting decisions accordingly (but some special case still need underwriter involved). This method could reduce the underwriting process and time dramatically and save the process of file submission and reviewing process by a human, it also increases the accuracy of the decision.

### Cognitive Insight

Through offering more potentially useful information on complex portions of the process, cognitive insight also drives efficiency and accuracy, which could provide help in the decision-making process, but the predictive model will leave the final decisions to the human users.

In the complex underwriting case, the predictive model could present granular visibility into the specific issues for given cases, it informs underwriter the items that need for their special evaluation. Further, cognitive insight could let the underwriter notice the unforeseen or unapparent evidence, which guides underwriters to make correct decisions. Some reinsurance companies already developed the underwriting toolkit for primary insurance companies, primary insurance companies' underwriters could upload the complex case into the toolkit, the system will give the feedback of questions that need specially address and provide an initial decision for reference.

The classification model is one of the predictive analytics methods that provide valuable underwriting insights.

The risk classification model uses historical loss data, insurance applicant characteristics (user portrait), and market variables to classify the applicant's risk level based on specified characteristics. Besides the covered risk, underwriters could also obtain an understanding of the potential risks associated with the applicants, such as the risk of misrepresentation, adverse selection, and the possibility of fraud claim reporting. After combining the overall risk, the underwriter could make the final decision with help from the model.

Accurately projecting the probability of expected outcomes can help underwriters set accurate expectations for the individual risk and the business line profitability. The united prediction model and the working process can also unify the different business processes in different business areas and reduce unnecessary waiting times.

The classification model could also drive efficiencies in customer submitting insurance application side and then improve the customer experience. After answer some basic questions, the model will give the customized document list based on the customer characteristic, which means each customer's document list might be different. For example, low-risk customers do not need to provide any additional documents in their application, while the high-risk customers may need to provide some sophisticated documents. Different insurance companies already developed customized document checklists based on different insurance products and customer types. These benefits can be further increased by the automated process of document type automated classification, extraction, and OCR technique. For example, in China, nearly every hospital's formats of the medical report, expense list, and invoice are all different, PICC Health Insurance is working on distinguishing the different documents and read the content by machine, which could dramatically save insured time in uploading different documents to correct windows.

## Claim Management

Claim settlements are the biggest expense for every insurance company, so insurance companies would like to understand the claim case and potential claim pattern as much as possible. Predictive analytics could provide help in the whole claim process and save unnecessary waste in different aspects, such as fraud detection, outlier identification, loss reserving estimation, and claim service improvement. It also contributes to budget management by using predicted results and balancing workload distributions and gives insurance companies strategic advantages.

### Fraud Claim Identification

Insurance companies are always battling with various fraud claims, but until now, they still not as successful as they would like to be. Based on The Coalition Against Insurance Fraud estimation, approximately USD 80 billion in fraudulent claims are made annually in the United States (all insurance lines). Additionally, fraud makes up 5-10% of claims costs for insurers in the United States and Canada. The Coalition also reports that more than one-third of people hurt in auto accidents exaggerate their injuries which caused 13-18 billion to US insurance bill, and nearly one-third of doctors exaggerate the severity of a patient's illness to help avoid the early discharge from a hospital.

The traditional methods that insurance companies used to detect claim fraud are identifying claim patterns, controlling underwriting activities, and using the special investigation unit (SIU) after the claim is reported. Most of these fraud solutions are rules-based which means it is easy for fraudsters to manipulate within the process and get around the designed rules. On the other hand, the predictive analysis uses the combination of rules, prediction modelings, text mining, and database searches to identify fraud.

Some insurance companies also use social media for signs of fraudulent behavior and use data gathered after a claim is reported to monitor insureds' online activity for potential fraud. For example, a claim specialist will compare the social media post and the claim statement to discover the evidence of the claimant lying.

By using predictive analytics, insurance companies can identify and prevent potential fraud before it happens and take corrective measures accordingly. Insurance companies also rely on predictive modeling for fraud detection or claim discrepancy. The most used methods in detecting claim fraud are clustering analysis and classification tree.

To identify the fraudulent claim, insurance companies build their fraud lists based on traditional fraud indicators (such as claimant continually push claim specialist for a quick settlement or provide too much/ too little documentation) or social media data mining. After that, insurance companies use social network analysis to examine suspicious links, connections, or relationships in a network. At last, the insurance companies use clustering analysis to discover the claim characteristics that indicate fraud.

Predictive analytics also uses text analytics and sentiment analysis to look at the big data behind the claim to detect fraud. In the claim department, a typical text analytics follow the process below:

- Claim adjusters draft claim report when investigate the claim;
- Clues are often hidden in the report, but the claim adjuster might not notice it;
- Claim report was input into the analytics system which was built on business rules and learned fraud pattern (such as the claimant alters the story over time), the model identifies the possible fraud evidence and gives the fraud claim score.

Although lots of insurance companies can identify fraudulent claims by analytics, there is still a lot of undetected frauds, the main reason is that fraud indicators are from past fraud. Intelligent and innovative fraudsters will change their fraud approach and pattern, this will limit indicator usefulness. Another reason is that insurance companies only have very limited historical data to train the predictive model, and the identified data may be lagged the new fraud pattern.

### Outlier Claims Identification

Outlier claims are those claims with unexpected high-cost loss. Predictive analytics can help insurance companies identify outlier claims. With the proper analytics tools, insurance companies can review claim cases and find similarities automatically and send suspicious claims to claim specialists or Special Investigation Unit (SIU) for further review or investigation. This method could dramatically decrease the workload of the claim department. Advanced notice of potential loss can also help insurance companies reduce the amount and the cost of outlier claims. Some health insurance companies in China are attempting to use analytics tools to filter all submitted claim first and mark the potential outlier or fraud claims with different colors of flags which stand for the risk levels, the claim specialist could only focus on those claims with higher risk.

### Loss Reserving Estimation

When a claim is first reported, it is impossible to predict the claim's final size and duration, especially in the long-tail claims, such as claims of liability insurance and worker's compensation. However, accurate loss reserving and claims forecasting are essential to the insurance companies' operations because it will affect the assessment of the current operation situation and future marketing and pricing strategy.

Predictive analytics can more accurately calculate loss reserve by comparing a loss with similar claims and then develop the potential pattern of the loss development. When claim data is updated, the analytics model could re-assess the loss reserve, evaluate the current loss development, and predict the final loss with updated information, so the insurance companies could understand the current business situations and could make better decisions on future development.

### Claim Process Transformation and Claim Timeliness Improvement

Claim service might be the most obvious customer service-oriented function in the whole core value chain of insurance. Customers are expecting to obtain a fast and personalized service, especially when they experience an unexpected loss. In the P&amp;C insurance industry, the demand for faster service may contradict the accuracy requirement of claim reviewing and present a challenge to insurance companies. With good predictive analytics systems, insurance companies can prioritize certain claims to save time, money, and resources, and the final goal is to retain business and increase customer satisfaction. Based on this point, the predictive analytics tool can anticipate the insured needs, understand their concerns, and then improve the relationship with the customer.

In 2018, Ant Financial (a fin-tech subsidiary company of Alibaba) released the investigation claim tool &quot;DingSunBao 2.0&quot; for the insurance industry. With the claim tool, after the car accident, the car owner only needs to take 6-10 pictures and upload them to the specific app, the app could identify the detailed damaged parts and estimate the possible expense of repairing in a minute. It is much faster than the traditional human adjuster handling process, which needs the car owner to call the insurance service hotline to report the loss, then send different paper or electronic documents to insurance companies or agencies, and wait for adjusters investigation and obtain claim result. DingSunBao simplifies all these processes and already helped the insurance industry to save 750,000 working hours of claim adjuster. Customers also get satisfied with the faster claim payment speed. In 2019, PingAn P&amp;C Insurance (the second-largest P&amp;C insurance company in China) published its new claim investigation and payment system, similar to DingSunBao, the customer needs to upload the pictures of the car damaged parts to the app, and the system will provide the estimated cost and recommend nearest factories or service center for repairing. Moreover, the claim payment will be transferred to the customer's bank account in seconds if the estimated damage is less than RMB 2000 (CAD 400). All these increase customer satisfaction toward claim service.

## Customer Service

Predictive analytics could help tailor customers' experience as it happens. The customer's reaction will impact the next feedback. Through predictive analytics, companies can capture what customers want at the contact moment, or exceed their expectations based on customer feedback and preferences.

When customers provide initial feedback, some companies use predictive analytics to precisely forecast customers' needs or provide early detection of precursors of customers' behaviors. This allows companies to be more proactive in customizing the services and then effectively serving customers.

### Customer Experience Optimization

Many consumers value tailored experience. Predictive analytics provides a way that insurance companies could understand the needs of customers rapidly when customers connect with the insurer.

For online customer service, the chat bot could predict the potential raised questions of the customer through observing the real-time input, and pop up the solutions, or transfer the issue to the determined respective department. To save customers time, the analytical model could be attached to the insurance policy database can bridge the possible information gap, and the customer could get what they need in a short time.

### Risk Management Oriented Customer Service

As mentioned above, the essence and the goal of future insurance is to help the customer to better manage their different risk (avoid risk, mitigate risk possibility or the risk result), instead of only providing monetary compensation after losses. By using predictive analytics and related smart product (such as wearable and intelligent helmets), insurance companies can predict the risk of customers' specific activities and then recommend the risk control or risk management methods accordingly.

# POTENTIAL PROBLEMS OF PREDICTIVE ANALYTICS

Predictive analytics had developed for many years, it is still a hot topic. In the insurance industry, nearly all insurers find that the benefits of predictive analytics out-weigh its costs, however, as with other analytics methods or tools, the predictive analytics techniques also entail disadvantages and limitations on its usability in particular business situations. Below are some issues that need to pay attention to.

## Technique Issue

Like other techniques, any predictive analytic model has its technique limitations based on the algorithms or the dataset it is based. When deciding to use predictive analytics, we should be aware of those potential limitations.

### Inherent Inaccuracy

A predictive model's potential for inaccuracy is an important consideration for insurance companies that rely on predictive modeling. Even the best model cannot always be 100% accurate, also as the business and market change, the model may not reflect the original business need and patterns.

An error term represents the portion of the model that is unexplained. The error term can be substantially different for various models and can result in significant variation between predictions and actual outcomes.

Errors in predictive models might be caused by errors in model specification. A model may include factors that are not significant predictors, or the potential significant factors be excluded or unobserved. The final source of error of a predictive model may also from the model's multiple assumptions, the difference between the development period and the actual usage may generate different assumptions. The significant changes in the parameters may invalidate a model. For example, the economic downturn or recent regulation change may substantially change the fraudulent claims numbers and the hidden claim pattern. If in the development period, the predictive model does not include any economic downturns effect or potential regulation change effect, it may not properly reflect the expected results of fraudulent claims during that period.

### Opaque Processes and Outcomes

Predictive analytics is an opaque process. The complex processes that underlie predictive analytics techniques are usually overwhelming for many people. This leaves customers and some model users get lost in the final decisions, they may unaware of the reasons why the application or claim case is rejected. The complexity and the opaque process make the situation, in which even the customer know all detailed information, they still cannot learn enough knowledge of the model, and then cannot know the logic behind the models.

For business purposes, most of the predictive models and the algorithms are opaque because they are subject to copyrights, so the public or individual doesn't know who wrote the program or whether the assumptions in the model apply to him/ her, and whether they are treated fairly.

## Privacy Issue

Predictive analytics have different forms, so the privacy implications, scopes, and implementations can also vary accordingly. As mentioned above, big data and predictive analytics can help in advanced research and innovation, it also brings new approaches to understanding the world and provides valuable decisions. On the other hand, because advanced predictive analytics improve the data collection, sharing, and linkages, it also poses potential privacy invasion, discrimination, or even ground of surveillance society. In this part, we will talk about the individual and societal privacy problems raised when implementing predictive analytics.

### Beyond Reasonable Expectations

Although inaccuracy is the technical problem of predictive analytics, accurate predictions could be a greater invasion of privacy in certain contexts. Through predictive analytics, even all the data acquisition related actions follow regulation, the possibility of revealing the individual's unexpressed desires or intentions could violate the privacy of the person. The use of predictive algorithms and deep analysis performed by trained specialists who can access data could make people feel the core privacy was violated because the specialists and scientists can inference the truth beyond what could be easily observed or known. In other words, those presumptions that are made based on easily observable activities are generally not offensive to people, however, the presumptions that are derived from deeper observations and understandings performed by machines and science may be unexpected and may go beyond people's reasonable expectations. Although the deep understanding might reveal some insights into people's lives, it also might be a double-edged sword.

### Discrimination

One of the applications of predictive analytics is to profile and categorize individuals based on his/ her future behaviors and intentions' inferences. In the customized advertisement and customized product development, some companies would like to gain more profits by excluding some customers from the accessibility of regular products or services. Furthermore, some companies could discriminate specific customer groups by different buying scenarios or dynamic pricing structures based on their characteristics such as willingness to pay, purchasing habit, and potential behavior after buying.

In September 2000, a leading online shopping website outraged some customers when the price discrimination was revealed. One buyer reportedly deleted the cookies on his computer that identified him as a regular customer. As a result, he watched the price of a DVD dropped from $26.24 to $22.74. Other consumers also discovered that in 2000, the leading company was using dynamic pricing when customers comparing prices on a &quot;bargain-hunter&quot;.

The same things also happened in China. The discriminating dynamic pricing issue was revealed in 2018. In 2020, several online shopping websites and online travel agencies were discovered to use the online shopping history and browse history to customize the price for different customers.

Although some countries already enacted laws or regulations to regulate discriminating predictive analytics, advanced technology can still use different ways to &quot;escape&quot; from the supervision. Moreover, considering customers are in disadvantaged positions of information asymmetry, it is hard for customers to obtain solid shreds of evidence.

### Knowledge and Consent

Consent is the key to govern privacy issues, it requires individuals to have basic understandings of how their information will be used and how to provide meaningful consent for its collection and use. The problem is that traditional consent form might not apply to the current complex and advanced data analytics (including predictive analytics).

In general, some people would like to use personal privacy or other personal information for free or low-price products or services. Based on this trend, some insurance companies provide free insurance coverage or insurance coverage at a low price to obtain personal information for further usages, such as cross-selling or data mining.

Some companies can obtain consent by including ambiguous &quot;notice&quot; to customers, and notices of obtaining different personal information are hidden deep within the privacy policy that consisted of complex legal language. Even organizations can explain personal information handling practices in lengthy terms and conditions or privacy policies, a common customer may still not read or understand it. However, summarized or simplistic styled personal information handling practices might also not helpful because it ignores the details that may make differences for privacy. In other words, transparency can leave customers incomprehensible and overly permissive to companies.

### Privacy Law

In different countries, privacy-related laws place different degree limits on the collection, storage, and usage of personal information. Some laws, such as the General Data Protection Regulation (GDPR), require personal information can be only collected where it directly relates to the operating programs or activities. Some laws require data collection departments to inform individuals the personal information purposes and authorities.

The decision of implementing predictive analytics should be preceded by careful considerations of the privacy impacts, the necessity of using predictive analytics, whether its use is reasonable and proportionate to the outcomes, and whether the program is effective.

## Cost and Benefit Comparison

In addition to the technique and privacy issues, many insurance companies may have to change their operation methods or processes when using predictive analysis techniques.

Insurance companies may have to consider continually invest money into hardware and software necessary to facilitate predictive modeling.

Also, previous poor data entry quality, poor record-keeping, and multiple systems bring the insurance companies uncleaned or inaccurate data that are necessary to support successful predictive modeling developments. During this process, data cleaning and data integration might last years to finish, and it involved inter-department or inter-company efforts.

As with other substantial changes in daily operations, insurance companies may also encounter resistance from internal departments, for example, the traditional operation department employee may not satisfy with the new models that will marginalize their current jobs or replace their jobs finally.

# CONCLUSION

Many insurance companies have begun to explore the application of big data in the industry and hope to leverage the information and analytics advantage into actionable insights, and then improve the operations and performance. To make the exposure and risk-return prediction more accurate, some insurance companies have adopted predictive analytics techniques in their core operations.

Predictive analytics involves the technology of multi-sources data collection and data analysis, the final goal is to help people better understand and predict behaviors, and extract meaningful insights and actionable information. It also investigates and analyzes the current and historical facts and patterns, and then predict the events' possible outcomes.

In this article, we introduced some predictive analytics underlying technologies and related applications in the insurance industry, especially in the fields of marketing and sales, product development, underwriting, claim management, and customer service. We also talked about some problems in using practicing predictive analytics.

When using the predictive analytics technique, although we need to pay attention to some potential problems, such as technique and privacy issues, we still believe the fair usage of predictive analytics could bring better understanding, actionable insights, and more advantages to our life and for the insurance industry.

# REFERENCE

1. [Predictive analytics](https://en.wikipedia.org/wiki/Predictive_analytics)
2. [Levels of Data Analytics](http://www.ithappens.nu/levels-of-data-analytics/)
3. [Top 6 Use Cases of Predictive Analytics in Insurance](https://www.formotiv.com/predictive-analytics-insurance-use-cases/#behavioral-analytics-predict-new-customer-risk)
4. [5 Benefits of Predictive Analytics for the Insurance Industry](https://diggyinsurance.com/5-benefits-of-predictive-analytics-for-the-insurance-industry/)
5. [Predictive analytics solutions](https://www.milliman.com/en/services/predictive%20analytics%20solutions)
6. [Predictive Analytics for Insurance - Part 1: What's Truly New for the Industry?](https://www.earley.com/knowledge/article/predictive-analytics-insurance-part-1-what-s-truly-new-industry)
7. [Predictive Analytics for Insurance Part 2: Classes of Application and Tools for Competitive Advantage](https://www.earley.com/knowledge/article/predictive-analytics-insurance-part-2-classes-application-and-tools-competitive)
8. [Business Intelligence, Planning and Predictive Analytics for Insurance Providers](https://www.board.com/en/insurance-providers#gref)
9. [InetSoft Webinar](https://www.inetsoft.com/business/bi/predictive_analytics_transform_insurance_industry/)
10. [Predictive Analytics for Insurance](https://www.spssanalyticspartner.com/industry-solutions/insurance/)
11. [Predictive Analytics in Property and Casualty Insurance: Real Value or More Empty Promises](https://www.the-digital-insurer.com/wp-content/uploads/2013/12/80-Consulting_Whitepaper_Predictive-Analytics-Property-Casualty-Insurance_05_2011.pdf)
12. [Analytics: A Powerful Tool for the Life Insurance Industry](https://www.capgemini.com/wp-content/uploads/2017/07/Analytics__A_Powerful_Tool_for_the_Life_Insurance_Industry.pdf)
13. [Yitu Technology](https://www.yitutech.com/en)
14. [保险大数据的痛点、现状、误区、解决之道和挑战](http://www.cbdio.com/BigData/2018-04/13/content_5702567.htm)
15. [淘宝退货运费险7周年：互联网保险的双十一狂欢](http://www.baoxianguancha.com/content-11-5020-1.html)
16. [蚂蚁金服升级车险定损宝：车主拍视频即可得到维修方案和价格](https://www.thepaper.cn/newsDetail_forward_2118355)
17. [保险科技技术发展趋势报告:大数据应用有两大重要意义](https://finance.sina.com.cn/money/insurance/bxyx/2020-04-01/doc-iimxyqwa4459828.shtml)
18. [大数据时代下，保险业迎来了怎样的机遇与挑战？](https://cloud.tencent.com/developer/article/1106747)
19. [轻微事故车主自助理赔 平安产险首推车险&quot;信任赔&quot;](https://m.21jingji.com/article/20190103/herald/5b109dd038b7b648e49635738fc5591c.html)
20. [Insurance Customer Purchase Prediction Based on Data Optimization](https://m.hanspub.org/journal/paper/32671)