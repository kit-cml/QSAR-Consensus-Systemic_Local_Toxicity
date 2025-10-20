Development of a Consensus-Based QSAR Models for Enhanced Multi-Endpoint Prediction of Systemic and Local Toxicities

FAUZAN SYARIF NURSYAFI¹, MUHAMMAD ADNAN PRAMUDITO², YUNENDAH NUR FUADAH³, and KI MOO LIM¹,⁴,⁵**
¹Computational Medicine Lab, Department of Medical IT Convergence Engineering, Kumoh National Institute of Technology, Gumi, 39177, Republic of Korea
²Computational Medicine Lab, Department of IT Convergence Engineering, Kumoh National Institute of Technology, Gumi, 39177, Republic of Korea
³Telecommunication Engineering Study Program, School of Electrical Engineering, Telkom University Main Campus, Bandung, Indonesia
⁴Computational Medicine Lab, Department of Biomedical Engineering, Kumoh National Institute of Technology, Gumi, 39177, Republic of Korea
⁵Meta Heart Co., Ltd, Gumi, 39253, Republic of Korea

Corresponding authors: kmlim@kumoh.ac.kr
, yunendah@telkomuniversity.ac.id

Overview

This repository contains the code for developing and evaluating QSAR (Quantitative Structure–Activity Relationship) models for multi-endpoint chemical toxicity prediction. The models employ a consensus-based approach integrating multiple molecular fingerprints (Morgan, MACCS, APF, RDKit+CDK), physicochemical descriptors, and machine learning algorithms (Random Forest, XGBoost, SVM). Cross-validation ensures robust and reliable model performance.

The repository includes:

Data preprocessing and descriptor calculation

Model training using both fingerprint and physicochemical features

Cross-validation (manual and original splits)

Evaluation of both individual and consensus models

All computations are performed in Python using the following libraries: RDKit, CDK-pywrapper, TensorFlow, scikit-learn, NumPy, and Pandas. Fixed package versions ensure reproducibility and consistent results across environments.

Repository Structure
Development and Evaluation Code/
│
├── Descriptor Computation_Preprosesing data.ipynb
├── Model_Evaluation.ipynb
├── Training_ML_Dermal_PhysicochemicalProperties_5foldCrossvalidation.ipynb
├── Training_ML_Fingerprint_10foldCrossvalidation.ipynb
├── Manual Split Dataset/
├── Original Split Dataset/

Usage

Compute descriptors: Use Descriptor Computation_Preprosesing data.ipynb to calculate molecular fingerprints and physicochemical descriptors for your dataset.

Train models: Use Training_ML_Fingerprint_10foldCrossvalidation.ipynb and Training_ML_Dermal_PhysicochemicalProperties_5foldCrossvalidation.ipynb for model training and cross-validation.

Evaluate models: Use Model_Evaluation.ipynb to perform consensus evaluation and generate metrics for all models.
