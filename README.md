XAI606
# Project proposal I (objective & dataset)

## I. Project Title:
#### Improving Bankruptcy Predictions: Neural Techniques Leveraging Taiwanese Bankruptcy Data
## II. Project Introduction:

### Objective:

To design and implement a neural network model that can accurately predict the risk of corporate bankruptcy from given financial indicators

### Motivation:

Bankruptcies can have ripple effects across economies, affecting job markets, stock markets, and the general health of the financial system. Traditional statistical methods of predicting bankruptcy, while effective, might not capture the intricate relationships present in modern financial systems. Neural networks, with their ability to learn and generalize from complex datasets, offer an avenue for enhancing predictive accuracy. Given the advancements in deep learning and the increasing availability of financial data, this project seeks to explore the potential of neural networks in the realm of financial forecasting.

## III. Dataset Description:

### Source: 

#### [ Taiwanese Bankruptcy Prediction. (2020). UCI Machine Learning Repository. https://doi.org/10.24432/C5004D. ]
The dataset, sourced from the UCI Machine Learning Repository, contains financial attributes of Taiwanese companies from 1999 to 2009, and it's structured to assist in predicting the possibility of bankruptcy based on these financial attributes.

The dataset comprises 95 features (financial attributes) that represent different financial metrics, providing insights into various aspects of a company's financial health. Additionally, there is 1 label that indicates the bankruptcy status.

