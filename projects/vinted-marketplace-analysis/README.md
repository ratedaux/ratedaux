# 🛍️ Vinted Product Analytics Case Study

> An independent Product Analytics case study exploring buyer behavior, conversion, and potential friction points in the Vinted marketplace.

Project Status: 🟡 In Progress  
Project Type: Independent Portfolio Project  
Product: Vinted  
Focus: Product Analytics · User Behavior · UX · Conversion · Experimentation

---

## 📌 Project Overview

Vinted is a peer-to-peer marketplace where users can buy and sell second-hand items.

For this case study, I am exploring the buyer journey from discovering an item to completing a purchase, with a particular focus on understanding where users may lose interest or encounter friction.

The project combines:

- 🔎 Product and UX research
- 💬 Qualitative analysis of user feedback
- 📊 Product analytics
- 💻 SQL analysis
- 📈 Data visualisation
- 💡 Product recommendations
- 🧪 Experiment design

> Disclaimer: This is an independent portfolio project and is not affiliated with Vinted. Any quantitative dataset created for the analysis is simulated and does not represent Vinted's internal data.

---

## 🎯 Business Question

### How could Vinted improve the buyer journey and increase purchase conversion?

To explore this question, I will investigate:

- Where potential drop-offs occur in the buyer journey
- Which user actions may indicate purchase intent
- Where users may encounter friction
- How user behaviour may differ across segments
- Which product improvements could potentially increase conversion

---

## 🧭 User Journey

The initial buyer journey I am investigating is:

Discover → Search → View Item → Favorite / Message Seller → Checkout → Purchase → Repeat Purchase

I will refine this journey as I explore the product and gather evidence.

### Key Questions

- What motivates a user to move from browsing to purchasing?
- Why might a user favourite an item without buying it?
- At which stage might users lose purchase intent?
- What information or interaction could reduce uncertainty?
- Which behaviours could indicate a higher likelihood of purchase?

---

## 📊 Project Roadmap

| Area | What I'm investigating | Status |
|---|---|---|
| 🎯 Business Problem | Identify potential friction in the buyer journey | 🟡 In Progress |
| 👤 Product Research | Explore the buyer experience and user journey | 🟡 In Progress |
| 🔎 Public Research | Analyze reviews, discussions and publicly available information | ⚪️ Planned |
| 💡 Hypotheses | Develop measurable hypotheses from the research | ⚪️ Planned |
| 📐 Metrics | Define relevant product and funnel KPIs | ⚪️ Planned |
| 🗄️ Data | Create a simulated product event dataset | ⚪️ Planned |
| 💻 SQL Analysis | Analyze conversion, funnel behavior and user segments | ⚪️ Planned |
| 📈 Dashboard | Build a product analytics dashboard | ⚪️ Planned |
| 💭 Insights | Translate analysis into product insights | ⚪️ Planned |
| 🚀 Recommendations | Suggest potential product improvements | ⚪️ Planned |
| 🧪 Experimentation | Design potential A/B tests | ⚪️ Planned |

---

## 🔎 Research Approach

I will use several sources of evidence rather than relying only on quantitative data.

### 1. Product Exploration

I will explore Vinted from different user perspectives, including:

- 🛍️ New buyer
- 🔄 Returning buyer
- 👗 New seller

I will document relevant parts of the experience, including:

- Onboarding
- Search and discovery
- Product pages
- Favorites
- Messaging
- Checkout
- Notifications
- Selling flow

### 2. Public User Feedback

**Sources analysed:** App Store, Google Play, Reddit.

| Theme | Seller reviews | Buyer reviews | % of reviews mentioning theme |
|---|---|---|---|
| Customer support | 18 | 7 | 25% |
| Dispute resolution | 18 | 7 | 25% |
| Search/filtering | 18 | 7 | 25% |
| Shipping | 18 | 7 | 25% |

Types of reported issues falling into the category of customer support: 

Some users reported the absence of a condition filter, while the feature was available in my current app version. This may indicate a staged rollout, A/B test, regional variation, or inconsistent UX rather than a universally missing feature.

---

### 3. Competitive Research

I will compare relevant parts of the experience with other marketplace products to identify differences in:

- Discovery
- Search
- Trust
- Checkout
- Seller experience
- User retention

---

## 💡 Initial Hypotheses

These are starting hypotheses, not conclusions.

### H1 — Favorites do not always indicate strong purchase intent

Users may use Favorites primarily as a way to save or compare items rather than as a direct step toward purchasing.

Potential analysis:

Favorite → Purchase conversion rate

---

### H2 — Purchase friction may occur late in the buyer journey

Additional information or costs revealed later in the purchasing process could contribute to abandonment.

Potential analysis:

Checkout Started → Purchase conversion

---

### H3 — New users may behave differently from returning users

Users familiar with the marketplace may move through the purchase funnel differently from first-time users.

Potential analysis:

Compare:

New Users vs. Returning Users

across funnel conversion and repeat purchase behavior.

---

## 📐 Key Metrics

The initial metrics I plan to investigate include:

### Acquisition & Engagement

- Active Users
- Sessions
- Product Views
- Searches
- Favorites

### Conversion

- View → Favorite Rate
- Favorite → Checkout Rate
- Checkout → Purchase Rate
- Overall Purchase Conversion Rate

### Retention

- Day 1 Retention
- Day 7 Retention
- Day 30 Retention
- Repeat Purchase Rate

### Segmentation

Where appropriate, I will compare behavior by:

- New vs. returning users
- Device
- Product category
- Price range
- Buyer activity level

---

## 🗄️ Data

Because Vinted's internal product data is not publicly available, the quantitative analysis will use a simulated event-level dataset.

The dataset will be designed around realistic marketplace events such as:

```text
app_open
search
product_view
favorite
message_seller
checkout_started
purchase
