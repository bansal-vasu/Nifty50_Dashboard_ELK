# Nifty50 Stock Analysis Dashboard

![et-analysis-stocks-excluded-from-nifty-50-outperform-those-included](https://github.com/user-attachments/assets/79b9af1c-2a19-4209-8268-7e23c46e4708)


The Stock Price Analysis Dashboard is a powerful tool designed to visualize and analyze trading data for various equities. Leveraging a structured dataset, the dashboard provides key insights into stock performance over multiple trading sessions. This dataset includes vital details such as the opening and closing prices, daily highs and lows, trading volumes, deliverable volumes, and the volume-weighted average price (VWAP).

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

**Dashboard**

![Eleastic_dashboard](https://github.com/user-attachments/assets/d7b016c9-634e-4ca9-b661-2ac1606e24dd)

The **video below** highlights the dynamic and interactive capabilities of a dashboard developed using the ELK Stack (Elasticsearch, Logstash, and Kibana). It emphasizes how users can leverage a range of controls and filters to interact with the dataset in real time, making data exploration intuitive and efficient.

By applying various filters—such as timestamps to focus on specific periods, geographic states for regional insights, and subcategories for granular analysis—the dashboard instantly updates to display data that matches the selected criteria. These filters ensure that users can narrow down vast datasets to pinpoint relevant information effortlessly.

The dashboard incorporates user-friendly controls, including dropdown menus for quick selection, sliders for precise adjustments, and other interactive elements that allow for seamless customization. This ensures that users can tailor the dashboard view to their unique analytical needs without requiring technical expertise.

Such interactive approach empowers users to explore data from multiple dimensions, uncover patterns, and derive actionable insights. By simplifying complex data queries and visualization, the dashboard becomes a robust tool for informed, data-driven decision-making across various use cases and industries.

[Elastic.webm](https://github.com/user-attachments/assets/f0715d79-625a-4902-b97f-a3f9e70a912c)

