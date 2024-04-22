# Master of Science Business Analytics - Capstone - Swire Coca-Cola Innovative Products Forecasting

## Business Problem

Swire Coca-Cola, USA, is responsible for producing, selling, and distributing Coca-Cola and various beverages across 13 states in the American West. The company is committed to continuously introducing innovative products into the market. These innovative products are designed to align with the discerned preferences and loyalty of the customers, but sometimes, they fail. 

Swire Coca-Cola encountered significant production and inventory management challenges for its new innovative products, Starlight and Dreamworld, which each exhibited distinct sales patterns requiring enhanced forecasting and strategic planning. For Starlight, robust sales persisted for 30 weeks, followed by a decline due to supply shortages. This issue hindered the company from capitalizing on the intense media support and public interest that could have further boosted sales. Conversely, Dreamworld experienced a sharp initial sales peak, quickly diminishing after 14 weeks. This decline was not attributed to supply chain issues but to overproduction based on overly optimistic demand forecasts, leading to excessive inventory and consequent financial losses.

Swire plans to release seven new innovative products. The main aim is to enhance its production planning and management specifically for these innovative products. The primary challenge requires forecasting the demand to mitigate instances of out-of-stock or overproduction of these innovative products, thereby maximizing profits.

## Solution

The first notebook, EDA, will examine Swire Coca-Cola's Exploration Data Analysis with data explorations, insights, and visualizations.
Utilize the Exploratory Data Analysis (EDA) to thoroughly examine the product's sales data, identifying key insights such as peak sales periods and notable seasonal trends. This detailed analysis will help uncover patterns and fluctuations in sales that are crucial for strategic planning and decision-making. 

Additionally, Exploratory Data Analysis (EDA) facilitates understanding why certain regions exhibit higher sales by analyzing the demographic dataset and establishing correlations between demographic factors and product preferences. This process helps identify which product categories or flavors perform well in sales and regions. This can help in targeting the distribution regions.

The second notebook, modeling forecast, will examine the forecasting of innovative products.

Identify standard products that closely align with the characteristics of the specified innovative products and utilize the sales data of these analogous products to forecast future sales.

**Selection of Comparable Products -** Choose the products that most closely match the innovative items in terms of brand, market category, manufacturer, package type, and flavor, ensuring they align closely with the specifications of the new products.

**Data Integration -** Filtered the dataset based on seven new innovative products and filtered it based on demographics like age and region.

**Sales Data Analysis -** Examined the weekly sales figures of these selected similar products to understand their market performance over time.

**Forecast Modeling -** I used ARIMA, Prophet, and Exponential smoothing time series forecasting models to predict future sales. I used the Mean Squared Error (MSE) and Mean Absolute Error (MAE) metrics to evaluate the best-performing model. 

In addition, I used the non-Swire's competitive data to forecast their sales of similar products, analyze their performance when compared to Swire's products, and compare both sales to identify patterns and public sentiments.

## Contribution

Led the project by formulating a clear business problem statement tailored to Swire Coca-Cola's requirements. An initial phase of Exploratory Data Analysis (EDA) was conducted to derive actionable insights from the datasets provided, aiming to address the specific challenges faced by Swire Coca-Cola. Utilized Google Big Query, I efficiently filtered large datasets into manageable formats and subsequently imported them into Google Colaboratory for detailed further analysis. This analysis included identifying seasonal trends, peak sales periods, and the performance of various flavors, packets, brands, and manufacturers. Data was further enriched by integrating demographic information, enabling targeted analysis of flavor preferences across different age groups and in the Southern and Western regions.

Similar existing products were identified to align closely with Swire Coca-Cola’s innovative product lines, and their sales were forecasted using ARIMA, Prophet, and Exponential Smoothing models. These models were evaluated based on their performance metrics. The findings provided recommendations on optimal periods and regions for launching these innovative products, leveraging the predictive power of the selected forecasting models.

## Business Value

**Optimal Launch Strategy -** The forecasting model developed for Swire Coca-Cola identifies the most favorable periods and regions for introducing specific innovative products. This strategic insight allows for an effective market entry, maximizing initial impact, long-term success, and customer satisfaction.

**Enhanced Inventory Management -** The model significantly aids inventory management by predicting demand more accurately. This helps Swire Coca-Cola optimize its stock levels, thereby reducing costs associated with excess inventory and minimizing the risk of product wastage.

