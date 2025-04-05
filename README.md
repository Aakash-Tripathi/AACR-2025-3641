# Predicting treatment outcomes using cross-modality correlations in multimodal oncology data

**Abstract Number: 3641**

**Authors:**  
Aakash Tripathi<sup>1,2,†</sup>, Asim Waqas<sup>1,3</sup>, Yasin Yilmaz<sup>2</sup>, Ghulam Rasool<sup>1,2,3</sup>  
<sup>1</sup> Machine Learning Department, Moffitt Cancer Center, Tampa, FL  
<sup>2</sup> Electrical Engineering Department, University of South Florida, Tampa, FL  
<sup>3</sup> Department of Biostatistics and Bioinformatics, Moffitt Cancer Center, Tampa, FL

**Contact:** Aakash.Tripathi@moffitt.org

---

![Project overview diagram](/docs/assets/overview.png)

Accurate prediction of treatment outcomes in oncology requires modeling the intricate relationships across diverse data modalities. This study investigates cross-modality correlations by leveraging imaging and clinical data curated through the Multimodal Integration of Oncology Data System (MINDS) and HoneyBee frameworks to uncover actionable patterns for personalized treatment strategies. Using data from over 11,400 cancer patients, we developed a machine learning pipeline that employs advanced embedding techniques to capture associations between radiological imaging phenotypes and histopathological features, aiming to predict survival outcomes and treatment efficacy. The HoneyBee framework played a key role in preprocessing and feature extraction, using foundation models for imaging and text data. Radiological imaging, such as computed tomography (CT) and magnetic resonance imaging (MRI), was transformed into high-dimensional embeddings with vision transformers and convolutional neural networks. Clinical data, including electronic health records and pathology reports, was structured into embeddings using biomedical language models. These embeddings ensured standardization and cross-modal alignment while capturing modality-specific features. HoneyBee also applied data augmentation and preprocessing, such as stain normalization and tokenization, to maintain data quality. MINDS provided a scalable, metadata-driven architecture for integrating datasets like patient demographics and treatment histories, supporting seamless ingestion, harmonization, and storage. Together, these frameworks created a unified, multimodal dataset optimized for predictive modeling and resilient to missing data. In training, embeddings were combined through late-stage fusion techniques to generate unified patient-level representations in latent space. These representations were used to train machine learning models, including gradient-boosted trees and neural networks, for survival analysis and treatment response prediction. Testing was conducted using stratified cross-validation to ensure generalizability across cancer subtypes and demographic groups. Results demonstrated significant predictive correlations, such as imaging-derived phenotypes linked to histopathological indicators of treatment response. The machine learning pipeline achieved a 12% improvement in concordance indices over unimodal approaches, underscoring the enhanced accuracy of cross-modality learning.

## TODO:

- [ ] Build a survival outcome and treatment efficacy cohort
- [ ] Generate embeddings for all modalities in the cohort
