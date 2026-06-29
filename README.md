# phishing-detection-nepal
Bilingual phishing detection for Nepali Digital Wallets(eSewa, Khalti) using ML.

Machine learning research detecting phishing SMS and URLs targeting eSewa and khalti users in Nepal using both English and Nepali text.

## Results
> **Note:** This is proof-of-concept study using a small, manually constructed dataset (110 Samples).
> Results demonstrate pipeline feasibility and methodology rather than production scale performance.

## Overview
This research addresses a gap in phishing detection literature since no published system exists for bilingual(English/Nepali) phishing detection.

### SMS Phishing Detection
|
Model
|
AUC-ROC
|
Recall
|
F1-Score
|
|
-------
|
------
|
-----
|
------
|
|
Logistic Regression
|
1.0000
|
1.0000
|
1.0000
|
1.0000
|
1.0000
|
|
Random Forest
|
0.9722
|
0.8333
|
0.8333
|
0.8333
|
0.8333
|
|
XGBoost
|
1.0000
|
1.0000
|
1.0000
|
1.0000
|
1.0000
|

### URL Phishing Detection
|
Model
|
AUC-ROC
|
Precision
|
Recall
|
F1-Score
|
|
-----
|
----
|
-----
|
-----=
|
|
Logistic Regression
|
1.0000
|
1.0000
|
1.0000
|
1.0000
|
|
Random Forest
|
1.0000
|
1.0000
|
1.0000
|
1.0000
|
|
XGBoost
|
1.0000
|
1.0000
|
1.0000
|
1.0000
|

### Language Specific Analysis
Best model(logistic Regression) accuracy by language:
-English: 100.0 %
-Nepali: 100.0 %

## Limitations
This study uses a small, manually constructed dataset(60 SMS, 50 URLs) due to the absence of any public Nepali Phishing dataset. While results show the full pipeline; bilingual text preprocessing, TF-IDF + hand-crafted feature engineering, URL structural analysis and multi-model comparision - the near perfect scores reflect the dataset's small size rather than claims of production grade accuracy. This work should be read as a methodology demonstration and foundation for future research on larger, real-world datasets.
