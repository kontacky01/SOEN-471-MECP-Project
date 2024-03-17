# SOEN-471-MECP-Project <br>
<b> Contributors </b> <br>
Peilin Han, Carmen Pop, Kalinga Swain, Natasha Uwase <br>
<b> Project Summary </b> <br><br>
Introduction<br>
This collaborative project with MECP, a company specializing in medical equipment sales, aims to tackle challenges in SKU analysis and product matching using a blend of traditional methods and innovative techniques. The dataset, sourced from files like mecp_scraper.py and life_supply.py, likely includes product information such as name, description, SKU, and price, represented as string and float data types. While the dataset's size remains undisclosed, our focus lies in resolving the research objective of Matching MECP SKUs with Competitors' SKUs, a critical task for inventory management, pricing strategy, and market analysis.<br><br>
Methodology<br>
To achieve this objective, we propose a comprehensive approach involving SKU comparison between MECP and its competitors. Leveraging big data analytics, our methodology will combine the Levenshtein distance calculation, early termination, parallelization, and min hashing for efficient and accurate SKU comparison. The Levenshtein distance metric quantifies dissimilarity between SKU datasets. With early termination techniques we can conserve computational resources by halting computation beyond a predefined threshold. Also, we plan to use parallelization to distribute workload across multiple processors, expediting distance computation.<br><br>
Post distance calculation, we will use min hashing to identify matching or similar SKUs efficiently. With a time complexity of O(N+M), where N is the size of MECP's dataset and M is the size of the competitor's dataset, min hashing offers scalability. This hashing technique generates fixed-size signatures for SKUs, facilitating rapid comparison across large datasets.<br><br>
Results<br>
To assess SKU matching accuracy, we will employ a rigorous evaluation framework, including precision, recall, and F1 score, comparing identified matches against ground truth data. Cross-validation experiments ensure algorithm robustness across diverse datasets and scenarios.<br><br>
In conclusion, our project presents a comprehensive approach to SKU comparison, crucial for MECP's competitive edge. By integrating Levenshtein distance, early termination, parallelization, and min hashing, we aim to provide MECP with actionable insights into its product landscape compared to competitors. This methodology not only scales to handle MECP's vast dataset but also ensures high accuracy in SKU matching, empowering informed decision-making in the consumer electronics market.
