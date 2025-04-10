# mushroom-classification
🍄 Mushroom Classification Project
Overview
During a summer fieldwork internship, I frequently encountered mushrooms in the wild. While some coworkers attempted to identify them based on visual traits, accurate classification — especially distinguishing edible from poisonous varieties — remained a challenge. This project investigates whether data science techniques can help identify distinguishing features of mushrooms and determine their edibility status based on common traits.

Essential Question
Can visual or structural traits of mushrooms be used to accurately determine if a mushroom is edible or poisonous?

Project Goals
Use dimensionality reduction (PCA and UMAP) to explore visual patterns in mushroom traits.

Identify whether specific features or combinations of features can help classify mushrooms as edible or poisonous.

Visualize data to assess clustering and overlap between classes.

Key Findings
PCA Analysis: While PCA revealed some variance across traits like stem width and cap diameter, it did not yield a clear division between edible and poisonous mushrooms.

UMAP Visualization: UMAP showed localized clustering of mushroom types but also demonstrated significant overlap between classes.

Traits & Classification: Some features (e.g., stem color) appeared to correlate with classification in isolated cases, but no single or simple combination of features was sufficient for reliable classification.

Real-world Insight: Consistent with field experience, data confirms that mushroom identification often requires more nuanced cues (smell, texture, spore print) not captured in the dataset.

Methods
Dimensionality Reduction:

PCA (Principal Component Analysis): Used to understand the variance across all features.

UMAP (Uniform Manifold Approximation and Projection): Used for visualization of clustering and structure in lower-dimensional space.

Data Processing:

Encoded categorical variables.

Normalized/standardized features as needed for PCA/UMAP.

Visualization:

Created plots showing distribution of mushrooms by edibility status along principal components and UMAP embeddings.

Dataset
Source: UCI Mushroom Dataset

Contains 8124 instances of mushrooms with 22 attributes (e.g., cap shape, gill color, stem surface).

Target label: edible (e) or poisonous (p).

Tools & Libraries
Python

pandas, numpy

scikit-learn

umap-learn

matplotlib, seaborn

Limitations
Dataset lacks certain real-world identification traits (smell, texture, spore print).

Many edible and poisonous mushrooms share nearly identical visual characteristics.

The model and visualizations are not reliable for field identification.

Conclusion
This project supports the idea that while mushrooms of the same class may share traits, there is significant overlap between edible and poisonous types. Field identification remains complex and should not rely solely on visual traits or simple heuristics.

📁 Project Structure
bash
Copy
Edit
mushroom-classification/
│
├── data/                     # Cleaned/preprocessed dataset
├── notebooks/                # Jupyter notebooks for EDA, PCA, UMAP
├── plots/                    # Generated visualizations
├── src/                      # Scripts for data processing and modeling
├── README.md                 # Project overview
└── requirements.txt          # List of dependencies
⚠️ Disclaimer
Do not use this model or analysis to identify wild mushrooms.
Incorrect identification can be dangerous or fatal. This project is for educational and exploratory data science purposes only.
