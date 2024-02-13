<p align="center">
    <h1 align="center">Graph Neural Network and Machine Learning Analysis of Functional Neuroimaging for Understanding Schizophrenia</h1>
</p>
<p align="center">
	<img src="https://img.shields.io/github/license/smruthig/Schizophrenia_Detection?style=flat&color=0080ff" alt="license">
	<img src="https://img.shields.io/github/last-commit/smruthig/Schizophrenia_Detection?style=flat&logo=git&logoColor=white&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/smruthig/Schizophrenia_Detection?style=flat&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/smruthig/Schizophrenia_Detection?style=flat&color=0080ff" alt="repo-language-count">
<p>
<p align="center">
		<em>Developed with the software and tools below.</em>
</p>
<p align="center">
	<img src="https://img.shields.io/badge/TensorFlow-FF6F00.svg?style=flat&logo=TensorFlow&logoColor=white" alt="TensorFlow">
	<img src="https://img.shields.io/badge/scikitlearn-F7931E.svg?style=flat&logo=scikit-learn&logoColor=white" alt="scikitlearn">
	<img src="https://img.shields.io/badge/Jupyter-F37626.svg?style=flat&logo=Jupyter&logoColor=white" alt="Jupyter">
	<img src="https://img.shields.io/badge/Keras-D00000.svg?style=flat&logo=Keras&logoColor=white" alt="Keras">
	<img src="https://img.shields.io/badge/SciPy-8CAAE6.svg?style=flat&logo=SciPy&logoColor=white" alt="SciPy">
	<br>
	<img src="https://img.shields.io/badge/Plotly-3F4F75.svg?style=flat&logo=Plotly&logoColor=white" alt="Plotly">
	<img src="https://img.shields.io/badge/Python-3776AB.svg?style=flat&logo=Python&logoColor=white" alt="Python">
	<img src="https://img.shields.io/badge/pandas-150458.svg?style=flat&logo=pandas&logoColor=white" alt="pandas">
	<img src="https://img.shields.io/badge/NumPy-013243.svg?style=flat&logo=NumPy&logoColor=white" alt="NumPy">
</p>
<hr>

##  Quick Links

> - [ Overview](#overview)
>   - [ Background](#background)
>   - [ Results](#results)
>   - [ Conclusions](#conclusions)
> - [ Repository Structure](#repository-structure)
> - [ Instructions](#instructions)
>   - [ Installation Locally](#installation-locally)
>   - [ Running Schizophrenia_Detection](#running-schizophrenia_detection)
> - [ Contributing](#contributing)
> - [ License](#license)

---

## Overview
### Background
Graph representational learning can detect topological patterns by leveraging both the network structure as well as nodal features. The basis of our exploration involves the application of graph neural network architectures and machine learning to resting-state functional Magnetic Resonance Imaging (rs-fMRI) data for the purpose of detecting schizophrenia. Our study uses single-site data to avoid the shortcomings in generalizability of neuroimaging data obtained from multiple sites.

### Results
The performance of our graph neural network models is on par with that of our machine learning models, each of which is trained using 69 graph-theoretical measures computed from functional correlations between various regions of interest (ROI) in a brain graph. Our deep graph convolutional neural network (DGCNN) demonstrates a promising average accuracy score of 0.82 and a sensitivity score of 0.84.

### Conclusions
This study provides insights into the role of advanced graph theoretical methods and machine learning on fMRI data to detect schizophrenia by harnessing changes in brain functional connectivity. The results of this study demonstrate the capabilities of using both traditional ML techniques as well as graph neural network-based methods to detect schizophrenia using features extracted from fMRI data. The study also proposes two methods to obtain potential biomarkers for the disease, many of which are corroborated by research in this area and can further help in the understanding of schizophrenia as a mental disorder.

---

##  Repository Structure

```sh
└── Schizophrenia_Detection/
    ├── Code
    │   ├── 1. Feature Generation
    │   │   ├── Global Binary Measures.ipynb
    │   │   ├── Global Weighted Measures.ipynb
    │   │   ├── Local Binary Measures.ipynb
    │   │   └── Local Weighted Measures.ipynb
    │   ├── 2. Threshold Comparison
    │   │   └── XGB for threshold comparison.ipynb
    │   ├── 3. Data Augmentation
    │   │   └── Data Augmentation Distribution sampling.ipynb
    │   ├── 4. Machine Learning
    │   │   └── All ML Models 10 fold CV.ipynb
    │   ├── 5. Graph Neural Network
    │   │   ├── DGCNN model 10 Fold CV.ipynb
    │   │   ├── DGCNN model.ipynb
    │   │   ├── DGCNN with node2vec.ipynb
    │   │   └── GCN model 10 fold CV.ipynb
    │   └── 6. Biomarker Detection
    │       ├── RLF feature selection.ipynb
    │       └── SpeCo.ipynb
    ├── README.md
    └── requirements.txt
```
---

## Instructions

The research paper can be found at [this link](https://link.springer.com/article/10.1186/s12868-023-00841-0).  
  
The data can be found at [this link](https://drive.google.com/drive/folders/1gNZOscYTzWxbGBtgI3Au3NiWDWOYHUpK).  
  
Ensure that you have installed the colab plugin on your google account if you want to run the code on google colab. To run the code on google colab, first right-click on the folder and select add shortcut to drive. After that, simply open and run any of the files. All the required package installations have been included in the code.

In order to run the code locally or in a virtual environment, the paths have to be changed accordingly. For example- `/content/drive/MyDrive/SUPPLEMENTARY CODE/Data/Metadata/phenotypic_data.csv` would change to `/SUPPLEMENTARY CODE/Data/Metadata/phenotypic_data.csv`. If absolute paths are required for the environment, add the required prefix before the modified path.

If you want to run the code locally on your system, create a virtual environment using Anaconda and run the requirements.txt file.

The preprocessed data is sufficient to run the given code files. However, the original data can be obtained from the UCLA repository.

###  Installation Locally

1. Clone the Schizophrenia_Detection repository:

```sh
git clone https://github.com/smruthig/Schizophrenia_Detection
```

2. Change to the project directory:

```sh
cd Schizophrenia_Detection
```

3. Install the dependencies:

```sh
pip install -r requirements.txt
```

###  Running `Schizophrenia_Detection`

Use the following command to run Schizophrenia_Detection using Jupyter:

```sh
jupyter notebook
```

---

##  Contributing

Contributions are welcome! Here are several ways you can contribute:

- **[Submit Pull Requests](https://github.com/smruthig/Schizophrenia_Detection/pulls)**: Review open PRs, and submit your own PRs.
- **[Report Issues](https://github.com/smruthig/Schizophrenia_Detection/issues)**: Submit bugs found or log feature requests for the `Schizophrenia_Detection` project.

<details closed>
    <summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your github account.
2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
   ```sh
   git clone https://github.com/smruthig/Schizophrenia_Detection
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to GitHub**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.

Once your PR is reviewed and approved, it will be merged into the main branch.

</details>

---

#  License

This project is protected under the [MIT License](https://opensource.org/license/mit/). 

---

