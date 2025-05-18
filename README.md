📌 Parameter Optimization of SVM
🔍 Objective
To optimize the parameters of the NuSVC (Support Vector Machine for classification) algorithm using different kernel functions and values of nu, across multiple randomized data splits. The aim is to identify the best performing configuration and analyze convergence behavior.

📊 Dataset
Name: Wine Dataset (from UCI ML Repository)

Classes: 3 wine cultivars (multi-class)

Features: 13 numeric features

Samples: 178 total

⚙️ Optimization Details
SVM Model: NuSVC from sklearn.svm

Hyperparameters Tuned:

kernel: linear, poly, rbf, sigmoid

nu: Random float from 0.01 to 0.99

Optimization Strategy:

10 random 70/30 train-test splits (S1 to S10)

100 iterations per sample with random parameter trials

Evaluation Metric: Accuracy

📁 Files Included
File	Description
parameter_optimization.ipynb	Main Colab notebook performing optimization
optimized_svm_results.csv	Table with best accuracy and parameters for each sample
convergence_plot_best_svm.png	Convergence graph of best performing sample
README.md	This file

📈 Results
Table 1: Best Accuracy and Parameters per Sample
Sample	Best Accuracy	Kernel	Nu
S1	e.g. 0.94	rbf	0.27
...	...	...	...

(Refer to optimized_svm_results.csv for full details)

📉 Convergence Plot


This plot shows how accuracy evolved over 100 iterations in the best-performing sample.

✅ Conclusion
The best accuracy was achieved using the NuSVC model with kernel='...' and nu=....

Different random splits significantly impacted the results.

The convergence graph helped visualize optimization effectiveness over iterations.
