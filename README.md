Submission Document – Trade Flow (B2B Marketplace)
a) Problem Statement Reference

Problem Statement Chosen:
Small retailers face difficulties in sourcing bulk products due to fragmented offline channels. Suppliers also lack a unified platform to reach many retailers efficiently.

Reason to Choose the Problem Statement:
The wholesale and retail ecosystem is shifting online. With global B2B marketplace sales projected to reach $3.6 trillion by 2024, there is a strong demand for a centralized, digital B2B procurement solution. Trade Flow addresses inefficiencies by modernizing the process for both suppliers and retailers.

b) Solution Overview

Proposed Approach (2–3 lines):
Build a digital B2B retail hub where suppliers upload and manage products, while retailers can discover, filter, and order in bulk. The platform integrates an AI-powered shopping assistant to improve decision-making and streamline sourcing.

Key Features / Modules:

Role-based accounts (Supplier / Retailer)

Supplier product management dashboard

Retailer product catalog with search & filters

Shopping cart system

AI-powered shopping assistant for queries & recommendations

Responsive, modern UI with fast navigation

c) System Architecture

Architecture Diagram / Workflow (Conceptual):

[Supplier / Retailer] 
       ↓
[React Frontend UI]
       ↓
[Application State / API Layer] → [AI Assistant API]
       ↓
[Cart Context / Local Storage / Future Database]


Data Flow Explanation:

Users select their role (Supplier/Customer).

Suppliers upload product details (stored in application state / backend).

Retailers browse catalog, search/filter, and add items to cart.

Cart context manages checkout flow.

AI Assistant processes queries and suggests products via AI API integration.

d) Technology Stack

Backend: Currently frontend-only prototype; future-ready for Node.js/Express.

Frontend: React + TypeScript, Vite bundler.

Databases: For prototype → Local storage & app state; future → SQL/NoSQL.

ML/AI Frameworks: AI Assistant API (integration-ready, e.g., OpenAI or Salesforce AI).

APIs / Libraries:

React Router (navigation)

React Context API & TanStack React Query (state & data)

Tailwind CSS & shadcn/ui (UI components)

Lucide React (icons)

e) Algorithms & Models

Algorithm(s) Chosen: Recommendation system (via AI chat assistant).

Reason for Choice: Helps retailers quickly identify suitable suppliers/products, improving engagement and sales conversions.

Model Training & Testing Approach:

Prototype → Uses external AI API for recommendations.

Future → Train custom recommendation models on user purchase history and supplier data.

f) Data Handling

Data Sources Used: Supplier product uploads, mock datasets (expandable to live APIs/datasets).

Preprocessing Methods: Product categorization, filtering, and rating normalization.

Storage / Pipeline Setup:

Prototype: In-browser state & local storage.

Future: Cloud DB (MongoDB/PostgreSQL) with pipelines for real-time updates.

g) Implementation Plan

Initial Setup & Environment: React + TypeScript project setup, Tailwind integration, routing configuration.

Core Module Development: Supplier dashboard, Retailer catalog, Cart system.

Integration & Testing: Add AI chat assistant, ensure cart & product management work seamlessly.

Final Deployment-ready Build: Optimize UI/UX, integrate backend & database, cloud deployment.

h) Performance & Validation

Evaluation Metrics:

User engagement (time on platform, AI assistant usage)

Conversion rate (cart additions → purchases)

Response time (UI interactions, AI assistant replies)

Testing Strategy:

Unit tests for components

Integration tests for workflows (login, product upload, cart)

User acceptance testing with demo retailers & suppliers

i) Deployment & Scalability

Deployment Plan:

Deploy frontend on Vercel/Netlify (prototype).

Future backend with Node.js/Express deployed on AWS/GCP with CI/CD pipelines.

Scalability Considerations:

Move from local state to cloud-based database.

API-based microservices for product, user, and order management.

AI recommendation model scaling with more user/product data.

Load balancing and CDN for global accessibility.
