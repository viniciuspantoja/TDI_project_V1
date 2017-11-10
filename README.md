<p>Content Based Recommendation System for Portfolio Managers</p>

<p>Project Proposal</p>

<p>1. Introduction</p>

<p>This project uses content based recommendation systems to recommend stocks to portfolio managers. The databases used to achieve the result are MorningStar financial and key ratios database, and Bureau Economic Analysis (BEA) sectorial databases. </p>

<p>2. Opportunity</p>

<p>There are over 300.000 portfolio managers in United States, most of them with a background on management. Most of them are self-employed, and have as clients their friends and close people who wishes to have their money applied in the stock market. Due to the big cost of hiring data scientists, their investment strategy doesn’t use the latest innovation on data analysis.</p>

<p>3. Solution</p>

<p>Our platform starts by receiving the investor’s portfolio and retrieving the following information:</p>

<p>a. The risk level of the portfolio;</p>

<p>b. Recommended stocks for diversifying the portfolio maintaining the risk level</p>

<p>c. Recommend stocks to invest, given a desired risk level; </p>

<p>3.1. Risk level </p>

<p>The risk level will be assessed by calculating the following risk indicators:</p>

<p>a. Interest Coverage Ratio – how many times the earnings can pay the interested owned in that year by the company</p>

![alt text](https://github.com/viniciuspantoja/TDI_project_V1/blob/master/aal_interest_coverage.png)

<p>b. Merton’s Model – Model that assess risk using option theory</p>

<p>c. Machine learning to approximate Moodys’ KMV model – Moodys’ KMV model is a proprietary model that uses a similar structure of Merton’s Model, but its details are not known. However, we have the output of the model (the ratings that Moody releases). As we have the information of the company, I’ll use deep learning to approximate it’s rating function. </p>

<p>3.2. Recommendation system</p>

<p>Here I will use a content based recommendation system. In other words, I’ll use information of the stocks to see which stocks have the same profile. The information used are divided in 6 big blocks:</p>

<p>a. PRICE RATIOS</p>

<p>a. Price to Earnings</p>

<p>b. Price to Book</p>

<p>c. Dividend Yield</p>

<p>b. PROFITABILITY RATIOS</p>

<p>a. Return on Assets</p>

<p>b. Return on Equity</p>

<p>c. Profit Margin</p>

<p>c. LIQUIDITY RATIOS</p>

<p>a. Current Ratio</p>

<p>b. Quick Ratio</p>

<p>d. DEBT RATIOS</p>

<p>a. Debt to Equity</p>

<p>b. Interest coverage Ratio</p>

<p>e. EFFICIENCY RATIOS</p>

<p>a. Asset Turnover</p>

<p>b. Inventory Turnover</p>

<p>f. Sectorial Information</p>

<p>a. Sector</p>

<p>b. Growth</p>

<p>c. 5 year tendency</p>

<p>I have the first results in this part. The graphs bellow shows the Asset turnover of recommended stocks, in case you own American Airlines stocks (AAL):</p>

![alt text](https://github.com/viniciuspantoja/TDI_project_V1/blob/master/aal_asset_turnover.png)

<p>This second graph shows the current ratio of the recommended stocks in case you own AAL:</p>

![alt text](https://github.com/viniciuspantoja/TDI_project_V1/blob/master/aal_current_ratio.png)

<p>3.3. Recommended stocks given a desired risk level</p>

<p>Finally, the manager can choose a goal risk level and the recommendation system will output those companies that have similar profile, but with the target risk level. </p>