**Insightful Product Analysis -** The analysis delivers valuable insights into Swire Coca-Cola’s most robust product offerings and aligns them with effective inventory management practices. This ensures that the best-performing products are adequately stocked and promoted, enhancing overall profitability.

**Targeted Marketing Strategies -** The project provides detailed information on the most responsive age groups and ideal climatic conditions for Swire Coca-Cola’s flavored drinks. This enables the company to design marketing strategies that are highly targeted and more likely to resonate with their intended audience.

**Competitive Analysis -** By comparing the sales performance of Swire Coca-Cola’s products against their competitors, the analysis offers a clear perspective on market position and competitive strengths. This allows Swire Coca-Cola to identify product improvement and innovation areas, enhancing its competitive edge in the marketplace.

## Challenges

**Dataset -** The dataset doesn't include data specific to the innovative product categories of interest. So, predicting future sales with a dataset that has yet to describe the innovative products is quite challenging. Careful consideration is required to approximate the attributes of these innovative products by analyzing similar existing products within comparable categories.

**Time Series -** Selecting an appropriate time series model for forecasting sales is inherently complex due to the nuances of historical sales data. We employed various popular time series models and assessed their performance using Mean Absolute Error (MAE) and Mean Squared Error (MSE) metrics to ensure robust evaluation.

**Data Integration -** Combining data from demographic and sales datasets presents challenges, particularly with the large volume of data that can lead to potential duplication. We utilized Google Big Query to manage and scrutinize data for duplicity efficiently, ensuring the integrity of our data integration process.

**Confidence Intervals -** Given the uncertainties in correctly identifying the products within the dataset, it is crucial to establish confidence intervals for the sales forecasts. These intervals provide a range for potential high and low sales figures, accommodating the variability and enhancing the reliability of our predictions.

**Computation Power -** The substantial dataset size demands significant computational resources, which has previously led to system instability and crashes. To mitigate this, we have implemented cloud-based GPUs to handle the extensive computations required.

**Validation -** Due to our reliance on similar products as proxies for the innovative products in our analysis, direct validation of model outputs is not feasible.  We will devise a validation methodology incorporating probability distributions and confidence intervals to circumvent this limitation. This approach will enable us to provide reliable estimates despite the absence of direct data on the innovative products.

## Lessons Learned

**Dataset Attribute Analysis -** Understanding the attributes within the dataset to select products that closely mirror innovative ones accurately.

**Data Management via Google Big Query -** Using Google Big Query to effectively manage and filter the extensive dataset, transferring refined data to Google Colab for further analysis.

**Time-Series Forecasting Proficiency -** Developed a deep understanding of time-series forecasting, using MSE and MAE metrics to optimize model selection and enhance forecast accuracy.

**Seasonal Sales Understanding -** Learned insights into the seasonal trends and their impact on product sales.

**Influence of Reviews and Tastes -** Recognized how consumer reviews and product taste preferences affect sales outcomes.

**Demographics on Sales -** Demographics (regional, climatic, age, and ethnic demographics) influence beverage sales, adding the need for demographic considerations in sales strategies.

**Engagement with Industry-Specific Datasets -** Extensive understanding of real-world, industry-specific datasets and application of business-oriented problem-solving techniques.

**Computational Effectiveness -** Learned cloud-based GPUs to manage high computational demands efficiently, improving system stability and performance.

**Translation of Analytics to Business Results -** Knowledge of converting analytical insights into concrete business outcomes, reinforcing the strategic value of data-driven decisions.

**Navigating Industry Complexities -** Acknowledged and adapted to the complexities and uncertainties in beverage sales, underlining the importance of flexibility and informed decision-making in the industry.


**[EDA Notebook](https://github.com/AbhiramMannam/Swire-Coca-Cola-Forecast/blob/main/Capstone_Completion_EDA.ipynb)**

**[Modeling Notebook](https://github.com/AbhiramMannam/Swire-Coca-Cola-Forecast/blob/main/Capstone_Completion_Modeling.ipynb)**

**[Presentation](https://github.com/AbhiramMannam/Swire-Coca-Cola-Forecast/blob/main/Swire_Innovators_Capstone%20Presentation.pdf)**

**[Award](https://github.com/AbhiramMannam/Swire-Coca-Cola-Forecast/blob/main/Abhiram%20Mannam%20Spring%202024%20MSBA.pdf)**

**[Website](https://swirewebsite-kxgpyieata-wm.a.run.app/)**






