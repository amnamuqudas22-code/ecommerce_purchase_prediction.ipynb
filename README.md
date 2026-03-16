# ecommerce_purchase_prediction.ipynb
A predictive analytics project analyzing online shopper behavior to identify high-intent visitors and predict purchases. Includes exploratory data analysis, a Gaussian Naive Bayes model, visualizations, and actionable recommendations to boost e-commerce conversions.

# Predicting Online Shopper Conversions: Turning Browsers into Buyers

**One-line hook:** Identify high-intent e-commerce visitors and increase conversions using predictive analytics.

---

## The Business Problem

An online retail company struggles to convert visitors into buyers — only about 15% of sessions result in a purchase. Missed opportunities cost revenue, while untargeted marketing increases expenses. The company needs a way to predict which visitors are most likely to purchase and focus efforts efficiently.

## The Data

The dataset contains 12,330 user sessions over one year, including metrics like number of product pages viewed, time spent on pages, bounce rates, traffic source, and visitor type. The target variable is Revenue (True = purchased, False = did not purchase).

## Key Discoveries

- **Product Engagement vs Purchase:** Visitors who focus on high-value product pages are more likely to buy, while those browsing many low-value pages are less likely to convert.
- **Bounce and Exit Rates Matter:** Lower bounce and exit rates correlate with higher likelihood of purchase.
- **Visitor Type Impacts Conversion:** Returning visitors are more likely to complete purchases than new visitors.

## Visualizing the Story

![Product Engagement vs Revenue](product_pages_vs_revenue.png)

*Visitors who engage with high-value pages are more likely to convert than casual browsers, highlighting the importance of targeted engagement.*

## Prediction Model

A Gaussian Naive Bayes model predicts which visitors will purchase with 42% recall and 63% precision, meaning it identifies a sizable portion of buyers while keeping false positives moderate. This allows marketing efforts to focus on high-intent users, recovering missed revenue opportunities without extra traffic acquisition costs.

## Recommendations

1. **Target high-value visitors with personalized promotions:** Send product recommendations or discounts to visitors who spend time on high PageValue and moderate ProductRelated pages; this could convert up to 42% of identified high-intent visitors.
2. **Reduce excessive browsing to improve conversion:** Streamline product navigation, highlight key pages, and reduce distractions for casual visitors; simplifying the experience could boost overall conversion rates.
3. **Proactively engage borderline visitors with nudges:** Use pop-ups, chat prompts, or session-based product suggestions for visitors who spend moderate time but haven’t purchased; targeting false negatives could recover a portion of missed buyers and increase revenue.

## Tools & Techniques

Python | Pandas | Scikit-Learn | Matplotlib | Seaborn | Gaussian Naive Bayes | Google Colab

---

*This project was completed as part of ISOM 835: Predictive Analytics at Suffolk University’s Sawyer Business School.*
