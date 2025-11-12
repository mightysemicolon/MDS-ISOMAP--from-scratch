This project presents a clean, from-scratch implementation of Classical Multidimensional Scaling (MDS) and Isomap, two foundational techniques in manifold learning and dimensionality reduction. Both algorithms are designed to uncover the underlying geometric structure of high-dimensional or distance-based data and represent it in a low-dimensional Euclidean space for visualization and analysis.

The notebook begins with reading a pairwise distance matrix (for example, distances between cities) and proceeds to compute spatial embeddings using both MDS and Isomap.
MDS relies on double centering of the squared distance matrix to form the B matrix, followed by eigendecomposition to extract principal coordinates that best preserve global pairwise relationships.
Isomap, in contrast, constructs a k-nearest neighbor graph and applies Dijkstra’s algorithm to estimate geodesic distances, thus capturing nonlinear manifold structures that MDS may overlook.

*The implementation includes:

Step-by-step derivation of both algorithms using NumPy and SciPy

Construction of geodesic distance graphs with scikit-learn’s kneighbors_graph

Interactive 2D visualizations with labeled points and adjustable rotation for alignment

Comparison of MDS and Isomap outputs to highlight differences in preserving local and global geometry

*Techniques Used

Linear and nonlinear dimensionality reduction

Eigen decomposition and spectral embedding

Graph-based distance approximation
