<h1>Scalable Ride Demand Prediction using a Distributed ETL Pipeline.</h1>
<hr>
<h2>📌 Project Overview</h2>
<p>
This project builds a <b>scalable ETL pipeline</b> to process NYC taxi ride data 
and predict hourly ride demand.
</p>

<p>
The objective is to transform raw ride data into structured, analytics-ready datasets 
and develop machine learning models for demand forecasting.
</p>

<p>
The project follows the <b>CRISP-DM methodology</b> and distributed data engineering principles.
</p>

<hr>

<h2>🏗️ Project Architecture</h2>

<p>
Raw Parquet Data <br>
→ Data Cleaning <br>
→ Feature Engineering <br>
→ Hourly Aggregation <br>
→ Structured Storage <br>
→ Machine Learning Models <br>
→ Evaluation
</p>

<hr>

<h2>📊 Dataset</h2>

<ul>
  <li>NYC Taxi Ride Dataset (Parquet format)</li>
  <li>Pickup & Dropoff timestamps</li>
  <li>Trip distance</li>
  <li>Passenger count</li>
  <li>Fare amount</li>
  <li>Location IDs</li>
</ul>

<hr>

<h2>⚙️ ETL Pipeline</h2>

<h3>🔹 Data Ingestion</h3>
<ul>
  <li>Loaded raw Parquet ride data</li>
</ul>

<h3>🔹 Data Cleaning</h3>
<ul>
  <li>Removed missing & invalid records</li>
  <li>Filtered unrealistic trip values</li>
  <li>Ensured timestamp consistency</li>
</ul>

<h3>🔹 Feature Engineering</h3>
<ul>
  <li>Extracted hour of day</li>
  <li>Extracted day of week</li>
  <li>Created weekend indicator</li>
</ul>

<h3>🔹 Aggregation</h3>
<ul>
  <li>Calculated hourly ride counts</li>
</ul>

<hr>

<h2>🗄️ Data Storage</h2>

<p>
Processed data was stored in a structured format to ensure:
</p>

<ul>
  <li>Efficient querying</li>
  <li>Reproducibility</li>
  <li>Scalability for future distributed processing</li>
</ul>

<hr>

<h2>🤖 Modeling & Evaluation</h2>

<ul>
  <li>Linear Regression</li>
  <li><b>Random Forest Regressor (Best Model)</b></li>
</ul>

<p>
Random Forest achieved the lowest RMSE and captured nonlinear demand patterns 
more effectively than Linear Regression.
</p>

<p><b>Key Insights:</b></p>
<ul>
  <li>Peak demand during rush hours</li>
  <li>Weekend behavior differs from weekdays</li>
  <li>Tree-based models outperform linear models</li>
</ul>

<hr>

<h2>🚀 Future Improvements</h2>

<ul>
  <li>Integrate Apache Spark for distributed processing</li>
  <li>Add weather & holiday features</li>
  <li>Deploy model via API for real-time predictions</li>
  <li>Develop visualization dashboard</li>
</ul>

<hr>

<h2>📂 Repository Structure</h2>
<pre><code>
Midterm-Project/
│
├── src/
│   ├── 01_Data_Cleaning_and_Preprocessing.ipynb
│   ├── 02_ETL_and_Data_Storage.ipynb
│   ├── 03_Modeling_and_Evaluation.ipynb
│   ├── nyc_rides.db
| 
├── data/
│   ├── raw.parquet
│   ├── cleaned.parquet
│
├── architecture/
├── pic/
├── README.md
</code>
</pre>

<hr>

<h2>👥 Team</h2>

<p>
<b>Harshavardhan J</b> – ETL Pipeline & Modeling <br>
<b>Cuthbeth</b> – Data Storage, CRISP-DM & Documentation
</p>

<hr>

<p align="center">
⭐ Distributed & Scalable Data Engineering – Midterm Project ⭐
</p>
