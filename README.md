# PRRpred: A Hybrid Model for Predicting Pattern Recognition Receptors Using Evolutionary Information

PRRpred is a computational web server developed for predicting Pattern Recognition Receptors, also known as PRRs, from protein sequences.

Pattern Recognition Receptors are important components of the innate immune system. They recognize pathogen-associated molecular patterns and damage-associated molecular patterns, helping the immune system detect infection, tissue damage, and inflammation. PRRpred uses similarity-based search, machine learning, and evolutionary information to classify proteins as PRRs or non-PRRs.

Web Server: http://webs.iiitd.edu.in/raghava/prrpred/



## Citation

Kaur, D., Arora, C., and Raghava, G. P. S. A Hybrid Model for Predicting Pattern Recognition Receptors Using Evolutionary Information. Frontiers in Immunology, 11, 71, 2020.

https://doi.org/10.3389/fimmu.2020.00071

This tool and dataset is also available on Zenodo 


## About the Research

Pattern Recognition Receptors are germline-encoded immune receptors that recognize conserved molecular patterns present in pathogens or damaged host cells. These receptors play a major role in innate immunity and help initiate inflammatory and antimicrobial responses.

Major classes of PRRs include:

- Toll-like receptors
- NOD-like receptors
- RIG-I-like receptors
- C-type lectin receptors
- Scavenger receptors
- Mannose receptors
- Peptidoglycan recognition proteins
- Secreted PRRs such as collectins, ficolins, and pentraxins

PRRs are involved in pathogen recognition, inflammation, autoimmune disorders, cancer, immunodeficiency, and vaccine adjuvant research. PRRpred was developed to computationally identify PRRs from protein sequences and support innate immunity research.

Data Compilation: PRR sequences were collected from PRRDB 2.0, while non-PRR sequences were obtained from Swiss-Prot. After removing identical sequences, the final dataset contained 179 unique PRRs and 274 non-PRRs.

Methodology: PRRpred uses a hybrid prediction strategy combining BLAST-based similarity search with machine learning models trained on protein sequence composition and evolutionary information.



## Key Features

### 1. PRR Prediction

Predictive Modeling: Allows users to submit protein sequences and predict whether they are likely to be Pattern Recognition Receptors.

Composition-Based Prediction: Uses amino acid composition-based models to classify PRRs and non-PRRs.

Evolutionary Information-Based Prediction: Uses PSSM-400 composition profiles generated from PSI-BLAST to capture evolutionary information from protein sequences.

Accuracy: The best hybrid model combining BLAST and PSSM-based Random Forest achieved 91.39% accuracy, MCC 0.82, and AUROC 0.95.



### 2. Similarity and Machine Learning Modules

BLAST-Based Search: Uses sequence similarity search to identify query proteins similar to known PRRs or non-PRRs.

Machine Learning Prediction: Uses classifiers such as Random Forest, Support Vector Machine, Logistic Regression, Extra Trees, K-Nearest Neighbor, and Multi-Layer Perceptron.

Hybrid Prediction: Combines BLAST similarity search with machine learning scores to improve prediction performance and handle cases where BLAST alone gives no hit.



### 3. Integrated Web-Bench

Composition-Based Module: Allows users to predict PRRs using amino acid composition-based models.

Evolutionary Information Module: Allows users to predict PRRs using PSSM-based evolutionary features.

Hybrid and Non-Hybrid Options: Users can choose either only machine learning-based prediction or hybrid prediction combining BLAST and machine learning.

User-Friendly Interface: PRRpred provides a responsive web interface compatible with desktops, tablets, and smartphones.



## Applications

Innate Immunity Research: PRRpred can help researchers identify proteins involved in innate immune recognition.

PRR Annotation: The tool can assist in annotating newly sequenced proteins as PRRs or non-PRRs.

Vaccine Adjuvant Research: Since PRRs are important targets for vaccine adjuvant design, PRRpred can support immunoinformatics-based vaccine studies.

Host-Pathogen Interaction Studies: PRRpred can help identify receptors involved in pathogen recognition and immune signaling.

Therapeutic Target Discovery: PRRs are linked with inflammation, autoimmune disorders, cancer, and immunodeficiency, so PRRpred may support target discovery in immune-related diseases.



## Contact and Authors

Prof. Gajendra P. S. Raghava  
Corresponding Author  

Email: raghava@iiitd.ac.in  

Department of Computational Biology  
Indraprastha Institute of Information Technology Delhi  
New Delhi, India  



## Support

This work was supported by the J. C. Bose Fellowship from the Department of Science and Technology, Government of India.

The authors also acknowledge Indraprastha Institute of Information Technology Delhi for financial support and fellowships.
