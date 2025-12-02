# Zerodha
Please try to implement the project on your own before proceeding to the lectures &amp; code.
Project Architecture & Flow
Overview
This project is a clone of the Zerodha trading platform, consisting of three main components:

Frontend (/frontend): The public-facing marketing website.
Dashboard (/dashboard): The logged-in trading interface (Kite clone).
Backend (/backend): The API server that powers the dashboard.
Component Roles
1. Frontend (/frontend)
Role: This is the landing page and marketing site where users learn about the platform.
Tech Stack: React.js, Bootstrap.
Key Pages:
Home: Hero section, awards, stats.
Signup: Entry point for new users.
About, Products, Pricing, Support: Informational pages.
Flow: Users visit this site first. Clicking "Signup" or "Login" (conceptually) would take them to the Dashboard.
2. Dashboard (/dashboard)
Role: This is the core trading application where users manage their portfolio.
Tech Stack: React.js.
Key Features:
Watchlist: Real-time stock prices.
Holdings: Long-term investments.
Positions: Intraday trades.
Orders: Buy/Sell interface.
Funds: Account balance management.
Flow: This app fetches data from the Backend API to display holdings, positions, and execute trades.
3. Backend (/backend)
Role: The server-side application that handles data persistence and business logic.
Tech Stack: Node.js, Express, MongoDB (Mongoose).
Key Endpoints:
GET /allHoldings: Fetches user's long-term holdings.
GET /allPositions: Fetches current open positions.
POST /newOrder: Places a new buy/sell order.
Flow: It connects to a MongoDB database to store and retrieve trade data, serving it to the Dashboard.
Overall User Flow
Visitor: Lands on frontend (port 3000/3001).
Action: Decides to trade -> Navigates to dashboard (port 3000/3001).
Trading:
User views Holdings -> Dashboard calls GET /allHoldings from Backend.
User places an Order -> Dashboard calls POST /newOrder to Backend.
Backend saves order to MongoDB.
Directory Structure
frontend/: React app for marketing pages.
dashboard/: React app for the trading UI.
backend/: Node.js API server connected to MongoDB.
 to resemble a link, use a button and change it with appropriate styles. Learn more: https://git
hub.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anch
or-is-valid
  Line 221:11:  The href attribute requires a valid value to be accessible. Provide a valid, nav
igable address as the href value. If you cannot provide a valid href, but still need the element
 to resemble a link, use a button and change it with appropriate styles. Learn more: https://git
hub.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anch
or-is-valid
  Line 225:11:  The href attribute requires a valid value to be accessible. Provide a valid, nav
igable address as the href value. If you cannot provide a valid href, but still need the element
 to resemble a link, use a button and change it with appropriate styles. Learn more: https://git
hub.com/jsx-eslint/eslint-plugin-jsx-a11y/blob/HEAD/docs/rules/anchor-is-valid.md  jsx-a11y/anch
or-is-valid
 
webpack compiled with 1 warning
 # zerodha
