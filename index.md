<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Project Portfolio</title>
  <style>
    /* Global Styles */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    /* Header */
   header {
      background: #f8f8f8;
      padding: 20px;
      border-bottom: 1px solid #ccc;
    }
    header h1 {
      margin: 0 0 10px 0; /* space under heading */
      font-size: 1.8rem;
      color: #333;
    }

    /* Navigation */
  nav {
      margin-top: 15px;
    }
    nav ol {
      margin: 0;
      padding-left: 1.5rem; /* indent for numbering */
    }
    nav li {
      margin-bottom: 5px; /* spacing between links */
    }
    nav a {
      text-decoration: none;
      color: #007bff;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }

    /* Main Content */
   main {
      margin: 20px;
    }
    article {
      margin-bottom: 40px;
      border-bottom: 1px solid #eee;
      padding-bottom: 20px;
    }
    article h2 {
      color: #333;
      margin-top: 0;
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
  </style>
</head>
<body>

  <!-- Header Section -->
  <header>
    <h1>Project Portfolio</h1>
    <nav>
      <ol>
        <li><a href="#adidas">Adidas Dashboard</a></li>
        <li><a href="#stock">German Stock Analysis</a></li>
        <li><a href="#abtesting">A/B Testing Banner</a></li>
      </ol>
    </nav>
  </header>

  <!-- Main Content -->
  <main>

    <!-- Adidas Project -->
   <article id="adidas">
      <h2>Adidas USA Sales Performance Dashboard (2020-2021)</h2>
      <div class="image-container">
        <!-- Replace with your actual image paths -->
        <img src="images/adidas_dashboard.png" alt="Adidas Dashboard Image 1">
        <img src="images/adidas2.png" alt="Adidas Dashboard Image 2">
      </div>
      <h3>Project Description</h3>
      <p>
        This project analyzes sales performance data of Adidas in the USA for the years 2020-2021, focusing on key metrics such as total sales, units sold, and operating margins. Using Power BI dashboards, the project provides visualizations and insights into sales trends, performance by region, retailer, product, and sales method.
      </p>
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
    </article>

    <!-- German Stock Market Analysis -->
   <article id="stock">
      <h2>German Stock Market Analysis (2023-2024)</h2>
      <div class="image-container">
        <!-- Replace with your actual image path -->
        <img src="images/Stock.png" alt="German Stock Market Dashboard">
      </div>
      <h3>Project Description</h3>
      <p>
        This project involves the analysis of the German Stock Market (DAX index) data for the years 2023-2024. Using Power BI dashboards, the project visualizes key metrics such as average close and open prices, daily returns, price range volatility, and trends in trading volumes.
      </p>
      <h3>Questions This Project Answers</h3>
      <ol>
        <li>Market Performance</li>
        <li>Volatility Analysis</li>
        <li>Daily Returns</li>
        <li>Volume Analysis</li>
        <li>Seasonality and Trends</li>
        <li>Key Performance Highlights</li>
      </ol>
    </article>

    <!-- A/B Testing Project -->
   <article id="abtesting">
      <h2>A/B Testing: Food &amp; Drink Banner</h2>
      <div class="image-container">
        <!-- Replace with your actual image path -->
        <img src="images/abtesting.jpg" alt="A/B Testing Overview">
      </div>
      <h3>Project Overview</h3>
      <p>
        This project evaluates whether displaying a food &amp; drink banner on the GloBox mobile website increases user conversions and revenue. Users are randomly assigned to either a control group (no banner) or a test group (banner displayed).
      </p>
      <p>
        For a detailed analysis including the SQL queries and statistical tests, please visit the project repository on GitHub.
      </p>
      <p style="text-align: center;">
        <a href="https://github.com/shubhammathur196/Projects/tree/e013037e40afa6c708db20d35be29b1eb6d06037/AB%20Testing"
           target="_blank"
           style="padding: 10px 20px; background: #007bff; color: #fff; text-decoration: none; border-radius: 5px;">
          View Project on GitHub
        </a>
      </p>
    </article>

  </main>
</body>
</html>
