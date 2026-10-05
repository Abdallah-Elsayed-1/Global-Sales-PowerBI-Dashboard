<div align="center">

  <h1>🌐 Global Enterprise Sales & Financial Analytics Dashboard</h1>
  <p><b>An End-to-End Power BI Business Intelligence Solution analyzing global sales streams, profit margins, regional performance, and multi-year time intelligence.</b></p>

  <!-- Clean Tech Stack Badge Bar -->
  <p align="center">
    <code>🟡 Power BI</code> &nbsp;|&nbsp; 
    <code>🔵 Power Query & M-Engine</code> &nbsp;|&nbsp; 
    <code>🟢 Advanced DAX & Time Intelligence</code> &nbsp;|&nbsp; 
    <code>🟣 Relational Star Schema</code> &nbsp;|&nbsp; 
    <code>📈 Financial Analytics</code>
  </p>

</div>

<hr />
<br />

<h2>📌 Project Overview</h2>
<p>
  This project delivers a comprehensive <b>Global Enterprise Sales Dashboard</b> designed to analyze multi-million-dollar transactional sales data across international territories and diverse customer segments over multiple fiscal years (2012 – 2014).
</p>
<p>
  <b>Business Value:</b> Transforms complex enterprise transactional data into actionable strategic insights, allowing c-suite executives and regional sales managers to evaluate profitability, monitor YoY growth, and optimize market expansion.
</p>

<br />

<h2>📊 Executive Dashboard Overview</h2>
<p>The primary interactive interface provides a consolidated high-level overview of total sales, gross profits, profit margins, order quantities, and geographic distributions:</p>

<div align="center">
  <img src="https://i.postimg.cc/V6nQSLRd/dashbwrd.png" alt="Global Sales Executive Dashboard" width="100%" />
</div>

<br />
<hr />
<br />

<h2>🔑 Key Performance Indicators (KPIs)</h2>
<ul>
  <li><b>Total Sales Revenue:</b> Cumulative top-line financial revenue across all geographic territories.</li>
  <li><b>Total Profit & Margin %:</b> Net financial earnings and profitability ratios calculated per order and region.</li>
  <li><b>Order Volume & Quantity:</b> Total fulfilled customer orders and item quantities shipped globally.</li>
  <li><b>Year-over-Year (YoY) Growth:</b> Dynamic Time Intelligence metrics tracking performance trends across years.</li>
</ul>

<br />
<hr />
<br />

<h2>🛠️ Analytics Architecture & Pipeline Stages</h2>

<h3>Stage 1: ETL & Power Query Data Transformation</h3>
<p>
  Raw transactional tables were ingested and processed using the <b>Power Query Engine</b>. Applied data preparation steps include removing empty records, converting data types, standardizing regional attributes, and crafting custom M-code logic.
</p>

<div align="center">
  <img src="https://i.postimg.cc/HxXDJs2x/bawr-kwyry.png" alt="Power Query ETL Engine" width="85%" />
</div>

<br />

<h3>Stage 2: Relational Data Modeling (Star Schema)</h3>
<p>
  Constructed an optimized <b>Star Schema Relational Model</b> connecting the central transactional fact table (<code>Fact_Sales</code>) with dimension tables (<code>Dim_Customer</code>, <code>Dim_Product</code>, <code>Dim_Date</code>, <code>Dim_Territory</code>) via strict 1-to-Many relationships.
</p>

<div align="center">
  <table border="0" width="100%">
    <tr>
      <td width="50%" align="center" valign="top">
        <h4>Overview Star Schema Architecture</h4>
        <img src="https://i.postimg.cc/j5P0WdX2/data-mwdylynj.png" width="95%" alt="Star Schema Data Model" />
      </td>
      <td width="50%" align="center" valign="top">
        <h4>Detailed Key Relationship Logic</h4>
        <img src="https://i.postimg.cc/V6nQSLR5/data-mwdylynj-atdh.png" width="95%" alt="Data Model Keys & Relationships" />
      </td>
    </tr>
  </table>
