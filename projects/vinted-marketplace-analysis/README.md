# 🛍️ Vinted Product Analytics Case Study

> An independent Product Analytics case study exploring buyer behaviour, conversion, and potential friction points in the Vinted marketplace.

Project Status: 🟡 In Progress  
Project Type: Independent Portfolio Project  
Product: Vinted  
Focus: Product Analytics · User Behavior · UX · Conversion · Experimentation

---

## 📌 Project Overview

Vinted is a peer-to-peer marketplace where users can buy and sell second-hand items. The platform depends on successful interactions between both sides: buyers need to trust that they will receive items as described, while sellers need to trust that they will be paid and protected from fraudulent claims.

For this case study, I am exploring the buyer and seller journey, with a particular focus on understanding where users may lose interest or encounter friction.

The project combines:

- 🔎 Product and UX research
- 💬 Qualitative analysis of user feedback
- 📊 Product analytics
- 💻 SQL analysis
- 📈 Data visualisation
- 💡 Product recommendations
- 🧪 Experiment design

- ## 📊 Project Roadmap

| Area | What I'm investigating | Status |
|---|---|---|
| 🎯 Business Problem | Identify potential friction in the buyer journey | 🟡 In Progress |
| 👤 Product Research | Explore the buyer experience and user journey | 🟡 In Progress |
| 🔎 Public Research | Analyze reviews, discussions and publicly available information | 🟡 In Progress |
| 💡 Hypotheses | Develop measurable hypotheses from the research | ⚪️ Planned |
| 📐 Metrics | Define relevant product and funnel KPIs | ⚪️ Planned |
| 🗄️ Data | Create a simulated product event dataset | ⚪️ Planned |
| 💻 SQL Analysis | Analyze conversion, funnel behavior and user segments | ⚪️ Planned |
| 📈 Dashboard | Build a product analytics dashboard | ⚪️ Planned |
| 💭 Insights | Translate analysis into product insights | ⚪️ Planned |
| 🚀 Recommendations | Suggest potential product improvements | ⚪️ Planned |
| 🧪 Experimentation | Design potential A/B tests | ⚪️ Planned |

---

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

## 🔎 Research Approach

I will use several sources of evidence rather than relying only on quantitative data.

### 1. Product Exploration

I will explore Vinted from both seller and buyer perspectives.

**Buyer journey**
Search
↓
Apply filters
↓
Find an item
↓
Check seller/listing
↓
Purchase
↓
Shipping
↓
Receive item
↓
Problem? → Contact support / Open issue

**Potential frictions during the buyer journey**
| Stage         | User goal            | Potential friction        |
| ------------- | -------------------- | ------------------------- |
| Search        | Find relevant item   | Limited filters           |
| Evaluate      | Assess item/seller   | Incomplete information    |
| Purchase      | Complete transaction | Shipping cost             |
| Post-purchase | Resolve problems     | Support/protection issues |

**Seller journey**
Create listing
↓
Receive order
↓
Ship item
↓
Buyer receives item
↓
Transaction completed
          ↓
       Problem?
          ↓
    Dispute/support

**Potential frictions during the seller journey**
| Stage         | User goal            | Potential friction        |
| ------------- | -------------------- | ------------------------- |
| Create listing| Sell an item         | Listing being taken down  |
| Shipping      | Shipping item        | Incomplete information/shipping issues|
| Buyer receives item | Buyer is satisfied | Condition doesn't match description        |
| Post-purchase | Resolve problems     | Support/protection issues |

### 2. Public User Feedback

**Sources analysed:** App Store, Google Play, Reddit, Trustpilot.

> Note: Reviews could contain multiple themes; percentages therefore do not sum to 100%.

**Seller's reviews:**
40 seller reviews analysed
| Theme | Reviews | % of seller reviews | 
|---|---|---|
| Customer support | 35 | 87.5% |
| Perceived buyer favoritism | 8 | 20% |
| Seller protection/scam | 7 | 17.5% |
| Dispute resolution | 6 | 15% |
| Shipping | 4 | 10% |

**Buyer's reviews:**
40 buyer reviews analysed
| Theme | Reviews | % of buyer reviews |
|---|---|---|
| Customer support | 26 | 65% |
| Item condition | 6 | 15% |
| Search/filtering | 7 | 17.5% |
| Scam | 11 | 27.5% |
| Shipping | 17 | 42.5% |
| Buyer protection | 19 | 47.5% |

In the following table, I'll provide more context for the mentioned categories

| Perspective | Theme                          | Included in this category                                                                                                                      |
| ----------- | ------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Seller      | **Customer support**           | Slow or absent responses, automated/template responses, inability to reach human support, unhelpful communication, unresolved support requests |
| Seller      | **Perceived buyer favoritism** | Sellers reporting that Vinted unfairly sided with buyers or that buyers received more protection in disputes                                   |
| Seller      | **Seller protection/scam**   | Sellers reporting scams, fraudulent buyers, financial losses, or feeling insufficiently protected against fraudulent activity                  |
| Seller      | **Dispute resolution**         | Complaints specifically about how a dispute, claim, refund, or conflict between buyer and seller was handled                                   |
| Seller      | **Shipping**                   | Problems with shipping costs, labels, lost/damaged parcels, delivery issues, or shipping-related restrictions                                  |
| Buyer       | **Customer support**           | Slow, automated, unhelpful, or ineffective responses; unresolved support requests                                                              |
| Buyer       | **Item condition**             | Items arriving in worse condition than described, inaccurate condition descriptions, or difficulty filtering by condition                      |
| Buyer       | **Search/filtering**           | Missing, limited, or ineffective search and filtering options, including difficulty narrowing listings by relevant criteria                    |
| Buyer       | **Scam**                       | Reports of fraudulent sellers/listings, counterfeit goods, or buyers losing money due to suspected scams                                       |
| Buyer       | **Shipping**                   | High shipping costs, delivery problems, limited location options, or difficulty identifying lower-shipping-cost listings                       |
| Buyer       | **Buyer protection**           | Buyers reporting inadequate protection, difficulty getting refunds, or feeling unsupported when an item was not received/as described          |


According to the data, customer support is the dominant pain point. Most users are complaining about automated or slow responses, poor resolution or perceived unfair decisions. Another pain point is sudden, automated account suspensions or restrictions that occur without clear human communication.

Some users reported the absence of a condition filter, while the feature was available in my current app version. This may indicate a staged rollout, A/B test, regional variation, or inconsistent UX rather than a universally missing feature.

---

### Business Problem

Since I don't have access to Vinted's internal data, I'll frame it as a potential business problem identified through user research and public feedback.

> User review analysis identified customer support and post-transaction protection as recurring pain points for both buyers and sellers. Ineffective support and perceived unfairness in dispute resolution may reduce trust in the platform and negatively affect user retention and marketplace activity.

The marketplace-specific risks are as follows:

**For buyers:**

If they don't trust protection → less willingness to purchase.

**For sellers:**

If they feel financially unprotected → less willingness to list and sell.

**For Vinted:**

Losing either side damages marketplace liquidity.

Poor experience / unresolved issue
↓
Loss of trust
↓
Reduced willingness to buy or sell
↓
Potential impact on marketplace activity and retention

---

## 💡 Initial Hypotheses

These are starting hypotheses, not conclusions.

### H1 — Favourites do not always indicate strong purchase intent

Users may use Favourites primarily as a way to save or compare items rather than as a direct step toward purchasing.

Potential analysis:

Favourite → Purchase conversion rate

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

across funnel conversion and repeat purchase behaviour.

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

Where appropriate, I will compare behaviour by:

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
