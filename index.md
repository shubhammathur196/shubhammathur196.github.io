<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Project Dashboards</title>
    <style>
        /* General body and layout styling */
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
        .project-container {
            border: 1px solid #ddd;
            border-radius: 8px;
            margin: 20px auto;
            padding: 20px;
            box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
            max-width: 90%; /* Default for mobile */
            background-color: #fff;
        }
        .image-container {
            text-align: center;
            margin: 20px 0;
        }
        .image-container img {
            max-width: 80%;
            height: auto;
            border: 1px solid #ccc;
            box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
        }
        footer {
            text-align: center;
            padding: 10px;
            background: #f4f4f4;
        }

  /* Responsive Design for Larger Screens */
       @media (min-width: 768px) {
            .project-container {
                max-width: 70%; /* For tablets and small desktops */
            }
        }

   @media (min-width: 1024px) {
            .project-container {
                max-width: 50%; /* For larger desktops */
            }
        }
    </style>
</head>
<body>
    <!-- Project 1: Adidas Dashboard -->
    <div class="project-container">
        <h1>Adidas USA Sales Performance Dashboard (2020-2021)</h1>
        <div class="image-container">
            <img src="images\adidas_dashboard.png" alt="Adidas Dashboard">
            <img src="images\adidas2.png" alt="Adidas Dashboard">
        </div>
        <section>
            <h2>Project Description</h2>
            <p>
                This project analyzes sales performance data of Adidas in the USA for the years 2020-2021, focusing on key metrics such as total sales, units sold, and operating margins. Using Power BI dashboards, the project provides visualizations and insights into sales trends, performance by region, retailer, product, and sales method. The dashboards are designed to aid decision-making by presenting the data in an interactive and user-friendly manner.
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
    </div>
<!-- Project 2: German Stock Market Dashboard -->
    <div class="project-container">
        <h1>German Stock Market Analysis (2023-2024)</h1>
        <div class="image-container">
            <img src="images\stock_dashboard.png" alt="German Stock Market Dashboard">
        </div>
        <section>
            <h2>Project Description</h2>
            <p>
                This project involves the analysis of the German Stock Market (DAX index) data for the years 2023-2024. Using Power BI dashboards, the project visualizes key metrics such as average close and open prices, daily returns, price range volatility, and trends in trading volumes. The aim is to provide actionable insights into market performance, volatility patterns, and high/low volume days to support investment strategies.
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
    </div>

   <footer>
        <p>&copy; 2025 Project Dashboards</p>
    </footer>
</body>
</html>
