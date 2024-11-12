# Minimum Enclosing Ball for Anomaly Detection on Biological Data

> Analyzing biological data for anomaly detection using Minimum Enclosing Ball (MEB) and variations of the Frank-Wolfe algorithm.

<p align="center">
<img src="https://github.com/alecruces/MEBMedBio/assets/67338986/87be068b-c18d-4b52-a352-9a95c50bcf2a" alt="MEB2" style="width:400px;height:auto;"/>
</p>

##  Keywords
 Anomaly detection, biological data
 
---

## Table of Contents

1. [About the Project](#about-the-project)
2. [Key Features](#key-features)
3. [Key Results](#key-results)
4. [Data Overview](#data-overview)
5. [Methodology](#methodology)
6. [Screenshots and Graphs](#screenshots-and-graphs)
7. [Technologies Used](#technologies-used)
8. [Setup & Installation](#setup--installation)
9. [Usage](#usage)
10. [Contributing](#contributing)
11. [License](#license)
12. [Contact](#contact)

---

### About the Project

This project explores the Minimum Enclosing Ball (MEB) problem and its applications in anomaly detection across biological datasets. We implement three Frank-Wolfe algorithm variants: Pairwise Frank-Wolfe, Blended Pairwise Conditional Gradient (BPCG), and a (1+ϵ)-approximation using Away-Steps. These methods are evaluated for computational efficiency, convergence rates, and anomaly detection performance in biological contexts.

### Key Features

- **Anomaly Detection**: Identification of anomalies in biological datasets.
- **Efficient Algorithms**: Implementation of three Frank-Wolfe-based algorithms, each offering unique advantages in convergence and computational performance.
- **Biological Data Application**: Practical application in detecting anomalies in datasets like breast cancer, gene expression, vertebral pathology, and maternity risk.

### Key Results

- **Convergence**: All three algorithms demonstrated linear convergence on the MEB problem.
- **Best Performance**: The (1+ϵ)-approximation (Yildirim 2008) showed superior computational performance, especially on high-dimensional datasets.
- **Recall Metrics**: Focused on recall as the benchmark for anomaly detection, achieving optimal recall values for most datasets.

### Data Overview

This study uses four biological datasets focused on anomaly detection. Links to each dataset:

- **Breast Cancer**: [Wisconsin Diagnostic Breast Cancer Dataset](https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)
- **Breast Cancer Gene Expression**: [Gene Expression Cancer RNA-Seq](https://archive.ics.uci.edu/dataset/401/gene+expression+cancer+rna+seq)
- **Vertebral Column Pathology**: [Vertebral Column Dataset](https://archive.ics.uci.edu/dataset/212/vertebral+column)
- **Maternity Risk**: [Maternity Risk Dataset](https://archive.ics.uci.edu/dataset/863/maternal+health+risk)

### Methodology

We apply three variants of the Frank-Wolfe algorithm to solve the MEB problem:

- **Pairwise Frank-Wolfe**: An efficient, projection-free algorithm.
- **Blended Pairwise Conditional Gradients (BPCG)**: An optimized variant that minimizes swap steps.
- **(1+ϵ)-Approximation with Away-Steps**: An approximation method designed for efficient handling of large datasets.

Each algorithm is evaluated on convergence rates, computational time, and accuracy metrics (primarily recall) in detecting anomalies.

### Screenshots and Graphs

1. **MEB for Maternity Risk dataset**  

  <p align="center">
  <img width="715" alt="MEB" src="https://github.com/user-attachments/assets/480b1d3e-cbb4-4d43-8053-b1e55075be19">
  </p>

2. **Computational Time and Iterations (Table)**  
   Summary table comparing computational time and iterations for each algorithm across datasets.

   | Dataset              | Algorithm | Time (ms)  | Iterations |
   |----------------------|-----------|------------|------------|
   | Breast Cancer        | PFW       | 664.50     | 1,484      |
   | Breast Cancer        | BPCG      | 647.54     | 2,998      |
   | Breast Cancer        | MEB(A)    | 49.15      | 44         |
   | Gene Expression      | PFW       | 369,959.76 | 100,000    |
   | Gene Expression      | BPCG      | 397,067.57 | 100,000    |
   | Gene Expression      | MEB(A)    | 2,116.30   | 44         |

### Technologies Used

> 🛠️ Emphasizing the primary tools and libraries utilized.

- ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white): Main programming language.
- **Optimization Algorithms**: Implemented variations of the Frank-Wolfe algorithm.
- **nbviewer Link**: [View the Jupyter Notebook](https://nbviewer.org/github/alecruces/MEBMedBio/blob/main/MEB_BPCG.ipynb)

### Setup & Installation

Clone the repository and install dependencies:

```bash
# Clone the repository
git clone https://github.com/username/MEBMedBio.git

# Navigate to the project directory
cd MEBMedBio

# Install dependencies
pip install -r requirements.txt
```

## Files  
* Code: `MEB_BPCG.ipynb`
* Report: `Report.pdf`
* Presentation: `Presentation.pdf`

### Usage

The repository includes the following files:

- **`MEB_BPCG.ipynb`**: Jupyter notebook with the full workflow, from data preprocessing to algorithm implementation and evaluation.
- **`Report.pdf`**: Detailed report on methodology, algorithmic analysis, and findings.
- **`Presentation.pdf`**: Summary presentation of key findings and insights.

To run the project, open `MEB_BPCG.ipynb` in Jupyter Notebook or [view it on nbviewer](https://nbviewer.org/github/alecruces/MEBMedBio/blob/main/MEB_BPCG.ipynb).

### Contributing

Contributions are welcome! Please see the contributing guidelines for more details.
