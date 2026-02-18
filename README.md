# Spectral Clustering Analysis: Performance Comparison with K-Means

## 📊 Project Overview

This repository contains the implementation and analysis of spectral clustering algorithms as part of an engineering thesis comparing clustering methodologies. The project evaluates the performance of spectral clustering algorithms—both standard and normalized Laplacian-based—against the traditional k-means algorithm on the classic Iris dataset.

## 🎯 Thesis Abstract

As data size and complexity continue to grow, efficient clustering techniques are essential for meaningful analysis. Having provided necessary theoretical base, this thesis evaluates the performance of spectral clustering algorithms—both standard and normalized Laplacian-based—against the traditional k-means algorithm. While k-means proves computationally efficient for simpler datasets, its accuracy declines as data complexity increases. Spectral clustering methods, particularly the normalized Laplacian approach, demonstrate superior clustering quality, achieving the highest Adjusted Rand Index (ARI). However, this comes at a higher computational cost. The findings suggest that k-means remains preferable for low-dimensional datasets, whereas spectral clustering is more suitable for high-dimensional, complex data requiring greater accuracy.

## 📁 Project Structure

```
SpectralClustering/
├── Main.ipynb              # Primary analysis notebook with complete implementation
├── Research.ipynb          # Exploratory data analysis and research development  
├── Engineering Thesis.pdf # Complete thesis document
└── README.md              # This file
```

## 🔬 Key Features

### Algorithms Implemented
- **K-Means Clustering**: Traditional centroid-based clustering algorithm
- **Standard Spectral Clustering**: Using unnormalized graph Laplacian
- **Normalized Spectral Clustering**: Using normalized graph Laplacian

### Analysis Components
- **Data Exploration**: Comprehensive analysis of the Iris dataset
- **Performance Metrics**: Adjusted Rand Index (ARI), Silhouette Score
- **Computational Analysis**: Time complexity and memory usage comparison
- **Visualization**: Clustering results and algorithm performance plots
- **Graph Theory**: Construction and analysis of graph Laplacians
- **Eigenvalue Analysis**: Spectral decomposition and eigenvector examination

## 📚 Technical Implementation

### Dependencies
```python
numpy
pandas
matplotlib
seaborn
scikit-learn
scipy
memory_profiler
```

### Key Methodologies

1. **Graph Construction**: k-nearest neighbors graph generation
2. **Laplacian Computation**: Both standard and normalized variants
3. **Eigendecomposition**: Computing eigenvalues and eigenvectors
4. **Dimensionality Reduction**: Projection onto eigenspace
5. **Performance Evaluation**: Multiple clustering quality metrics

## 📈 Key Findings

- **K-Means**: Computationally efficient but limited accuracy on complex data
- **Standard Spectral Clustering**: Improved clustering quality over k-means
- **Normalized Spectral Clustering**: Highest clustering accuracy (best ARI scores)
- **Trade-offs**: Superior accuracy comes with increased computational cost

## 🚀 Usage

### Running the Analysis

1. **Main Analysis**:
   ```bash
   jupyter notebook Main.ipynb
   ```

2. **Research & Development**:
   ```bash
   jupyter notebook Research.ipynb
   ```

### Dataset Requirements
- The project uses the Iris dataset (`iris.csv`)
- Ensure the dataset path is correctly set in the notebooks

## 📊 Results Summary

The analysis demonstrates that:
- **Low-dimensional datasets**: K-means is preferable due to computational efficiency
- **High-dimensional, complex data**: Spectral clustering provides superior accuracy
- **Normalized Laplacian approach**: Achieves the highest clustering quality metrics

## 🎓 Academic Context

This work is part of an engineering thesis focusing on unsupervised learning and graph-based clustering algorithms. The research contributes to understanding the practical trade-offs between computational efficiency and clustering accuracy in different data scenarios.

## 📄 Documentation

For detailed theoretical background, methodology, and comprehensive results, refer to the complete thesis document: `Engineering Thesis.pdf`

## 🛠️ Future Work

- Extension to larger, more complex datasets
- Implementation of additional spectral clustering variants
- Analysis of parameter sensitivity
- Comparison with modern deep clustering approaches

---

*This project demonstrates the practical application of spectral clustering theory and provides insights into algorithm selection for different data characteristics.*
