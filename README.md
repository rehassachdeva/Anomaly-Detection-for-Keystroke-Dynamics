# Comparing Anomaly-Detection Algorithms for Keystroke Dynamics

### What is keystroke dynamics (or keystroke biometrics)?

- study of whether people can be distinguished by their typing rhythms.

### Applications

- acting as an electronic fingerprint
- access-control and authentication mechanism
- detecting computer-based crimes

### Existing work
Comparing Anomaly-Detection Algorithms for Keystroke Dynamics
- http://www.cs.cmu.edu/~maxion/pubs/KillourhyMaxion09.pdf
- http://www.cs.cmu.edu/~keystroke/

### Data
Refer to DataDescription.txt

### Detectors implemented and Results

| Detector                       | Average Equal-Error Rate | Standard deviation of EER |
|--------------------------------|--------------------------|---------------------------|
| Manhattan Scaled Detector      | 0.0945                   | 0.068375                  |
| Outlier Count (z-score)        | 0.103167                 | 0.07691                   |
| Nearest Neighbor (Mahalanobis) | 0.1075                   | 0.06213                   |
| SVM (one-class)                | 0.12068                  | 0.0586                    |
| Manhattan Filtered             | 0.12535                  | 0.081299                  |
| Mahalanobis                    | 0.1337                   | 0.06678                   |
| Mahalanobis Normed             | 0.1337                   | 0.06678                   |
| Manhattan                      | 0.15                     | 0.09                      |
| K-Means                        | 0.1559                   | 0.072                     |
| Neural Network (auto-assoc)    | 0.16417                  | 0.0914199                 |
| Euclidean                      | 0.16929                  | 0.0931429                 |
| Euclidean Normed               | 0.2107                   | 0.1174                    |
| Neural Network (standard)      | 0.6551                   | 0.1866                    |

### Files for detectors

- Neural Network (standard) - NeuratNetStandardDetector.ipynb
- Neural Network (auto-assoc) - NeuratNetAutoAssocDetector.ipynb
- Svm - svm.ipynb
- KMeans - kmeans.ipynb
- Other detectors - KeystrokeDynamics.ipynb