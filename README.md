# Partition and Clustering R Code

<h2>Introduction</h2>
  <p>This repository contains R code for partitioning and clustering data using various algorithms. It includes implementations for data preprocessing, partitioning, and clustering techniques.</p>

  <h2>Installation</h2>
  <p>To use this code, make sure you have the following libraries installed in your R environment:</p>
  <ul>
    <li>readxl</li>
    <li>NbClust</li>
    <li>factoextra</li>
    <li>cluster</li>
    <li>fpc</li>
  </ul>
  <p>You can install these libraries using the following commands:</p>
  <pre><code>install.packages("readxl")
    install.packages("NbClust")
    install.packages("factoextra")
    install.packages("cluster")
    install.packages("fpc")
  </code></pre>

  <h2>Usage</h2>
  <ol>
    <li>Clone this repository to your local machine:</li>
  </ol>
  <pre><code>git clone https://github.com/your-username/partition-and-clustering-r.git</code></pre>
  
  <ol start="2">
    <li>Open the R script containing the code.</li>
    <li>Modify the file path in the script to point to your dataset.</li>
    <li>Run the script in your preferred R environment (e.g., RStudio).</li>
  </ol>

  <h2>Sub Task 1</h2>
  <h3>Data Preprocessing</h3>
  <ul>
    <li>The script reads an Excel file containing the dataset.</li>
    <li>It handles missing values by replacing them with the mean of their respective columns.</li>
    <li>Duplicates are removed from the dataset.</li>
    <li>Outliers are detected and removed using the IQR method.</li>
    <li>The dataset is then scaled for further analysis.</li>
  </ul>

  <h3>Clustering</h3>
  <ul>
    <li>The optimal number of clusters is determined using the NbClust package, which provides various indices such as the elbow method, gap statistic, and silhouette method.</li>
    <li>K-Means clustering is performed on the scaled dataset with the optimal number of clusters.</li>
    <li>Cluster analysis results, including cluster centers, assignments, and evaluation metrics, are provided.</li>
    <li>Cluster plots and silhouette plots are generated for visual inspection.</li>
  </ul>

  <h2>Sub Task 2</h2>
  <h3>Principal Component Analysis (PCA)</h3>
  <ul>
    <li>Principal Component Analysis is applied to the scaled dataset.</li>
    <li>The number of principal components is chosen based on the cumulative proportion of variance explained.</li>
    <li>NbClust is used again to determine the optimal number of clusters after PCA transformation.</li>
    <li>K-Means clustering is performed on the transformed dataset.</li>
    <li>Cluster analysis results and evaluation metrics are provided.</li>
    <li>Cluster plots and silhouette plots are generated for visual inspection.</li>
  </ul>

  <h2>Conclusion</h2>
  <p>This R code provides a comprehensive approach to partitioning and clustering data, including preprocessing steps and evaluation of clustering results. It can be applied to various datasets for exploratory data analysis and pattern discovery.</p>

  <h2>Contributing</h2>
  <p>Contributions are welcome! If you have any suggestions or improvements, feel free to open an issue or submit a pull request.</p>

  <h2>License</h2>
  <p>This project is licensed under the <a href="LICENSE">MIT License</a>.</p>
