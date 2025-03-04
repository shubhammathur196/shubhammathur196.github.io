<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Project Portfolio</title>
  <style>
    /* Global Styles */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      line-height: 1.6;
    }
    header, nav, main, footer {
      margin: 0;
      padding: 0;
    }
    /* Header & Navigation */
    header {
      background: #007bff;
      color: #fff;
      padding: 10px 20px;
      text-align: center;
    }
    header h1 {
      margin: 0;
    }
    nav ul {
      list-style: none;
      padding: 0;
      margin: 10px 0 0;
      display: flex;
      justify-content: center;
      gap: 20px;
    }
    nav ul li a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
    }
    /* Main Content */
    main {
      margin: 20px;
    }
    article.project {
      margin-bottom: 40px;
      border-bottom: 1px solid #ccc;
      padding-bottom: 20px;
    }
    article.project h2 {
      color: #333;
      text-align: center;
    }
    section {
      margin: 20px 0;
    }
    section h3 {
      color: #333;
    }
    .image-container {
      text-align: center;
      margin: 20px 0;
    }
    .image-container img {
      max-width: 100%;
      height: auto;
      margin: 10px;
    }
    /* Footer */
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
  <header>
    <h1>My Project Portfolio</h1>
    <nav>
      <ul>
        <li><a href="#adidas">Adidas Dashboard</a></li>
        <li><a href="#stock">German Stock Analysis</a></li>
        <li><a href="#abtesting">A/B Testing Banner</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <!-- Adidas Project Section -->
    <article id="adidas" class="project">
      <h2>Adidas USA Sales Performance Dashboard (2020-2021)</h2>
      <div class="image-container">
        <img src="images/adidas_dashboard.png" alt="Adidas Dashboard Image 1">
        <img src="images/adidas2.png" alt="Adidas Dashboard Image 2">
      </div>
      <section>
        <h3>Project Description</h3>
        <p>
          This project analyzes sales performance data of Adidas in the USA for the years 2020-2021, focusing on key metrics such as total sales, units sold, and operating margins. Using Power BI dashboards, the project provides visualizations and insights into sales trends, performance by region, retailer, product, and sales method.
        </p>
      </section>
      <section>
        <h3>Questions This Project Answers</h3>
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
    </article>

    <!-- German Stock Market Analysis Section -->
<article id="stock" class="project">
      <h2>German Stock Market Analysis (2023-2024)</h2>
      <div class="image-container">
        <img src="images/Stock.png" alt="German Stock Market Dashboard">
      </div>
      <section>
        <h3>Project Description</h3>
        <p>
          This project involves the analysis of the German Stock Market (DAX index) data for the years 2023-2024. Using Power BI dashboards, the project visualizes key metrics such as average close and open prices, daily returns, price range volatility, and trends in trading volumes.
        </p>
      </section>
      <section>
        <h3>Questions This Project Answers</h3>
        <ol>
          <li>Market Performance</li>
          <li>Volatility Analysis</li>
          <li>Daily Returns</li>
          <li>Volume Analysis</li>
          <li>Seasonality and Trends</li>
          <li>Key Performance Highlights</li>
        </ol>
      </section>
    </article>

    <!-- A/B Testing Project Section -->
<article id="abtesting" class="project">
      <h2>A/B Testing: Food &amp; Drink Banner</h2>
      <div class="image-container">
        <img src="images/abtesting.jpg" alt="A/B Testing Overview">
      </div>
      <section>
        <h3>Project Overview</h3>
        <p>
          This project evaluates whether displaying a food &amp; drink banner on the GloBox mobile website increases user conversions and revenue. Users are randomly assigned to either a control group (no banner) or a test group (banner displayed).
        </p>
        <p>
          For a detailed analysis including the SQL queries and statistical tests, please visit the project repository on GitHub.
        </p>
        <p style="text-align: center;">
          <a href="https://github.com/shubhammathur196/Projects/tree/e013037e40afa6c708db20d35be29b1eb6d06037/AB%20Testing" target="_blank" style="padding: 10px 20px; background: #007bff; color: #fff; text-decoration: none; border-radius: 5px;">View Project on GitHub</a>
        </p>
      </section>
    </article>
  </main>
  <footer>
    <p>&copy; 2025 Project Dashboards</p>
  </footer>
</body>
</html>
