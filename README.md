# KMSWT-Term-Project

## Mapping the Academic Landscape
Authors: Aditya Chawla (19CH3AI12), Apurva Anand (19EE10008), Pauras Meher (19ME3AI21), Saurabh Mishra (19IE3AI20)

This project aims to create a knowledge graph of professors and their research areas at IIT Kharagpur using data scraping, preprocessing, and clustering techniques. The resulting knowledge graph can provide insights into the research areas and expertise of professors in various departments and enable students to efficiently locate and identify suitable professors to undertake research projects within their respective areas of interest.

## Methodology
### Data Scraping
Data was scraped from the IIT Kharagpur website for each department, including the names and research areas of the faculty members. The requests and BeautifulSoup modules were used to extract the necessary information from the HTML content of the web pages.

### Clustering
After data scraping, related research topics were clustered into broad research areas using LDA and BERTopic algorithms. Lemmatization was performed to reduce words to their base form. The number of topics was selected based on the coherence score.

### Topics Visualization
Topics were visualized to better understand the clusters.

### CSV File Generation
Two dictionaries were generated and used to create a dataframe containing the name, department, and broad research area of the professors. The resulting CSV file was generated for further analysis.

### Ontology Design
The Cellfie tool was used to create an ontology from the generated CSV file. The resulting ontology contained three classes - Professor, Department, and Research_Area - and four object properties - hasDepartment, hasResearchArea, isDepartmentOf, and isResearchAreaOf.
