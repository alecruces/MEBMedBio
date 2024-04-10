# Minimum Enclosing Ball for Anomaly Detection on Biological Data
---

##  Description 
The Minimum Enclosing Ball (MEB) is a problem with a wide range of applications, of which anomaly detection is a prominent one. In this project, the goal is to understand and implement the MEB problem through three different variants of the Frank-Wolfe algorithm: the Pairwise Frank-Wolfe, the Blended Pairwise Conditional Gradient, and an adaptation using Away-Steps. Through the convergence analysis, it is concluded that all of the algorithms have linear convergence when applied to the MEB problem. To test and compare their performances, after exploring the theoretical results that appear in the literature, the implemented algorithms are used to find anomalies in the context of four different medical and biological problems using several metrics, focusing on recall. Finally, it is observed that the third algorithm (from Yildirim (2008)) consistently outperforms the others across all four datasets in terms of computational time and number of iterations.

<p align="center">
<img src="https://github.com/alecruces/MEBMedBio/assets/67338986/87be068b-c18d-4b52-a352-9a95c50bcf2a" alt="MEB2" style="width:400px;height:auto;"/>
</p>

##  Keywords
 Anomaly detection, biological data
 
##  Data
* Breast cancer dataset: https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic
* Breast cancer gene expression dataset: https://archive.ics.uci.edu/dataset/401/gene+expression+cancer+rna+seq
* Vertebral column pathology dataset: https://archive.ics.uci.edu/dataset/212/vertebral+column
* Maternity risk dataset: https://archive.ics.uci.edu/dataset/212/vertebral+column

## Methods
* Three variants of the Frank-Wolfe algorithm: Pairwise Frank-Wolfe, Blended Pairwise Conditional Gradient and an adaptation using Away-Steps.
* Minimum Enclosing Ball Problem

## Software 
* Python
  
## Files  
* Code: `MEB_BPCG.ipynb`
* Report: `Report.pdf`
* Presentation: `Presentation.pdf`

