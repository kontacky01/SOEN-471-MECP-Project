# SOEN-471-MECP-Project <br>
<b> Contributors </b> <br>
Peilin Han, Carmen Pop, Kalinga Swain, Natasha Uwase <br>
<b> Project Summary </b> <br>
We're collaborating with MECP, a company specializing in the sale of medical equipment.This project aims to address various challenges in the domain of SKU analysis and product matching, utilizing a combination of traditional methods and machine learning techniques. We speculate that the dataset comprises product information extracted from files such as mecp_scraper.py and life_supply.py, featuring fields including product name, description, SKU, and price, likely represented as string and float data types. The dataset's size remains undisclosed at this stage.
Research Objectives:
1.	Comparing and Matching MECP SKUs with Competitors' SKUs:
•	Subtask 1: Comparing. We plan to employ a hybrid approach, combining Jaccard similarity with shingling for initial dataset reduction, followed by the application of Levenshtein distance for detailed comparison. The computational intensity of Jaccard similarity will be managed through MapReduce frameworks, facilitating parallel comparison across multiple nodes for scalability. This sequential integration balances accuracy with computational efficiency.
•	Subtask 2: Matching. We will use min-hashing for SKU matching. We chose it for its optimal computational complexity.
2.	Mapping/Matching SKUs Using Machine Learning Models: We plan to employ Decision Trees, Random Forests, and clustering algorithms (k-means or hierarchical) for SKU mapping, leveraging the power of machine learning to enhance matching accuracy and efficiency.
3.	Predicting Prices for Matched Products (Matched SKUs): We plan to use linear regression, Decision Trees, and Random Forests to predict prices for matched products, providing valuable insights into pricing dynamics and competitive positioning. Next, we'll evaluate the loss of the three models to determine which one best fits our data and yields the most precise price predictions. </b>
This project integrates diverse methodologies, spanning from traditional similarity metrics to advanced machine learning models, to tackle challenges in SKU comparison, matching, and price prediction. Through this comprehensive approach, we aim to optimize product analysis and enhance strategic decision-making in competitive market landscapes.
