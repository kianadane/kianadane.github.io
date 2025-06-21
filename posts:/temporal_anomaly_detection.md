---
title: "Temporal Anomaly Detection in Satellite Imagery"
date: 2025-05-01
categories: 
  - Publications
layout: single
---

PDF: [Download](/papers/Temporal_Anomaly_Detection_in_Multi_Spectral_Satellite_Imagery.pdf)

Abstract: This project advances the field of anomaly detection in
remote sensing by analyzing temporal patterns in multispec-
tral satellite imagery. We explored three main approaches:
Functional Principal Component Analysis (fPCA), the Prithvi-
EO-2.0 foundational model (Prithvi), and Continuous Change
Detection and Classification (CCDC). Our main focus was on
the fPCA model, which achieved 66% accuracy and an F1
score of 0.30 for anomaly detection.
Despite challenges—including the need for temporal down-
sampling, artifacts in the Planet.com imagery (such as sensor-
induced banding or haze not attributable to clouds), and limited
ground truth labels (only 3–5% manually annotated)—the
fPCA model demonstrated strong performance, particularly
for sparse time series data. It is computationally efficient,
requiring only 3–4 minutes per site, making it well-suited for
environments where data are regularly updated and the model
must be re-run frequently.
Although Prithvi achieved slightly higher accuracy, its preci-
sion, recall, and F1 scores were lower, and its run times were
highly variable. Nonetheless, with further development and
optimization, Prithvi has the potential to become a competitive
alternative. CCDC performed moderately well, with stable
accuracy across sites, but its sensitivity to input parameters
and reliance on having only a few temporal gaps limited its
performance in noisier datasets.
All three models—fPCA, Prithvi, and CCDC—would bene-
fit from consistent preprocessing and fully harmonized datasets
to enable more direct and fair comparisons. Future work will
focus primarily on enhancing the fPCA and Prithvi models,
with an emphasis on improving noise reduction techniques and
developing more robust anomaly detection algorithms.