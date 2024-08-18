# Graph Resilience Analysis

This repository contains the implementation and analysis of network resilience and community detection using the Email-Eu-core and LastFM datasets. The project evaluates the resilience of networks and communities under various conditions, including node addition and removal, and compares original networks with synthetic models like Chung Lu and UPA.

## Table of Contents
- [Project Overview](#project-overview)
- [Folder Structure](#folder-structure)
- [Datasets](#datasets)
- [Methodology](#methodology)
- [Resilience Analysis](#resilience-analysis)
- [Community Detection](#community-detection)
- [Machine Learning Analysis](#machine-learning-analysis)
- [Installation and Setup](#installation-and-setup)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Project Overview

The purpose of this project is to analyze the resilience of networks, specifically focusing on how they withstand failures and attacks. Using the Email-Eu-core and LastFM datasets, we investigate the structural integrity and robustness of networks through graph theoretical approaches, community detection, and machine learning models.

## Folder Structure
```
.
├── Documentation/
│   ├── Final_report.pdf
│   ├── Literature_Review and EDA.pdf
│   ├── Methodology and Experiments.pdf
│   └── Results Report_final.pdf
├── Email/
│   ├── Data/
│   │   ├── chung_lu_model.gml
│   │   ├── email-Eu-core-department-labels.txt
│   │   ├── email-Eu-core.txt
│   │   ├── email_graph.gml
│   │   ├── email_labels.json
│   │   ├── email_node_features.csv
│   │   └── upa_model.gml
│   ├── src/
│   │   ├── Community_Resilience_Testing.ipynb
│   │   ├── Community_detection.ipynb
│   │   ├── Data_Preprocessing.ipynb
│   │   ├── EDA.ipynb
│   │   ├── Resilience_testing.ipynb
│   │   └── machine_learning_analysis.ipynb
│   ├── EDA_email.ipynb
│   └── Email_network_analysis.ipynb
├── Lastfm_asia/
│   ├── Data/
│   │   ├── ba_model_lastfm.gml
│   │   ├── chung_lu_model_lastfm.gml
│   │   ├── lastfm_asia_edges.csv
│   │   ├── lastfm_asia_features.json
│   │   ├── lastfm_asia_target.csv
│   │   ├── lastfm_graph.gml
│   │   ├── lastfm_node_features.csv
│   │   ├── lastfm_targets_processed.csv
│   │   └── upa_model_lastfm.gml
│   ├── src/
│   │   ├── Community_Resilience_Analysis.ipynb
│   │   ├── Community_detection.ipynb
│   │   ├── Data_Preprocessing.ipynb
│   │   ├── EDA.ipynb
│   │   ├── Resilience_testing.ipynb
│   │   └── machine_learning_analysis.ipynb
│   ├── EDA_lastfm.ipynb
│   └── Lastfm_network_analysis.ipynb
├── LICENSE
├── Users
├── Users.pub
└── .DS_Store
```
## Documentation

- **Final_report.pdf**: The comprehensive final report of the project, including all findings and conclusions.
- **Literature_Review and EDA.pdf**: A detailed literature review and exploratory data analysis report.
- **Methodology and Experiments.pdf**: Documentation of the methodology and experiments conducted during the project.
- **Results Report.pdf**: A summary of the results obtained from the resilience analysis and machine learning experiments.

## Email

- **Data/**: Contains the datasets and graph models for the Email network analysis.
- **src/**: Jupyter notebooks for various stages of analysis, including community detection, resilience testing, and machine learning analysis.
- **EDA_email.ipynb**: Exploratory data analysis specific to the Email dataset.
- **Email_network_analysis.ipynb**: The main notebook for Email network analysis.

## Lastfm_asia

- **Data/**: Contains the datasets and graph models for the LastFM network analysis.
- **src/**: Jupyter notebooks for various stages of analysis, including community detection, resilience testing, and machine learning analysis.
- **EDA_lastfm.ipynb**: Exploratory data analysis specific to the LastFM dataset.
- **Lastfm_network_analysis.ipynb**: The main notebook for LastFM network analysis.

## Other Files

- **LICENSE**: The license file for the project.
- **Users & Users.pub**: Public and private key files.

## Datasets

1. **Email-Eu-core**: This dataset includes email communications within a European research institution, with department labels for each individual.
2. **LastFM Asia**: A social network of LastFM users from Asian countries, including user connections and country information.

## Methodology

The methodology involves preprocessing the datasets, constructing graphs, detecting communities using the Louvain method, and evaluating network resilience under different scenarios using synthetic models (Chung Lu and UPA).

## Resilience Analysis

We performed resilience testing by adding and removing nodes based on various strategies, such as random selection, degree centrality, and betweenness centrality. The analysis compares the original network's resilience against synthetic models.

## Community Detection

Communities within the networks were detected using the Louvain method, which optimizes modularity to identify densely connected subgroups.

## Machine Learning Analysis

We utilized machine learning models, specifically Random Forest and SVM classifiers, to predict node roles and analyze network resilience based on structural features like degree centrality and clustering coefficient.

## Installation and Setup

To set up this project on your local machine:

1. Clone the repository:

   ```bash
   git clone https://github.com/adishdmc/Graph_Resilience_Analysis.git
Navigate to the project directory:
bash
Copy code
cd Graph_Resilience_Analysis
Install the required dependencies:
bash
Copy code
pip install -r requirements.txt
Launch Jupyter Notebook:
bash
Copy code
jupyter notebook
Usage

To use the project:

Navigate to the src/ directory within the Email or Lastfm_asia folders.
Open the Jupyter notebooks to run the analysis.
Follow the steps in each notebook to execute the community detection, resilience testing, and machine learning analysis.
Results

The results of the analysis are documented in the Documentation folder, providing insights into the resilience of the Email and LastFM networks, the effectiveness of synthetic models, and the performance of machine learning classifiers.

Contributing

Contributions are welcome! Please submit a pull request or open an issue if you have suggestions for improvements or would like to contribute to the project.

License

This project is licensed under the MIT License - see the LICENSE file for details.
