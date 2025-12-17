# Development Roadmap (2-Week Timeline)

## Week 1 — Core Data & Display
**Goal:** Functional dashboard displaying live Bitfinex data.

- [ ] **Project Setup**
    - [ ] Initialize React/TypeScript project
    - [ ] Install core libraries (charting, UI, Firebase)
    - [ ] Set up project structure and routing

- [ ] **Bitfinex Integration**
    - [ ] Create WebSocket service manager
    - [ ] Implement connection/reconnection logic
    - [ ] Subscribe to `ticker` channel for 5-7 major pairs

- [ ] **Core Dashboard Components**
    - [ ] Build Asset Ticker Table with live prices
    - [ ] Implement price change indicators (color/arrows)
    - [ ] Create basic chart displaying price history
    - [ ] Add asset selection functionality

- [ ] **Basic UI/UX**
    - [ ] Implement responsive dashboard layout
    - [ ] Add loading/error states
    - [ ] Style core components

## Week 2 — Firebase Features & Polish
**Goal:** Add user features and deploy a presentable application.

- [ ] **Firebase Integration**
    - [ ] Set up Firebase project and configuration
    - [ ] Implement anonymous authentication
    - [ ] Create Firestore structure for user data

- [ ] **User Features**
    - [ ] Build watchlist functionality (star/save assets)
    - [ ] Implement Live Viewers counter
    - [ ] Add simple visual price triggers (UI-only alerts)

- [ ] **Advanced Components**
    - [ ] Build Order Book for selected asset
    - [ ] Enhance chart with real-time updates
    - [ ] Add Shared Sentiment widget (bullish/bearish votes)

- [ ] **Final Polish & Deployment**
    - [ ] Optimize performance (throttle rapid updates)
    - [ ] Complete responsive design
    - [ ] Deploy to Vercel/Netlify
    - [ ] Document setup and features

---

**Success Criteria:**
1. See live cryptocurrency prices updating in a table
2. Select assets to view their order book and price chart
3. Star favorites that persist across sessions
4. See how many other users are currently viewing the dashboard
