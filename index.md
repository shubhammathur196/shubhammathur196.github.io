



<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Project Dashboards</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }
        h1, h2 {
            text-align: center;
            color: #333;
        }
        section {
            margin: 20px;
        }
        .image-container {
            text-align: center;
            margin: 20px 0;
        }
        .image-container img {
            max-width: 100%;
            height: auto;
        }
        footer {
            text-align: center;
            padding: 10px;
            background: #f4f4f4;
        }
        /* Responsive Design */
        @media (min-width: 768px) {
            body {
                margin: 0 10%;
            }
        }
        @media (min-width: 1024px) {
            body {
                margin: 0 20%;
            }
        }
    </style>
</head>
<body>
    <h1>Adidas USA Sales Performance Dashboard (2020-2021)</h1>
    <div class="image-container">
        <img src="images/adidas_dashboard.png" alt="Adidas Dashboard Image 1">
        <img src="images/adidas2.png" alt="Adidas Dashboard Image 2">
    </div>
    <section>
        <h2>Project Description</h2>
        <p>
            This project analyzes sales performance data of Adidas in the USA for the years 2020-2021, focusing on key metrics such as total sales, units sold, and operating margins. Using Power BI dashboards, the project provides visualizations and insights into sales trends, performance by region, retailer, product, and sales method.
        </p>
    </section>
    <section>
        <h2>Questions This Project Answers</h2>
        <ol>
            <li>Overall Sales Performance</li>
            <li>Sales by Region</li>
            <li>Best Performing Areas</li>
            <li>Retailer Performance</li>
            <li>Product Analysis</li>
            <li>Sales Trends Over Time</li>
            <li>Sales Method Analysis</li>
            <li>Geographic Distribution</li>
        </ol>
    </section>

   <h1>German Stock Market Analysis (2023-2024)</h1>
    <div class="image-container">
        <img src="images/Stock.png" alt="German Stock Market Dashboard">
    </div>
    <section>
        <h2>Project Description</h2>
        <p>
            This project involves the analysis of the German Stock Market (DAX index) data for the years 2023-2024. Using Power BI dashboards, the project visualizes key metrics such as average close and open prices, daily returns, price range volatility, and trends in trading volumes.
        </p>
    </section>
    <section>
        <h2>Questions This Project Answers</h2>
        <ol>
            <li>Market Performance</li>
            <li>Volatility Analysis</li>
            <li>Daily Returns</li>
            <li>Volume Analysis</li>
            <li>Seasonality and Trends</li>
            <li>Key Performance Highlights</li>
        </ol>
    </section>
<!-- BEGIN: A/B Testing Project Section -->
    <h1>A/B Testing: Food &amp; Drink Banner</h1>
    <div class="image-container">
        <img src="images/abtesting.jpg" alt="A/B Testing Overview">
    </div>
    <section>
        <h2>Project Description</h2>
        <p>
            Welcome to your first Mastery Project! In this project, you will analyze the results of an A/B test for GloBox, an online marketplace specializing in unique and high-quality products from around the world. GloBox has recently expanded its food &amp; drink offerings, and the Growth team decided to test whether a banner highlighting these products on the mobile website could increase conversion rates and revenue.
        </p>
        <p>
            In the test setup, users are randomly assigned to one of two groups:
            <strong>Control Group (Group A)</strong> – Users see the standard page without the banner.
            <strong>Test Group (Group B)</strong> – Users see the page with the food &amp; drink banner.
        </p>
        <p>
            Your task is to compare key metrics such as conversion rates, average spend, and overall revenue between the two groups using SQL queries. The goal is to provide data-driven recommendations on whether GloBox should launch the banner experience to all users.
        </p>
    </section>
    <section>
        <h2>Key SQL Queries</h2>
        <pre><code>
-- 1) Combine Activity, Users, and Groups (mobile-only)
SELECT a.*, u.*, g."group"
FROM activity a
JOIN users u ON u.id = a.uid
JOIN groups g ON u.id = g.uid
WHERE a.device IN ('A', 'I');

-- 2) Calculate conversion by group (using LEFT JOIN so non-purchasers aren't excluded)
SELECT
    g."group" AS group_name,
    COUNT(DISTINCT u.id) AS total_users,
    COUNT(DISTINCT CASE WHEN a.uid IS NOT NULL THEN u.id END) AS users_with_purchase,
    1.0 * COUNT(DISTINCT CASE WHEN a.uid IS NOT NULL THEN u.id END)
         / COUNT(DISTINCT u.id) AS conversion_rate
FROM users u
JOIN groups g ON u.id = g.uid
LEFT JOIN activity a ON u.id = a.uid AND a.device IN ('A', 'I')
GROUP BY g."group";

-- 3) Compare average spend by group and device
SELECT
    a.device,
    g."group" AS test_group,
    AVG(a.spent) AS average_amount_spent
FROM activity a
JOIN users u ON u.id = a.uid
JOIN groups g ON u.id = g.uid
WHERE a.device IN ('A', 'I')
GROUP BY a.device, g."group"
ORDER BY a.device, g."group";

-- 4) Statistical significance (two-proportion z-test logic)
-- Count converters in each group, compute pooled conversion rate, standard error, and z-score.
        </code></pre>
    </section>
    <!-- END: A/B Testing Project Section -->

   <footer>
        <p>&copy; 2025 Project Dashboards</p>
    </footer>
</body>
</html>
