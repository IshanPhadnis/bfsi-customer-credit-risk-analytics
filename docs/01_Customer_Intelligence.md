## Question 1 — Customer Segmentation by CLV (Percentile-Based)

### 🎯 Objective
Segment customers into Low, Medium, High, and VIP tiers using dynamic percentile-based segmentation.

### 💼 Why does this matter?
Not all customers carry the same value to the bank. Percentile-based segmentation (rather than fixed CLV thresholds) automatically adapts as the customer base changes, making it a more durable way to prioritize retention, cross-sell, and risk-monitoring efforts across tiers.

### 🧠 Approach
- Rank all customers by `CLV` in descending order
- Use `NTILE(4)` to split the ranked customers into 4 equal-sized groups
- Map tile 1 (highest CLV) → VIP, tile 2 → High, tile 3 → Medium, tile 4 (lowest CLV) → Low

### 💻 SQL

```sql
WITH cte AS (
    SELECT
        Customer_ID,
        CLV,
        NTILE(4) OVER (ORDER BY CLV DESC) AS tiers
    FROM bank.customer
)

SELECT
    Customer_ID,
    CLV,
    CASE
        WHEN tiers = 1 THEN 'VIP'
        WHEN tiers = 2 THEN 'High'
        WHEN tiers = 3 THEN 'Medium'
        ELSE 'Low'
    END AS segment
FROM cte
ORDER BY CLV DESC;
```

### 💡 Business Recommendation

VIP and High-tier customers (top 50% by CLV) should be prioritized for premium relationship management and retention efforts, since they represent the bank's most valuable relationships. Medium and Low tiers are better suited for scaled, automated engagement (e.g., digital-only offers) rather than high-touch service, optimizing cost-to-serve against customer value.

### 📊 Tableau Visual
<img width="2194" height="1544" alt="image" src="https://github.com/user-attachments/assets/0a11a6af-8510-4238-a140-4c293d9b2188" />
# =====================================================================
