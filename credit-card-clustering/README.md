<div align="center">

<h1>Credit Card Customer Segmentation</h1>

<p>
Segmenting credit card users based on financial behavior using PCA and K-Means clustering.
</p>

<p>
<a href="credit_card_clustering_project.html">View Notebook</a> •
<a href="#key-insight">Key Insight</a> •
<a href="#approach">Approach</a>
</p>

</div>

<hr>

<h2>Overview</h2>

<p>
This project applies unsupervised machine learning techniques to segment credit card customers based on their spending patterns, credit usage, and repayment behavior.
</p>

<p>
By transforming raw financial data into structured behavioral dimensions using Principal Component Analysis (PCA), the model identifies distinct customer groups with similar financial characteristics.
</p>

---

<h2 align="center">Cluster Profiles</h2>

<p align="center">
<img src="/images/cluster_segments.png" width="700" alt="Customer Cluster Profiles">
</p>

---

<h2 id="key-insight">Key Insight</h2>

<p>
Customer behavior is driven by a combination of spending intensity, credit dependency, and repayment discipline rather than any single variable.
</p>

<p>
The segmentation reveals clear groups such as low-activity users, high-value spenders, disciplined full payers, and high-risk credit-dependent customers, reflecting real-world financial behavior patterns.
</p>

---

<h2 id="approach">Approach</h2>

<ul>
<li>Data cleaning and preprocessing</li>
<li>Exploratory data analysis</li>
<li>Feature engineering</li>
<li>Feature scaling</li>
<li>Principal Component Analysis (PCA)</li>
<li>K-Means clustering</li>
<li>Cluster interpretation</li>
</ul>

---

<h2>Tools</h2>

<p>
Python • Pandas • NumPy • Seaborn • Scikit-learn • Matplotlib
</p>

---

<h2>Future Improvements</h2>

<ul>
<li>Cluster validation using additional metrics</li>
<li>Deployment via interactive dashboard (Streamlit)</li>
<li>Real-time customer classification pipeline</li>
<li>Integration with business decision systems</li>
</ul>
