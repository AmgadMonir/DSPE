# DSPE
Dynamic Self-paced Ensemble for Imbalance-aware Learning

In this paper, we introduce the **Dynamic Self-paced Ensemble (DSPE)**, as a novel heuristic algorithm that integrates meta-learning-based ensembles (i.e Self-Paced Ensemble) with dynamic ensemble selection techniques for **handling imbalanced data**. Taking advantages of both: **<ins>Meta-Learning</ins>** (to learn undersampling strategy from the majority class), and **<ins>Dynamic Ensemble Selection</ins>** (to estimate the local competences of base estimators around the location of unseen test sample). Meta-learning-based ensembles solve the limitations of oversampling/undersampling strategies that employ distance-based metrics like KNN. By Meta-learning, the training feedback information is used to capture the underlying distribution between classes; considering intricacies of imbalanced data, such as noise and class overlap. Employing dynamic ensemble selection excels imbalance-aware learning ***by leveraging the local competencies of base classifiers within specific regions of the feature space for the neighbourhood of the unseen test sample.*** The proposed method solves the limitations of existing static ensemble methods that depend on the majority voting of all estimators, emphasizes the need for adaptive strategies that can effectively handle imbalanced data.

The authors present experimental results demonstrating the effectiveness of DSPE over static ensemble methods, showcasing its ability to enhance performance and stability across different ensemble sizes. 

**Contribution:**
- **(1)**: [An analysis of the imbalanced learning capability of Meta-learning based ensemble that could be affected by
the type of its base classifier]
- **(2)**: [An analysis of coupling Meta-learning-based ensembles with dynamic ensemble selection for handling imbalanced data classification tasks.]
- **(3)**: [ Examining how various ensemble sizes influence the effectiveness of dynamic selection in imbalanced learning.]


## Installation

Follow these steps to install and set up the project locally:

1. **Clone the Repository**

   First, clone this repository to your local machine:
   ```bash
   git clone https://github.com/AmgadMonir/DSPE.git

2. **Navigate to the Project Directory Change into the project directory**
   ```bash
    cd DSPE
   
3. **install Requirement**  .
    The required Python dependencies are:
     + imbalanced_ensemble
     + imbalanced-learn==0.11.0
     + deslib
     + pandas
     + sklearn
     + matplotlib 
     ```bash
     
     pip install imbalanced-ensemble
     pip install imbalanced-learn==0.11.0
     pip install deslib


# checking the following documentations if necessary

  + **DES** : https://deslib.readthedocs.io/en/latest/index.html
  + **Imbalanced-Ensemble** : https://imbalanced-ensemble.readthedocs.io/en/latest/
  + **Imbalanced-Learn** : https://imbalanced-learn.org/stable/
