# Research-projects-analysis-NLP

# Analysis of Research Projects with NLP techniques

This repository contains the analysis of various Natural Language Processing (NLP) research projects. The project applies several NLP preprocessing techniques, feature extraction methods, and classification models to analyze and draw insights from research datasets. The main goal is to process and classify text data to extract meaningful insights from a large dataset of research projects.

## Project Structure
- `NLP_Researches_Analysis.ipynb`: Jupyter Notebook with the data preprocessing, feature extraction (using techniques like TFIDF and Word2Vec), and analysis using classification models such as Random Forest and BERT.

## Setup

### Requirements
- Python 3.7 or higher
- Jupyter Notebook

### Usage
Open the Jupyter Notebook to view and run the code:

jupyter notebook NLP_Researches_Analysis.ipynb

In the own notebook there is cell for the import of the neccessary libraries.

## Methods and Techniques
- **Data Preprocessing**: Text cleaning, tokenization and lemmatization.
- **Feature Extraction**: Text Vectorization Techniques by implementing TFIDF, Word2Vec, BERT embeddings.
- **Classification Models**: Random Forest and BERT for document classifcation.

## Dataset

The dataset is available at [projects.xlsx](./projects.xlsx). It comprises **35,378 entries** detailing research projects funded by the European Commission within the H2020 Program. The dataset includes fields such as:

- `projectID`: Unique identifier for each project.
- `acronym`: Project acronym.
- `title`: Project title.
- `summary`: Project summary.
- `startDate` & `endDate`: Project start and end dates.
- `totalCost`: Total cost of the project.
- `ecMaxContribution`: Maximum contribution from the European Commission.
- `countryContr`: Funding received by each participating country.
- `coordinatorCountry`: Country coordinating the project.
- `euroSciVocCode`: Thematic code for the project, with categories available in the [SciVocCodes.xlsx](./SciVocCodes.xlsx) file.
- `publicationID` & `patentID`: Identifiers for publications and patents related to the project.

This data was sourced from CORDIS, available on the EU Open Data Portal [here](https://data.europa.eu/data/datasets/cordish2020projects?locale=es).

### Dataset Structure

The dataset consists of several columns representing different aspects of the text data, such as:
- **Text**: The main content for analysis.
- **Labels/Categories**: The categorization assigned to each text sample, indicating its type, topic, or sentiment (if applicable).

## Adapting the Code for Other Applications

The code in this project is designed for NLP analysis of research summaries but can be adapted for other domains by modifying key steps in the data preprocessing and vectorization process:

1. **Adjust Data Preprocessing**: 
   - Modify the code to accommodate different fields or text structures specific to the new dataset.
   - Adjust tokenization, stopword removal, or text normalization settings based on the characteristics of the new text data, such as technical jargon or common abbreviations in fields like healthcare or environmental studies.

2. **Update Vectorization and Embedding Methods**:
   - Select embeddings relevant to the new context, such as **BioBERT** for biomedical text or **SciBERT** for scientific literature, to capture domain-specific language nuances.
   - If the data requires a different kind of similarity measure or text clustering, modify vectorization methods to focus on those aspects.

3. **Revise Classification and Clustering Models**:
   - Adapt or retrain classification algorithms based on the new data categories. For example, in a healthcare application, categories might include disease types or treatment methods.
   - If clustering is applied, modify the number of clusters and distance metrics to better fit the new dataset’s underlying structure.

4. **Tailor Visualizations**:
   - Update the visualizations to highlight metrics or insights that are most relevant to the target domain. For instance, healthcare applications might benefit from visualizing clusters by patient outcome or treatment success, while environmental studies might focus on regional trends.


## Acknowledgments
This project was developed as part of the Master's program in Telecommunications Engineering at Universidad Carlos III de Madrid (UC3M). Special thanks to my collaborators [Elena Almagro]([https://linkedin.com/in/elenaalmagro/) and [Juan Muñoz](https://www.linkedin.com/in/juan-munoz-villalon/) for their valuable contributions and teamwork throughout the project.
