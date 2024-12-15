# Nifty50 Stock Analysis Dashboard

![et-analysis-stocks-excluded-from-nifty-50-outperform-those-included](https://github.com/user-attachments/assets/79b9af1c-2a19-4209-8268-7e23c46e4708)


The Stock Price Analysis Dashboard is a powerful tool designed to visualize and analyze trading data for various equities. Leveraging a structured dataset, this dashboard provides key insights into stock performance over multiple trading sessions. This dataset includes vital details such as the opening and closing prices, daily highs and lows, trading volumes, deliverable volumes, and the volume-weighted average price (VWAP).

By incorporating trends from daily trades and deliverables, the dashboard enables traders, analysts, and investors to make informed decisions. It also highlights changes in stock behavior, including significant price fluctuations and market activity patterns. This tool is an essential resource for tracking stock performance and identifying opportunities in dynamic financial markets.

## Dataset Description

[Dataset Source](https://www.kaggle.com/datasets/rohanrao/nifty50-stock-market-data)

The dataset contains detailed trading information for various equities (EQ) over multiple trading sessions. It provides a comprehensive view of stock performance, covering a variety of critical metrics and enabling in-depth analysis of market trends, trading activity, and price movements. Below is a holistic breakdown of the dataset:

**Dataset Columns**
 - **Symbol:** The ticker symbol representing the equity being traded.
 - **Series:** Indicates the market series for the equity, which is "EQ" (Equity).
 - **Previous Close:** The closing price of the stock from the previous trading session, serving as a reference point for the current day.
 - **Open:** The price at which the stock started trading for the day.
 - **High:** The highest price the stock reached during the trading session.
 - **Low:** The lowest price the stock reached during the trading session.
 - **Last:** The last traded price of the stock before the market closed.
 - **Close:** The official closing price of the stock at the end of the trading session.
 - **VWAP (Volume-Weighted Average Price):** A critical metric that reflects the average price of the stock weighted by the total trading volume during the session.
 - **Volume:** The total number of shares traded during the session, indicating liquidity and market activity.
 - **Trades:** The number of individual transactions that occurred during the trading session.
 - **Deliverable Volume:** The number of shares out of the total volume that were marked for delivery (actual transfer of shares post-trade), representing long-term interest in the stock.
 - **Deliverables:** A ratio of the deliverable volume to the total traded volume, expressed as a fraction or percentage. This indicates the proportion of trades intended for actual settlement versus speculative trading.

## Dashboard

![Eleastic_dashboard](https://github.com/user-attachments/assets/d7b016c9-634e-4ca9-b661-2ac1606e24dd)

**Applications of the Dashboard**
 - **Trading Strategy Development:** Build trading strategies based on volatility, liquidity, and volume metrics.
   
 - **Investment Decisions:** Use deliverable volume ratios to identify stocks with high investor interest.
   
 - **Market Sentiment Analysis:** Assess trends over time to infer market sentiment and predict future performance.
   
 - **Quantitative Modeling:** Use historical data to develop predictive models for stock price and volume movements.

The **video below** highlights the dynamic and interactive capabilities of a dashboard developed using the ELK Stack (Elasticsearch, Logstash, and Kibana). It emphasizes how users can leverage a range of controls and filters to interact with the dataset in real time, making data exploration intuitive and efficient.

By applying various filters—such as timestamps to focus on specific periods, geographic states for regional insights, and subcategories for granular analysis—the dashboard instantly updates to display data that matches the selected criteria. These filters ensure that users can narrow down vast datasets to pinpoint relevant information effortlessly.

The dashboard incorporates user-friendly controls, including dropdown menus for quick selection, sliders for precise adjustments, and other interactive elements that allow for seamless customization. This ensures that users can tailor the dashboard view to their unique analytical needs without requiring technical expertise.

Such interactive approach empowers users to explore data from multiple dimensions, uncover patterns, and derive actionable insights. By simplifying complex data queries and visualization, the dashboard becomes a robust tool for informed, data-driven decision-making across various use cases and industries.

[Elastic.webm](https://github.com/user-attachments/assets/f0715d79-625a-4902-b97f-a3f9e70a912c)

## Dasboard Analysis

1. How do the average low and high prices fluctuate over short time intervals?

**Price Trends Over Time**
   
This graph shows the trend of average low prices (green) and average high prices (blue) over time. The x-axis represents timestamps at 10-second intervals, and the y-axis indicates price values.

Initially, there is a sharp increase in both average low and high prices, peaking around 12:30.

After the peak, prices begin to show volatility, experiencing multiple drops and recoveries throughout the observed period.

Towards the end, prices trend downward, indicating a potential correction or reduced market activity.

**Insight:** This graph helps identify short-term price trends and volatility, highlighting rapid changes in stock performance over time.

![ELK 1](https://github.com/user-attachments/assets/1c129a68-4b27-403d-85d4-e498bf5ef1da)

<br>

2. What is the trading volume distribution across different 3-minute intervals?

**Trading Volume Analysis**

This bar chart visualizes the trading volume for each 3-minute interval. The x-axis shows the timestamp at 3-minute intervals, and the y-axis represents the value of volume traded.

The trading volume starts at a moderately high level around 12:30 and peaks between 12:33–12:39, indicating heightened trading activity.

Post-12:40, there is a significant drop in volume, suggesting reduced market participation or lower activity during this period.

**Insight:** This graph highlights periods of peak trading activity, which could help pinpoint significant market events, announcements, or active participation windows.

![ELK 2](https://github.com/user-attachments/assets/8693b9ef-e680-472f-a4d2-21db2cd7b73b)

<br>

3. What is the trend of deliverable volumes over 5-minute intervals?

**Deliverable Volume Percentage**

This horizontal bar chart displays the value of deliverables (deliverable percentage) at 5-minute intervals. The y-axis represents timestamps, while the x-axis shows the value of deliverables.

At 12:30, the deliverable percentage is the highest.

Between 12:35–12:40, the deliverable percentage decreases but remains significant.

At 12:45 and 12:50, the values show a slight recovery but remain lower compared to earlier intervals.

**Insight:** This graph reveals the distribution of deliverable volumes, indicating how much of the traded stock was delivered. High deliverable percentages can reflect investor confidence or long-term holding patterns, while lower percentages may indicate speculative trading.

![ELK 3](https://github.com/user-attachments/assets/639d97f5-5376-41a5-920a-e916dd9cf8a4)

<br>

4. How do deliverable volumes change over time, and what patterns can be observed in the moving average?

**Moving Average of Volume Deliverables**

This bar chart shows the moving average of deliverable volumes over time, with the x-axis representing timestamps (per minute) and the y-axis indicating the moving average count of deliverables.

The deliverable volume starts relatively low around 12:30 and steadily increases over time, reaching stability at higher levels after 12:35.

Minor fluctuations are observed toward the end, but overall the values remain consistently high.

**Insight:** The graph highlights a trend of gradual improvement in deliverable volumes over time, suggesting increasing market participation or confidence as the session progresses.

![ELK 4](https://github.com/user-attachments/assets/53ed9be2-d5fe-4f61-a0cd-624049d3022e)

<br>

5. How are the open prices correlated with the median close prices?

**Open vs Close Price Correlation**

This graph visualizes the relationship between open prices and close prices using vertical lines to depict the correlation. The x-axis represents the open price, and the y-axis indicates the median of close prices.

As the open price increases, the median of close prices also tends to rise, showing a positive correlation.

The graph highlights consistent behavior, with most data points showing close prices trailing open prices in an expected pattern.

**Insight:** This graph confirms a strong positive correlation between open and close prices. It suggests that stocks tend to close higher or at levels proportional to their open price.

![ELK 5](https://github.com/user-attachments/assets/3cd05c40-0f09-4537-9936-6dcae96a43bf)

<br>

6. How do average low prices vary across time, and what role do price ranges play?

**Average Price Range Analysis**

This line graph displays average low prices over 5-minute intervals with color-coded price ranges (indicated by the legend on the right).

At the beginning (12:30), average low prices start high but quickly drop across most price ranges.
Between 12:35–12:40, prices stabilize and show convergence around a common range.

Post-12:45, the average low prices begin to diverge again, suggesting volatility across multiple price ranges.

**Insight:** This graph helps in identifying price movements over short intervals and highlights periods of convergence and divergence among different price ranges, which can indicate changing market dynamics.

![ELK 6](https://github.com/user-attachments/assets/439e478e-e0b2-4e7a-9682-f357b44cf0d1)

<br>

7. How does the median closing price relate to the highest and lowest closing prices observed in the dataset? Are there outliers influencing the mean significantly compared to the median?

**Median of Close**

This graph displays the median of the closing prices of the stock over the dataset's time period, which is 573.75.

The median value is accompanied by the median volume, which is 522,809. This represents the middle value of trading volumes, indicating a typical level of trading activity without being skewed by extremely high or low values.

In the dataset, the close prices range from 436 to 1,102.4, making the median a central and more reliable measure for summarizing stock performance.

![ELK 7](https://github.com/user-attachments/assets/f9a3b0e0-2150-4f62-b729-cb1aadbce3d0)

<br>

8. Is there a trend in the deliverable percentage over time? Does it increase during periods of higher volume or closing price volatility?

**Deliverables Gauge**

This gauge graph focuses on the average deliverables, which is 0.287 (or 28.7% of the total traded volume). Deliverables measure the percentage of shares delivered for settlement compared to the total shares traded.

A low deliverable percentage indicates more speculative trading (e.g., intraday trades or high liquidity without long-term holding intent).

The benchmark of 0.5 suggests that the deliverable percentage is significantly lower than what might be expected for a stock with long-term investor interest.

![ELK 8](https://github.com/user-attachments/assets/c682f104-e63a-4ba5-83c2-05d557ccb9b8)

<br>

9. How frequently does the closing price reach or exceed the upper benchmark of 750, and what factors (e.g., volume or market trends) contribute to these occurrences?

**Closing Price Benchmarking**

This bar graph compares the closing price of 436 against a range benchmark of 0–750. The closing price falls below the midpoint of the range (375), suggesting relatively weaker performance compared to a defined upper benchmark.

When compared to the dataset, the closing price of 436 is significantly lower than the maximum closing price (1,102.4). The benchmark graph helps visualize how the stock performs within a predefined range.

![ELK 9](https://github.com/user-attachments/assets/0f1d98fd-8db9-42a4-88f3-9361421e79dd)

<br>

10. What factors may be contributing to the observed fluctuations in the deliverable volume share over time, and how could this information be used to inform trading strategies or market analysis?

**Deliverable Volume Share**

The deliverable volume share fluctuates significantly across the trading days, ranging from around 0.15% to over 0.60%.

There appear to be periods of relatively higher deliverable volume share, such as the range between 0.40% and 0.60%, as well as periods of lower deliverable volume share, below 0.30%.

The graph provides a visual representation of the variability in the deliverable volume share, which could be useful for understanding trading patterns and liquidity for the stock.

![ELK 10](https://github.com/user-attachments/assets/a84f436b-c998-4beb-aa10-2d9c95fc8c11)

<br>

**Summary of Insights:**

 - **Price Trends:** Identify fluctuations in average price trends and volatility over short intervals.
 - **Trading Volume:** Highlight intervals with peak and declining trading activity.
 - **Deliverable Volume:** Assess periods where deliverable volumes are higher or lower, providing insights into investor sentiment.
 - **Moving Average of Volume Deliverables:** Gradual and stable increase in deliverable volumes over time indicates rising market participation.
 - **Open vs Close Price Correlation:** A strong positive correlation between open and close prices shows price consistency.
 - **Average Price Range Analysis:** Price trends display early volatility, followed by stabilization and subsequent divergence, signaling market fluctuations.
 - **Median of Close:** The median closing price of the stock is 573.75, which represents a central and more reliable measure of stock performance compared to the full range of closing prices from 436 to 1,102.4.
 - **Deliverables Gauge:** The average deliverables, or the percentage of shares delivered for settlement compared to the total shares traded, is 28.7%, which is significantly lower than the benchmark of 50%, suggesting more speculative trading activity.
 - **Closing Price Benchmarking:** The closing price of 436 falls below the midpoint of the defined range of 0-750, indicating relatively weaker performance compared to the upper benchmark, which the stock has only reached occasionally based on the data.
 - **Deliverable Volume Share:** The deliverable volume share exhibits significant fluctuations, ranging from around 0.15% to over 0.60%, indicating variable trading patterns and liquidity for the stock.

## Managerial Insights

 - Closely monitor short-term price volatility and fluctuations in average low and high prices to identify potential market opportunities or risks.
   
 - Analyze trading volume patterns across 3-minute intervals to pinpoint periods of heightened market activity, which could signal important events or investor sentiment shifts.
   
 - Examine the trend and distribution of deliverable volumes over time to gauge the level of long-term investor interest versus speculative trading activity.
   
 - Utilize the moving average of deliverable volumes to identify gradual improvements in market confidence and participation.
   
 - Leverage the positive correlation between open and close prices to anticipate potential price movements and develop more effective trading strategies.
   
 - Assess average price range variations to understand evolving market dynamics and identify periods of convergence and divergence, which could inform risk management and hedging decisions.

## Conclusion

The comprehensive dataset provides various insights that can inform various managerial decisions and trading strategies. By analyzing price trends, trading volumes, deliverable volumes, and the relationship between open and close prices, managers can gain a deeper understanding of the stock's performance, market sentiment, and investor behavior. These insights can be used to identify opportunities, mitigate risks, and optimize trading activities. Additionally, the benchmarking and comparison tools, such as the median closing price and the deliverables gauge, offer valuable context for evaluating the stock's positioning within the market. Ultimately, this multifaceted analysis enables managers to make more informed and data-driven decisions to enhance the overall performance and strategic positioning of the business.
