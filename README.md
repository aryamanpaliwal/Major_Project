# Major_Project
This project aimed to survey the realm of heart-stroke discovery and the potential of utilizing Quantum Computing to upgrade this critical facet of healthcare. Traditional designs for detecting heart strokes frequently encounter challenges related to their veracity and computational complexity. To overcome these restraints, Our system influences the unique possessions of quantum computing, particularly the phenomenon of destructive interference, to guarantee that clustering everything works correctly and is doable for requests in real-world questions. By joining the K-means clustering accompanying the quantum principles, our approach aims to provide a more accurate and adept discovery of heart stroke.
In our study, we conducted inclusive experiments utilizing various datasets of patients with accompanying heart stroke to judge the performance. The findings show that our method outperforms established patterns and former quantum methods, exhibiting superior veracity and adeptness in heart-stroke discovery. 
The ability to correctly and efficiently discover heart stroke using quantum-driven approaches can bring about proper mediation, upgraded patient outcomes, and diminished healthcare costs, which in a proper sequence will lead to a lower number of afterlife events from heart stroke. Moreover, the verdicts shed light on the potential of quantum computing to advance accuracy cure, and personalized healthcare.

## Dataset Description
The Stroke Prediction Dataset offers a rich collection of records aimed at understanding and predicting the occurrence of strokes. This dataset comprises a range of relevant attributes that provide insights into various aspects related to strokes. The dataset consists of 12 features, including the target attribute that signifies whether a patient has experienced a stroke (Target = "1") or not (Target = "0").
The dataset encompasses diverse information about each patient, including their age, sex, hypertension status, presence of heart disease, whether they are married or not, the type of work they are engaged in, their residence type, average glucose level, body mass index (BMI), smoking status, and the availability of relevant medical history. Each of these features contributes to the comprehensive nature of the dataset, enabling researchers and data scientists to explore the potential risk factors and patterns associated with strokes.
To ensure the dataset's compatibility with machine learning algorithms, preprocessing steps are required, including data cleansing, handling missing values, and feature engineering techniques such as encoding categorical variables. By applying these preprocessing techniques, researchers can unlock the dataset's potential and utilize machine learning algorithms to develop predictive models that can aid in stroke prevention and treatment strategies. The next sections describe the various preprocessing steps, such as Dimensionality reduction, outlier rejection, feature scaling, etc. used during the course of our study. 

# Quantum K-means Algorithm
## Introduction
The Quantum K-means Algorithm is an extension of the classical K-means clustering algorithm that utilizes quantum computing techniques for clustering data points. This algorithm employs quantum principles such as superposition and interference to process and analyze data in a quantum state representation.

## Algorithm Overview
1. Input:
   - Convert input data points X = [x1, x2, x3, ..., xN] into a quantum state |ψ⟩ using amplitude encoding.
   - Specify the initial cluster centroids: |1⟩, |2⟩, ..., |k⟩.

2. Distance Calculation using Destructive Interference:
   - Calculate the distance (Dist) using the formula:
     Dist = Norm * sqrt(2 * P|1⟩), where Norm is the normalization factor and P|1⟩ is the probability of measuring the state |1⟩.

3. Repeat the following steps until convergence:
   a. Cluster Updation:
      - Assign each data point (xn) to the nearest cluster using the Nearest-Cluster function:
        Ck = Cluster(Xn) = argk min(k=1,K) {gnk || xn − wk ||^2}, where Ck represents the k-th cluster.
   
   b. Centroid Updation:
      - Update the centroid (wk) of each cluster by calculating the mean of the data points assigned to that cluster:
        wk = (1/Ck) ∑n(gnk xn)

4. Output:
   - The algorithm converges when the cluster assignments and centroids stabilize.
   - The final output consists of K clusters, each containing the respective data points (Ck).

## Usage
1. Provide the input data points in the form of a classical dataset.
2. Initialize the cluster centroids and encode the data points into a quantum state.
3. Execute the Quantum K-means Algorithm by repeating the cluster updation and centroid updation steps until convergence.
4. Retrieve the final clusters and respective data points as the algorithm's output.

## Requirements
- Qiskit: A quantum computing framework for implementing quantum algorithms.
- Python: Programming language used to run the algorithm.
