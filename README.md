# SOEN-471-MECP-Project <br>
<b> Contributors </b> <br>
Peilin Han, Carmen Pop, Kalinga Swain, Natasha Uwase <br><br>
<b>Project Summary </b> <br><br>
Introduction:<br>
This collaborative project with MECP, a company specializing in medical equipment sales, aims to tackle challenges in SKU analysis and product matching. The datasets are from MECP and 3 other competitors, C6, LifeSupply, and MedicalWarehouse. Each table has product name, price, SKU, and the description of the product, represented as string and float data types. Our primary goal is to address the research objective of matching MECP SKUs with those of competitors, with a particular emphasis on enhancing the efficiency and scalability of the matching process.<br><br>
Approach:<br>
  1.	Data Preprocessing: The initial step will entail preprocessing product information datasets by standardizing attributes like product names, descriptions, and SKUs, while also eliminating inconsistencies and irrelevant data.<br>
  2.	Tokenization and Shingling: Next, we will tokenize the product descriptions into shingles. This step facilitates the generation of a compact representation of the product attributes for efficient comparison.<br>
  3.	MinHash Signature Construction: We will then use MinHashing to construct signatures for each product based on its shingles. Multiple hash functions might be applied to generate a set of minimum hash values, forming the MinHash signature. This process reduces the dimensionality of the data while preserving similarity information.<br>
  4.	Similarity Estimation: We will use MinHash signatures to estimate Jaccard similarity between product pairs, indicating attribute similarity. A threshold on Jaccard similarity scores will determine potential matches.<br>
  5. Comparison: For model comparison needs, we are building a second model to compare the before; here we are just using Lavenshtein distance method with fuzzy string matching algorithm either by using token_sort_ratio or token_set_ratio to calculate the the similarity ratio for each complete sentences of the columns and we append that ratio column creating a new structure which has MECP products, competetion1 products, competetion2 products (identified by unique SKU id); higher ratio denotes higher similarity.
  6.	Validation: Additionally, validation techniques such as manual inspection or ground truth datasets will be used to evaluate the accuracy of the matching algorithm.
<br><br>

<b> Expected Outcomes: </b> <br>
•	Development of a scalable and efficient SKU matching system capable of handling large datasets.<br>
•	Improved accuracy in identifying matching products across different datasets, leading to enhanced inventory management and operational efficiency.<br>
•	Reduction in manual effort required for product matching, allowing for more streamlined business processes.<br>
•	Comparing the models to choose the best and efficient for the assigned task.<br>


