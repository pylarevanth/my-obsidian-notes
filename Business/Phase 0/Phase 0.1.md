## B0.1 — What Is a Business?

### 🎯 Goal

By the end of B0.1, you should be able to explain:

- What a business is
- What **value creation** means
- Who **customers** are
- What **products and services** are
- What a **market** is
- How **revenue, costs, and profit** work
- Who **stakeholders** are
- How all of these connect to our final Business AI platform

---

# 1. What Is a Business?

At the simplest level:

> **A business solves a problem or fulfills a need for customers by providing value, and receives something in return—usually money.**

Think of:

```
Customer has a problem
        ↓
Business provides a solution
        ↓
Customer receives value
        ↓
Customer pays
        ↓
Business earns revenue
        ↓
Business pays its costs
        ↓
Remaining amount = profit
```

### Example: Food Delivery

A customer:

> "I want food from a restaurant, but I don't want to travel."

A food-delivery company provides:

- Restaurant discovery
- Ordering
- Payment
- Delivery
- Tracking

The customer gets **convenience**.

The business receives money through things such as delivery fees, commissions, subscriptions, etc.

---

# 2. Value Creation

This is one of the **most important business concepts**.

### What is value?

Value is the benefit a customer receives from a product or service.

A business creates value by solving a problem **better, faster, cheaper, easier, or more conveniently**.

### Example

Suppose a company provides accounting software.

Before:

```
Manual accounting
        ↓
5 hours/day
        ↓
High effort
        ↓
Errors
```

After:

```
Accounting software
        ↓
Automation
        ↓
1 hour/day
        ↓
Less effort + fewer errors
```

The software creates value by saving:

- Time
- Money
- Effort
- Errors

### Important distinction

**Value ≠ Price**

If a customer receives ₹10,000 worth of benefit from a product but pays ₹2,000:

```
Customer value = ₹10,000
Price          = ₹2,000
```

The customer may consider the purchase highly valuable.

---

# 3. Customer

A **customer** is the person or organization that buys or uses a business's offering.

There can be different customer types.

### Individual

```
Netflix → Individual viewer
```

### Business

```
Salesforce → Company
```

### Government

```
Technology vendor → Government department
```

The important question for a business is:

> **Who are we creating value for?**

---

# 4. Product

A **product** is something a business provides to customers to solve a problem or satisfy a need.

Examples:

- Smartphone
- Car
- Laptop
- Software
- Clothing
- Financial application

### Example

Apple provides:

```
iPhone
Mac
iPad
Apple Watch
```

The product is the actual offering customers receive.

---

# 5. Service

A **service** provides value through an activity or ongoing operation rather than primarily through ownership of a physical product.

Examples:

- Consulting
- Cloud computing
- Transportation
- Food delivery
- Banking
- Streaming

For example:

```
Uber

Customer
   ↓
Requests transportation
   ↓
Uber connects customer + driver
   ↓
Customer receives transportation
```

The customer is primarily paying for the **service**.

---

# 6. Market

A **market** is the environment in which customers and businesses interact around a particular need, product, or service.

Example:

```
Food Delivery Market
        ↓
Customers
Restaurants
Delivery platforms
        ↓
Transactions
```

Another example:

```
Cloud Computing Market
        ↓
AWS
Microsoft Azure
Google Cloud
        ↓
Businesses needing computing infrastructure
```

A market can be analyzed through:

- Customers
- Competitors
- Demand
- Supply
- Pricing
- Market size
- Growth

We'll study these much more deeply in **B2 — Strategy & Market Analysis**.

---

# 7. Revenue

**Revenue is the money a business receives from selling its products or services.**

Example:

A SaaS company has:

```
1,000 customers
₹1,000/month/customer
```

Monthly revenue:

```
1,000 × ₹1,000
= ₹10,00,000
```

So:

**Revenue = ₹10 lakh/month**

### Important

Revenue is **not profit**.

A company can have:

```
Revenue = ₹10 lakh
Costs   = ₹8 lakh

Profit  = ₹2 lakh
```

We'll study revenue models in **B1.1** and business metrics in **B3**.

---

# 8. Costs

A business has to spend money to operate.

Examples:

- Employee salaries
- Servers
- Office
- Marketing
- Raw materials
- Software
- Logistics
- Electricity

Suppose:

```
Revenue = ₹10 lakh

Costs:
Employees     ₹4 lakh
Infrastructure ₹2 lakh
Marketing      ₹1 lakh
Operations     ₹1 lakh
-----------------------
Total costs   ₹8 lakh
```

---

# 9. Profit

The simplest relationship:

```
Profit = Revenue − Costs
```

Example:

```
Revenue = ₹10 lakh
Costs   = ₹8 lakh

Profit = ₹2 lakh
```

This is fundamental because businesses ultimately need sustainable economics.

However, **profit is not the only thing businesses care about**.

A company might deliberately spend heavily today to:

- Acquire customers
- Build infrastructure
- Enter a new market
- Develop a new product

because management expects future returns.

We'll learn this decision-making aspect later.

---

# 10. Stakeholders

A **stakeholder** is someone who can affect or is affected by the business.

Common stakeholders:

```
                BUSINESS
                   │
       ┌───────────┼───────────┐
       ↓           ↓           ↓
   Customers    Employees   Investors
       ↓           ↓           ↓
   Suppliers    Management  Government
```

### Examples

