# Smart India Hackathon Workshop
# Date: 11-11-2026
## Reference Number: 26000807
## Name: Tejaswini T

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
ReverseMandi is a demand-led farm marketplace that connects Farmer Producer Organizations (FPOs) with nearby consumers and bulk buyers. It brings buyer requirements, FPO produce listings and shared logistics together so sellers can compare offers and estimated costs before dispatch.

Small buyers—including apartment societies, shops, hostels and community kitchens—can combine compatible requirements by location and delivery date. FPOs can respond to buyer requests with offers that show the price and estimated costs, such as packing, transport and platform charges. This helps FPOs compare expected net returns before accepting an order. Local market prices may be shown for reference, but they are not guaranteed.

Buyers can post upcoming needs, while FPOs list expected harvest quantities and dates. This planning view can help FPOs organize collection and communicate likely demand to members. Forecasts are estimates, not confirmed orders, and any forward commitment must state its quantity, price and cancellation terms.

The platform can also support shared pickup and delivery planning, including route suggestions. FPOs and transporters confirm the final logistics plan. Completed orders record agreed prices, fees, logistics costs and delivery details, helping buyers and FPOs track transactions.

Order records may support a future integration with authorized lenders, subject to FPO consent and lender checks. Financing is outside the initial prototype, and credit is not guaranteed. ReverseMandi’s proposed distinction is its combined workflow for demand pooling, offer comparison, harvest planning, logistics and transaction records. Its usefulness and distinctiveness should be validated against existing platforms before claiming it is unique.


## Technical Approach
Technologies
- Apps: React Native or Flutter for FPOs and buyers; React web portal for FPO operations.
- Access: Local-language interface and FPO-assisted listings. WhatsApp or IVR may be added through an authorized provider.
- Backend and data: FastAPI or Node.js with PostgreSQL and PostGIS.
- Demand planning: Group compatible buyer requests by crop, quantity, location and delivery window. Start with historical averages and seasonal patterns; consider advanced forecasting when reliable data is available.
- Logistics: OpenStreetMap and a routing tool such as OR-Tools to suggest routes for dispatcher or FPO approval.
- Trust and integrations: Crop-specific listing details, photos, weight records and issue resolution. Use documented APIs and modular adapters to explore ONDC or e-NAM integrations, subject to access and approvals.
- Payments and hosting: Track payment status and use a provider sandbox in the prototype; a payment partner handles live payments. Use cloud hosting suited to the team, with role-based access, encryption, backups and audit records.
- Data: Use pilot transactions and permitted public market information, documenting external sources.

## Feasibility and Viability
The prototype can use established tools for produce listings, offers, order records, location-based demand grouping and basic route suggestions. Reliable forecasting will need more transaction data, so early estimates should remain simple and clearly labeled.

A pilot will depend on participating FPOs, repeat buyers and transport providers. Start in one district with one or two FPOs, a few buyers and two or three crops. Possible revenue models include transaction, buyer subscription or logistics coordination fees; validate these with users before relying on them. Integrations with e-NAM, ONDC, payment providers or lenders depend on partner access and approvals.
Challenges and responses
Low digital literacy, limited trust and low order volumes could make demand pools difficult to sustain. FPO staff or local facilitators can support onboarding, while the pilot begins with a small group of recurring buyers and sellers. Confirm pooled orders only when everyone agrees on quantity, price and delivery terms.

Harvest estimates may be wrong, and produce quality, cancellations, payment delays and transport costs can create disputes. Label forecasts as estimates, use consistent listing fields, and record quality, delivery, cancellation and payment terms before confirming orders. Track actual logistics costs and fulfillment results before expanding.

Collect only the data needed for the pilot and explain who can access it. Treat external platform, payment and lending integrations as future possibilities until access and approvals are secured.
## Impact and Benefits
Farmers and FPOs could gain better visibility into buyer needs and competing offers, compare expected proceeds after disclosed costs, and keep records of agreed terms. Consumers and institutions could discover produce from participating FPOs, while small buyers may benefit from pooled orders and bulk buyers can specify quantities, quality and delivery needs more clearly.

Aggregated reports may help government and market stakeholders understand transactions completed through the platform, subject to data-sharing arrangements.
Expected benefits
The platform may improve farmer net realization or reduce buyer costs if better matching and pooled logistics reduce avoidable expenses. FPO-assisted onboarding could help farmers who need support using digital tools, and local collection or packing may create work where demand allows. Better route planning could reduce unnecessary travel or delays. These economic, social and environmental benefits should be measured during the pilot rather than assumed.
Pilot measures
Track farmer and FPO proceeds after costs, buyer landed cost for comparable orders, time to confirm orders, and the share delivered in full and on time. Also record rejected or damaged produce, vehicle use, estimated versus actual delivery distance, repeat use, and feedback from farmers, FPOs and buyers.
## Research and References
Remove These Lines
• e-NAM, FPO trading: https://enam.gov.in/stakeholders-Involved/fpos
• RBI, “Agriculture Supply Chain Dynamics: Evidence from Pan-India Survey” (2024): https://www.rbi.org.in/Scripts/BS_ViewBulletin.aspx?Id=22326
• Agmarknet, agricultural market prices: https://agmarknet.gov.in
• SFAC, Farmer Producer Organizations: https://www.sfacindia.com/FPOS.aspx
• Google OR-Tools, route optimization: https://developers.google.com/optimization/routing