###  Features (Financial Attributes):
Here's what each feature means.
#####	1	ROA(C) before interest and depreciation before interest: Represents the Return on Assets, prior to accounting for interest and depreciation. It provides an insight into the company's efficiency in using assets to generate earnings without certain deductions.
#####	2	ROA(A) before interest and % after tax: Measures Return on Assets before interest deductions and after considering taxes. This ratio can indicate the effectiveness of asset usage in generating post-tax returns.
#####	3	ROA(B) before interest and depreciation after tax: Reflects the Return on Assets, before interest but after deducting depreciation and tax. This shows profitability related to asset utilization, adjusted for depreciation.
#####	4	Operating Gross Margin: Denotes the percentage difference between revenue and the cost of goods sold. It's vital in gauging the core profitability of the company's primary operations.
#####	5	Realized Sales Gross Margin: This is the actual gross margin achieved from sales, considering possible returns or discounts. It provides a real-world view of sales profitability.
#####	6	Operating Profit Rate: Measures the profitability from the main business operations as a percentage of sales. It's a key metric to understand how efficiently the core operations are generating profits.
#####	7	Pre-tax net Interest Rate: The net interest rate before accounting for taxes. It helps businesses understand the cost of debt relative to their earnings, without tax implications.
#####	8	After-tax net Interest Rate: Reveals the net interest rate once taxes have been accounted for. This offers insights into the real cost of financing after tax deductions.
#####	9	Non-industry income and expenditure/revenue: Compares income and expenditure that's not directly related to the primary business operations to revenue. This helps to identify ancillary streams or costs in relation to primary revenue.
#####	10	Continuous interest rate (after tax): This denotes the consistent interest rate after accounting for taxes. It's vital for assessing the sustained cost of debt in a post-tax scenario.
#####	11	Operating Expense Rate: Demonstrates operating expenses as a percentage of sales. A crucial metric to understand the operational efficiency of a company.
#####	12	Research and development expense rate: Represents the proportion of sales spent on R&D. This can indicate the company's commitment to innovation and future growth.
#####	13	Cash flow rate: Provides a snapshot of the company's cash flow in relation to its size or operations. It's essential for gauging liquidity and operational efficiency.
#####	14	Interest-bearing debt interest rate: Shows the interest rate on debt that carries interest. This rate is crucial for understanding the cost of borrowed funds.
#####	15	Tax rate (A): This provides the effective tax rate imposed on the company. Helps businesses anticipate tax obligations and strategize accordingly.
#####	16	Net Value Per Share (B): Represents the intrinsic value of each share. Investors use this to understand their stake's underlying value in the company.
#####	17	Net Value Per Share (A): This signifies the intrinsic value attributed to each share. It's a key metric for shareholders assessing the worth of their investment.
#####	18	Net Value Per Share (C): This measures the value of each share. It offers another perspective on the per-share value of the company.
#####	19	Persistent EPS in the Last Four Seasons: Highlights the consistency in Earnings Per Share over the last four quarters. This is pivotal for understanding earnings stability across the year.
#####	20	Cash Flow Per Share: Denotes the cash flow generated per outstanding share. It's crucial for investors to gauge a company's liquidity and cash generation efficiency on a per-share basis.
#####	21	Revenue Per Share (Yuan ¥): Indicates the revenue earned for every share, denominated in Yuan. Useful for shareholders to measure the company's sales performance against the number of shares.
#####	22	Operating Profit Per Share (Yuan ¥): Provides the amount of operating profit attributed to each share, measured in Yuan. It helps investors understand the profitability from core operations relative to their shareholdings.
#####	23	Per Share Net profit before tax (Yuan ¥): Details the net profit before tax divided by the number of shares. This metric gives a pre-tax profitability assessment on a per-share basis.
#####	24	Realized Sales Gross Profit Growth Rate: Measures the growth rate in gross profit from actual sales over a specific period. It's essential for tracking the enhancement or reduction of sales profitability.
#####	25	Operating Profit Growth Rate: Examines the growth rate of profit derived from primary operations. It's pivotal for understanding the trajectory of core business profitability.
#####	26	After-tax Net Profit Growth Rate: Assesses the growth of the net profit after accounting for taxes. It's key for tracking the net profitability trend of the company.
#####	27	Regular Net Profit Growth Rate: Analyzes the growth of consistent net profit over time. This ratio reveals the stability and predictability of a company's earnings.
#####	28	Continuous Net Profit Growth Rate: Chronicles the sustained net profit growth, typically over successive periods. Useful for understanding long-term profitability consistency.
#####	29	Total Asset Growth Rate: Indicates how rapidly the company's assets are growing. This metric is fundamental for assessing whether a company is in expansion or consolidation mode.
#####	30	Net Value Growth Rate: Tracks the growth rate of the company's net value. It's crucial for evaluating how effectively the company accumulates wealth over time.
#####	31	Total Asset Return Growth Rate Ratio: Shows the growth rate ratio of the returns generated from total assets. This is pivotal for comparing how efficiently assets are utilized year over year.
#####	32	Cash Reinvestment %: Illustrates the percentage of cash earnings that are reinvested back into the business. A key indicator of the company's growth strategy and capital allocation.
#####	33	Current Ratio: Compares a company's current assets to its current liabilities. Essential for understanding short-term liquidity and the ability to meet short-term obligations.
#####	34	Quick Ratio: Matches liquid assets, excluding inventory, to current liabilities. A more stringent measure of immediate solvency, especially when inventory turnover is slow.
#####	35	Interest Expense Ratio: Relates interest expenses to total revenue. Useful for understanding the relative burden of interest costs in comparison to sales revenue.
#####	36	Total debt/Total net worth: Demonstrates the relationship between a company's total debt and its total net worth. Critical for gauging financial leverage and risk.
#####	37	Debt ratio %: Represents the proportion of assets funded by debt. It provides insights into the company's dependency on external financing versus equity.
#####	38	Net worth/Assets: Compares net worth to total assets. Useful for determining the degree to which a company's assets are financed by equity.
#####	39	Long-term fund suitability ratio (A): It assesses the appropriateness of long-term funds in relation to the company's needs. Essential for long-term financial planning and stability.
#####	40	Borrowing dependency: Quantifies the company's reliance on borrowed funds for its operations. Highlights potential financial vulnerabilities and the risk exposure from debt.
#####	41	Contingent liabilities/Net worth: Contrasts potential future obligations with the company's current net worth. It's pivotal for assessing potential risks against the current value of the company.
#####	42	Operating profit/Paid-in capital: Relates the profit from primary operations to the initial capital invested by shareholders. Provides insights into the return on the initial investment from core operations
#####	43	Net profit before tax/Paid-in capital: Compares the pre-tax net profit to the capital initially invested by shareholders. Essential for understanding the profitability before tax relative to the original investment.
#####	44	Inventory and accounts receivable/Net value: Relates the sum of inventory and accounts receivable to the company's net value. Useful for assessing liquidity and the efficiency of asset management.
#####	45	Total Asset Turnover: Measures how effectively the company uses its assets to generate sales. A higher ratio indicates better asset utilization.
#####	46	Accounts Receivable Turnover: Evaluates the frequency with which the company collects its receivables. Useful for understanding the efficiency of credit sales collection.
#####	47	Average Collection Days: Represents the average number of days it takes for the company to receive payments for its credit sales. Indicates the speed of cash inflow from customers.
#####	48	Inventory Turnover Rate (times): Indicates how often inventory is sold and replaced during a period. Useful for understanding stock management efficiency.
#####	49	Fixed Assets Turnover Frequency: Measures how efficiently fixed assets are used to generate sales. Pivotal for companies with significant investments in fixed assets.
#####	50	Net Worth Turnover Rate (times): Assesses how effectively a company's net worth is used to generate sales. Reflects efficiency and financial health.
#####	51	Revenue per person: Denotes the revenue generated per employee. It's useful for gauging operational efficiency and labor productivity.
#####	52	Operating profit per person: Relates operating profit to the number of employees. Offers insights into labor profitability.
#####	53	Allocation rate per person: Represents the allocation of resources per employee, giving insights into resource distribution and efficiency.
#####	54	Working Capital to Total Assets: Measures the proportion of working capital to total assets. Indicates the company's operational liquidity relative to its size.
#####	55	Quick Assets/Total Assets: Compares the most liquid assets to total assets. Useful for evaluating immediate solvency in relation to the company's size.
#####	56	Current Assets/Total Assets: Demonstrates the proportion of assets that are expected to be converted into cash within a year relative to all assets. Indicates liquidity and short-term financial health.
#####	57	Cash/Total Assets: Highlights the proportion of cash in hand to total assets. A vital metric for understanding liquidity and potential growth opportunities.
#####	58	Quick Assets/Current Liability: Contrasts the most liquid assets with current liabilities. Reflects the company's ability to meet short-term obligations without relying on inventory sales.
#####	59	Cash/Current Liability: Matches cash reserves with current liabilities. Essential for gauging the immediate ability to pay off short-term debts.
#####	60	Current Liability to Assets: Measures the proportion of current liabilities to total assets. Indicates potential financial vulnerabilities and solvency concerns.
#####	61	Operating Funds to Liability: Assesses the relationship between funds from operations and liabilities. Useful for understanding the company's capacity to service its debts from core operations.
#####	62	Inventory/Working Capital: Compares inventory value to working capital. Provides insights into inventory management and its potential impact on liquidity.
#####	63	Inventory/Current Liability: Relates inventory to current liabilities. Essential for understanding potential liquidity challenges, especially if inventory turnover is slow.
#####	64	Current Liabilities/Liability: Measures the proportion of short-term debts to total liabilities. Indicates the company's short-term financial obligations in relation to its total debt.
#####	65	Working Capital/Equity: Compares working capital, which indicates operational liquidity, to shareholder's equity. Provides insights into the company's reliance on equity to finance its short-term operations.
#####	66	Current Liabilities/Equity: Demonstrates the proportion of current liabilities to equity. A high ratio may indicate higher financial risk.
#####	67	Long-term Liability to Current Assets: Contrasts long-term debts with assets expected to be converted into cash within a year. Pivotal for understanding potential long-term financial burdens against short-term asset liquidity.
#####	68	Retained Earnings to Total Assets: Compares accumulated profits not distributed to shareholders with total assets. Reveals how much of the company's assets are financed by undistributed profits.
#####	69	Total income/Total expense: Relates total revenue to total expenses. Essential for understanding profitability and operational efficiency.
#####	70	Total expense/Assets: Compares total expenses to total assets. Provides insights into cost management relative to the size of the company.
#####	71	Current Asset Turnover Rate: Measures how efficiently current assets are used to generate sales. Reflects short-term asset utilization.
#####	72	Quick Asset Turnover Rate: Assesses the efficiency of the company's most liquid assets in generating sales. Highlights immediate asset efficiency without the influence of inventory.
#####	73	Working capital Turnover Rate: Indicates how efficiently the company uses its working capital to generate sales. Reflects operational liquidity and efficiency.
#####	74	Cash Turnover Rate: Measures the frequency with which a company uses its cash to generate sales. Pivotal for companies that prioritize liquid assets.
#####	75	Cash Flow to Sales: Relates cash flow from operations to sales revenue. Indicates the company's ability to convert sales into cash.
#####	76	Fixed Assets to Assets: Demonstrates the proportion of fixed assets to total assets. Useful for gauging the significance of long-term assets in the company.
#####	77	Current Liability to Liability: Measures the proportion of short-term obligations to total liabilities. Provides insights into the company's short-term financial commitments relative to its total debt.
#####	78	Current Liability to Equity: Contrasts current liabilities with shareholders' equity. Indicates the degree of financial risk related to short-term obligations.
#####	79	Equity to Long-term Liability: Compares shareholders' equity to long-term debts. Essential for understanding the company's long-term financial stability.
#####	80	Cash Flow to Total Assets: Matches cash flow from operations to total assets. Provides insights into how efficiently the company converts its assets into cash.
#####	81	Cash Flow to Liability: Relates cash flow from operations to total liabilities. Indicates the company's ability to service its debts from operational cash flow.
#####	82	CFO to Assets: Compares cash flow from operations (CFO) to total assets. Highlights the efficiency of assets in generating operational cash.
#####	83	Cash Flow to Equity: Relates operational cash flow to shareholders' equity. Provides insights into the return on equity from cash flow.
#####	84	Current Liability to Current Assets: Contrasts short-term obligations with assets expected to be converted into cash within a year. Indicates liquidity and the ability to meet short-term financial commitments.
#####	85	Liability-Assets Flag: A binary indicator signaling if total liabilities exceed total assets. If the value is '1', it indicates potential solvency issues, while '0' means assets exceed liabilities.
#####	86	Net Income to Total Assets: Compares net income to total assets. Reflects the efficiency of asset utilization in generating profits.
#####	87	Total assets to GNP price: Relates the company's total assets to the Gross National Product price. Useful for understanding the company's size relative to the nation's economy.
#####	88	No-credit Interval: Indicates the time duration in which the company operates without relying on external credit. Highlights the company's financial independence and liquidity.
#####	89	Gross Profit to Sales: Measures the ratio of gross profit to sales revenue. Provides insights into the company's profitability before deducting operational expenses.
#####	90	Net Income to Stockholder's Equity: Contrasts net income with shareholder's equity. Offers insights into the return on equity.
#####	91	Liability to Equity: Demonstrates the relationship between the company's total liabilities and shareholder's equity. Reveals the degree of financial leverage and risk.
#####	92	Degree of Financial Leverage (DFL): Quantifies the sensitivity of the company's earnings per share (EPS) to changes in its operating income. Indicates the potential volatility of earnings due to the structure of financing.
#####	93	Interest Coverage Ratio (Interest expense to EBIT): Measures the company's ability to cover interest expenses with its earnings before interest and taxes (EBIT). Indicates solvency and risk of default.
#####	94	Net Income Flag: A binary indicator denoting the presence (value of '1') or absence (value of '0') of net income. It alerts stakeholders to the company's profitability status.
#####	95	Equity to Liability: Contrasts shareholder's equity with total liabilities. Provides insights into the company's financial stability and reliance on external financing


### Label (Bankruptcy):
Bankruptcy Status (1: Went Bankrupt, 0: Did not go bankrupt)

### Data Splitting
The data is divided into three sets and uploaded:

Training set (60%): Used to train our neural network model. (train_dataset.csv)

Validation set (20%): To tune the model parameters and prevent overfitting. (valid_dataset.csv)

Test set (20%): To evaluate the model's performance on unseen data. (test_dataset.csv)

