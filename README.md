# Product-Delivery-Date-Prediction-

**Abstract**



In this project, we created and tuned models to predict delivery times for eBay packages given a dataset of eBay shipment records. We implemented four models—linear regression, fully connected neural network, XGBoost, and CatBoost—and compared the their effectiveness on the shipment data. We additionally examined different strategies to clean our dataset, engineer new features, and fine-tune each model. Ultimately, the fully connected model performed the best.

**Introduction**


The economy of online shopping is bigger than it has ever been and continues to grow each year. It follows that the market for being able to deliver goods quickly and reliably is becoming more and more competitive. In addition to improving the overall flow of transactions, knowing when a package will be delivered is a major factor in customer satisfaction, making the ability to accurately predict delivery dates essential to companies such as eBay.

The process of achieving this, however, poses many challenges. In the case of eBay, the majority of transactions are carried out between individual sellers and buyers, often resulting in the data for goods and their delivery being inconsistently recorded. This, in addition to packages being processed by a variety of different delivery services, means that data labels are frequently missing or incorrect. Further, the shipment date is largely left to the sole decision of each individual seller, resulting in a high degree of variability.

**Approach**

We worked to provide a solution to these problems and provide a model to enable the accurate prediction of delivery dates using machine learning.

To implement our model, a number of decisions were made and tested, including deciding the optimal means by which to clean the data (for instance, whether to omit training data that has missing or incorrect features or to assign it average values based on correctly labeled training data), deciding whether to compute the estimation holistically from shipment to delivery date or to compute multiple separate estimates on separate legs of the delivery process, and deciding which features to include and in which leg.

Should our model have some error, it is important that it produces random rather than systematic error. Specifically, we want to avoid creating a model which might consistently predict early delivery dates, which could lead to sellers and delivery services rushing packages and resulting in the employment of more non-sustainable methods, such as shipping half-full boxes, as well as increasing the pressure on employees to have to work faster and faster.