</div>

<br />

<h3>Stage 3: Advanced DAX & Measure Calculations</h3>
<p>Developed core mathematical DAX calculations and Time Intelligence measures:</p>
<ul>
  <li><code>Total Revenue</code> = <code>SUM(Fact_Sales[LineTotal])</code></li>
  <li><code>Total Profit</code> = <code>SUM(Fact_Sales[LineTotal]) - SUM(Fact_Sales[TotalCost])</code></li>
  <li><code>Profit Margin %</code> = <code>DIVIDE([Total Profit], [Total Revenue], 0)</code></li>
</ul>

<br />
<hr />
<br />

<h2>🎯 Interactive Filtering & Multi-Dimensional Analysis</h2>

<h3>1. Fiscal Year Time Intelligence Comparisons</h3>
<p>Comparative analysis showing business scaling from early baseline stages in 2012 to peak revenue performance in 2014:</p>

<div align="center">
  <table border="0" width="100%">
    <tr>
      <td width="50%" align="center" valign="top">
        <h4>Fiscal Year 2012 Performance</h4>
        <img src="https://i.postimg.cc/MTV2cKDM/snt-2012.png" width="95%" alt="Sales Performance 2012" />
        <p align="left"><small>Establishes baseline sales volumes and early operational order trends.</small></p>
      </td>
      <td width="50%" align="center" valign="top">
        <h4>Fiscal Year 2014 Expansion</h4>
        <img src="https://i.postimg.cc/LXLKq6T4/Ssnt-2014.png" width="95%" alt="Sales Performance 2014" />
        <p align="left"><small>Demonstrates significant top-line revenue expansion and volume growth.</small></p>
      </td>
    </tr>
  </table>
</div>

<br />

<h3>2. Regional Drill-Down & Account-Level Analysis</h3>
<p>Deep-dive slicing capabilities enabling territory managers and sales reps to evaluate specific market penetration:</p>

<div align="center">
  <table border="0" width="100%">
    <tr>
      <td width="33%" align="center" valign="top">
        <h4>Belgium Territory (2014)</h4>
        <img src="https://i.postimg.cc/0QDR62fN/bljyka-2014.png" width="95%" alt="Belgium Slicer 2014" />
        <p align="left"><small>Country-specific analysis for Belgium in 2014.</small></p>
      </td>
      <td width="33%" align="center" valign="top">
        <h4>Territory Region Slicer</h4>
        <img src="https://i.postimg.cc/7608CYVT/fltr-balryjn.png" width="95%" alt="Regional Slicer Analysis" />
        <p align="left"><small>Slices dashboard across global sales territories.</small></p>
      </td>
      <td width="33%" align="center" valign="top">
        <h4>Customer Account Isolation</h4>
        <img src="https://i.postimg.cc/qqrf2VbJ/fltr-balʿmyl.png" width="95%" alt="Customer Account Slicer" />
        <p align="left"><small>Tracks individual high-value B2B/B2C accounts.</small></p>
      </td>
    </tr>
  </table>
</div>

<br />
<hr />
<br />

<h2>💡 Strategic Business Insights</h2>
<ol>
  <li><b>Geographic Revenue Drivers:</b> Top-performing international territories contribute over 60% of total revenue, highlighting key targets for future retail expansion.</li>
  <li><b>High-Margin Customer Retention:</b> B2B accounts filtered by high order volume yield superior profit margins compared to smaller individual transactions.</li>
  <li><b>Operational Scalability:</b> Multi-year analysis confirms healthy growth momentum, recommending increased inventory allocation for high-demand product lines during Q3/Q4.</li>
</ol>

<br />
<hr />
<br />

<h2>📂 Repository Architecture</h2>
<pre>
├── Data/                        # Global transactional sales datasets
├── Reports/                     # Global_Sales_Performance_Dashboard.pbix
├── Screenshots/                 # Process visual walkthroughs
└── README.md                    # Detailed documentation
</pre>
