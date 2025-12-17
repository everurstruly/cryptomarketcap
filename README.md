# ThatCoinmarketcap: Real-Time Market Data Visualization

A React-based dashboard application that connects to live cryptocurrency data feeds. This project focuses on building a responsive interface that consumes and visualizes high-frequency real-time data, while integrating user-specific features through a backend service. The goal is to demonstrate practical full-stack development skills by combining external APIs, real-time state management, and persistent user data in a single, cohesive application.

---

## Purpose and Focus

*   **Connecting to and managing live data streams** from a production WebSocket API, handling connection states, errors, and reconnection logic.
*   **Processing and displaying high-frequency data updates** efficiently in a React interface, using state management techniques to ensure UI responsiveness.
*   **Implementing standard financial data visualizations**—including a live price ticker, an order book, and an interactive chart—that form the core of trading and analytics platforms.
*   **Integrating a backend-as-a-service (Firebase)** to move beyond a static frontend, adding features like user-specific data persistence and real-time collaborative features that sync across all connected clients.

---

## Core Features

### 1. Asset List and Ticker
This component acts as the primary navigation and overview for the dashboard. It displays a continuously updated list of cryptocurrency pairs, providing a live snapshot of market movements. Users can interact with this list to drill down into specific assets, driving the data displayed in all other components.

*   **Live Price**: The latest price for each asset, updating directly from the data feed.
*   **24-Hour Change**: A visual indicator showing whether the price is up or down over the past day.
*   **Interactive Selection**: Clicking on any asset will populate the other dashboard components with its specific data.
*   **User Watchlists**: Users can star their favorite assets. This personalized list is saved to a database and syncs across browsing sessions.

### 2. Order Book
The order book visualizes market depth, representing the current balance of supply and demand for a selected asset. It provides a transparent view of the pending buy and sell orders in the market, which is critical information for understanding immediate price pressure and liquidity.

*   **Market Depth Chart**: A two-sided display showing the top 15 active buy orders (bids) and sell orders (asks) in the market, along with their volumes.
*   **Live Updates**: The order book updates in real-time as new orders are placed and filled.
*   **Bid/Ask Spread**: A clear visualization of the difference between the highest current buy price and the lowest current sell price.

### 3. Interactive Price Chart
This chart provides historical context for price movements. It transforms a raw stream of trade data into a visual narrative of market activity, allowing users to see trends and patterns over different timeframes for the selected cryptocurrency pair.

*   **Historical and Live Data**: The chart loads past price data and then updates in real-time with new trades.
*   **Candlestick Format**: Prices are shown using candlestick bars, a standard format that displays the opening, closing, high, and low price for a given time period.

### 4. User and Collaboration
This suite of features extends the dashboard from a passive display into an interactive, shared application. It demonstrates how to layer user-specific functionality and real-time collaboration on top of a public data stream, showcasing full-stack application logic.

*   **Live Price Triggers**: Users can set simple price targets for assets on their watchlist (e.g., "Alert me if Bitcoin exceeds $90,000"). This logic runs in the browser, and when triggered, creates a prominent visual notification within the dashboard.
*   **Live Viewers Counter**: A display showing the number of users currently viewing the dashboard, updated in real-time.
*   **Shared Market Sentiment**: A simple widget where users can vote "Bullish" or "Bearish" on an asset and see the aggregated, live results from all current users.

---

**Success Criteria:**
1. See live cryptocurrency prices updating in a table
2. Select assets to view their order book and price chart
3. Star favorites that persist across sessions
4. See how many other users are currently viewing the dashboard