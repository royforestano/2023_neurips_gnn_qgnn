# Based on the submission: A Comparison Between Invariant and Equivariant Classical and Quantum Graph Neural Networks

Machine learning algorithms are heavily relied on to understand the vast amounts of data from high-energy particle collisions at the CERN Large Hadron Collider (LHC). The data from such collision events can naturally be represented with graph structures. Therefore, deep geometric methods, such as graph neural networks (GNNs), have been leveraged for various data analysis tasks in high-energy physics. One typical task is jet tagging, where jets are viewed as point clouds with distinct features and edge connections between their constituent particles. The increasing size and complexity of the LHC particle datasets, as well as the computational models used for their analysis, greatly motivate the development of alternative fast and efficient computational paradigms such as quantum computation. In addition, to enhance the validity and robustness of deep networks, one can leverage the fundamental symmetries present in the data through the use of invariant inputs and equivariant layers. In this paper, we perform a fair and comprehensive comparison between classical graph neural networks (GNNs) and equivariant graph neural networks (EGNNs) and their quantum counterparts: quantum graph neural networks (QGNNs) and equivariant quantum graph neural networks (EQGNN). The four architectures were benchmarked on a binary classification task to classify the parton-level particle initiating the jet. Based on their AUC scores, the quantum networks were shown to outperform the classical networks. However, seeing the computational advantage of the quantum networks in practice may have to wait for the further development of quantum technology and its associated APIs. 


There are five notebooks in this repository based on:

1. Loading and Sorting the Data
2. GNN and EGNN Models
3. QGNN Model
4. EQGNN Model
5. ROC Curves for all models

There are also

6. Preprocessing (Python file in utils directory)
7. Saved sorted numpy arrays for testing (2.-4.)  (numpy arrays in data directory).
8. Saved sorted numpy arrays for testing (5.)  (numpy arrays in roc_data directory).

To run the first notebook (1.), you need to download the 20 Pythia 8 [https://zenodo.org/records/3164691] files and uncomment the first few lines reading in the 20 data files.

The other notebooks (2.-4.) can be run using (6.-7.).

The notebook (5.) can be run using (8.).