**Customers**

Want good products and services.

**Employees**

Want compensation, growth, and a good working environment.

**Investors**

Want the business to create financial value.

**Suppliers**

Want reliable business and payment.

**Government**

Cares about regulations, taxes, compliance, etc.

A good business decision often requires balancing different stakeholder interests.

---

# 11. The Complete Business System

Now connect everything.

```
                    MARKET
                       ↓
                  CUSTOMER NEED
                       ↓
                    BUSINESS
                       ↓
                PRODUCT / SERVICE
                       ↓
                  VALUE CREATED
                       ↓
                    CUSTOMER
                       ↓
                     PRICE
                       ↓
                   REVENUE
                       ↓
                    − COSTS
                       ↓
                    PROFIT
```

But this isn't a one-time process.

A real business continuously repeats the cycle:

```
Create value
     ↓
Acquire customers
     ↓
Generate revenue
     ↓
Control costs
     ↓
Generate profit
     ↓
Reinvest
     ↓
Improve product
     ↓
Create more value
     ↓
Acquire more customers
```

---

# 12. 🔥 Our Project Connection

This is where B0.1 becomes important for our final project.

Our eventual system isn't simply going to analyze random numbers.

It needs to understand **business entities and relationships**.

For example:

```
Customer
   ↓
Purchases
   ↓
Product
   ↓
Generates
   ↓
Revenue
   ↓
Requires
   ↓
Costs
   ↓
Produces
   ↓
Profit
```

Imagine management asks:

> **"Why did profit decrease this quarter?"**

Our system shouldn't immediately ask an LLM to guess.

It should eventually investigate:

```
Profit decreased
       ↓
Revenue?
       ↓
Costs?
       ↓
Revenue by product?
       ↓
Revenue by customer segment?
       ↓
Pricing?
       ↓
Customer churn?
       ↓
Operating costs?
       ↓
Identify contributing factors
       ↓
Evidence
       ↓
Recommendation
```

That's the mindset we are building from **B0.1 onward**.

---

# 📝 NOTION NOTES — B0.1

## What is a Business?

A business creates value for customers by solving problems or fulfilling needs and receives value in return, usually through revenue.

### Core Concepts

|Concept|Meaning|
|---|---|
|**Business**|Organization/system that creates and captures value|
|**Value**|Benefit received by the customer|
|**Customer**|Person or organization receiving/buying the offering|
|**Product**|Tangible or digital offering|
|**Service**|Activity/ongoing offering that provides value|
|**Market**|Environment where businesses and customers interact|
|**Revenue**|Money earned from selling products/services|
|**Cost**|Resources/money spent to operate|
|**Profit**|Revenue − Costs|
|**Stakeholder**|Party affected by or able to affect the business|

### Core Formula

```
Profit = Revenue − Costs
```

### Core Business Flow

```
Problem
 ↓
Solution
 ↓
Customer
 ↓
Value
 ↓
Revenue
 ↓
Costs
 ↓
Profit
```

---

# 🎯 INTERVIEW Q&A

### Q1. What is a business?

**Answer:**

A business is an organization or system that creates value for customers by solving problems or fulfilling needs and captures value in return, usually through revenue.

---

### Q2. What is value creation?

**Answer:**

Value creation is the process of providing a benefit to customers by solving a problem or fulfilling a need in a way they consider worthwhile.

---

### Q3. What is the difference between revenue and profit?

**Answer:**

Revenue is the money a business earns from its products or services, while profit is what remains after subtracting costs from revenue.

```
Profit = Revenue − Costs
```

---

### Q4. What is a market?

**Answer:**

A market is the environment in which businesses and customers interact around products, services, or needs.

---

### Q5. Who are stakeholders?

**Answer:**

Stakeholders are individuals or organizations that can affect or are affected by a business, such as customers, employees, investors, suppliers, and government.

---

### Q6. Can a company have high revenue but low profit?

**Answer:**

Yes.

For example:

```
Revenue = ₹100 crore
Costs   = ₹95 crore

Profit  = ₹5 crore
```

The company has high revenue but relatively low profit because its costs are high.

---

### Q7. Why is understanding business important for an AI engineer building a business AI system?

**Answer:**

Because the AI system must understand what the business metrics represent and how they relate to business decisions. Without business understanding, an AI system may produce technically correct analysis that is not useful for management.

---

# 🧪 PRACTICAL EXERCISE

Take **Amazon** as an example and identify:

```
Customer:
?

Products:
?

Services:
?

Value created:
?

Revenue:
?

Major costs:
?

Stakeholders:
?

Market:
?
```

Don't worry about getting everything perfect. The objective is to train yourself to **look at a company as a business system rather than just a brand/app**.

---

# 🧠 B0.1 REVIEW

Before moving to **B0.2**, make sure these relationships are clear:

```
Customer
   ↓
Has a problem/need
   ↓
Business provides
   ↓
Product/Service
   ↓
Creates value
   ↓
Customer pays
   ↓
Revenue
   ↓
Business incurs costs
   ↓
Profit
```

### The most important takeaway

> **Business = creating value for customers + capturing enough value to operate sustainably.**

And this foundation will eventually allow us to answer much more complicated questions such as:

> **"Revenue dropped 15%. What happened, why did it happen, and what should management do?"**

That is the type of reasoning our final Business AI platform must eventually perform.

**B0.1 complete.**

---
