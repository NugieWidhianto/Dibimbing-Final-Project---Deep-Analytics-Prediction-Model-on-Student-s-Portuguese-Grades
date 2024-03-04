# :zap: Dibimbing Final Project - Deep Analytics & Prediction Model on Student's Portuguese Grades at 2 School in Portugal :zap:

> Link for the dataset : https://www.kaggle.com/datasets/whenamancodes/student-performance/data?select=Portuguese.csv

## Project Introduction
Project ini dibuat untuk mengetahui apa-apa saja yang menjadi pengaruh terhadap **performa siswa** di sekolah menengah / SMP dan membuat **model prediksi dan 'Deep Analytics'** terhadap performa siswa disekolah.

https://camo.githubusercontent.com/55e4079e69ec5d8246620ecff24ed093877ab0f9011e71d8dec0a2c460c886ab/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f507974686f6e2d3337373641423f7374796c653d666f722d7468652d6261646765266c6f676f3d707974686f6e266c6f676f436f6c6f723d7768697465

Dalam **skala bisnis**, hal ini dapat digunakan dan difungsikan dalam skala kecil maupun besar, dengan contoh:
- **Skala Kecil** : Perbaikan sistem pendidikan dan pengajaran pada suatu sekolah.
- **Skala Besar** : Perbaikan sistem pendidikan suatu daerah/kota/provinsi/negara, dalam hal pengajaran dan pemerhatian terhadap aspek-aspek baik secara akademik ataupun diluar akademik terhadap performa siswa disekolah.

## Business Questions
### 1. Alasan / pengaruh terhadap nilai siswa?
- H0 - Nilai siswa hanya dipengaruhi oleh alasan generik yang berhubungan dengan akademik
- H1 - Nilai siswa juga dipengaruhi oleh alasan diluar akademik siswa
### 2. Apakah jenis kelamin mempengaruhi nilai siswa?
- H0 - Nilai siswa TIDAK dipengaruhi oleh jenis kelamin
- H1 - Terdapat PERBEDAAN NILAI antar jenis kelamin siswa
### 3. Apakah Pekerjaan dan Tingkat Edukasi orang tua mempengaruhi nilai siswa?
- H0 - Nilai siswa TIDAK dipengaruhi oleh Pekerjaan ataupun tingkat edukasi orang tua siswa
- H1 - Terdapat relevansi dan perbedaan yang signifikan antar nilai siswa dengan jenis pekerjaan dan tingkat pendidikan orang tua yang berbeda
### 4. Apakah kegiatan ekstrakurikuler mempengaruhi nilai siswa secara negatif?
- H0 - Kegiatan Ekstrakurikuler membuat nilai siswa menjadi lebih buruk dibanding mereka yang tidak memiliki kegiatan ekstrakurikuler
- H1 - Kegiatan Ekstrakurikuler tidak mempengaruhi nilai siswa
- H2 - Kegiatan Ekstrakurikuler membuat nilai siswa menjadi lebih baik dibanding mereka yang tidak memiliki kegiatan ekstrakurikuler
### 5. Apakah Hubungan Romantis mempengaruhi nilai siswa?
- H0 - Nilai siswa TIDAK dipengaruhi oleh Hubungan Romantis siswa
- H1 - Nilai siswa DIPENGARUHI oleh Hubungan Romantis siswa

## Libraries 
Libraries Python yang paling banyak digunakan pada project ini adalah **Pandas, Numpy, Matplotlib dan Seaborn**. Adapula Libraries lain-nya yang saya gunakan untuk keperluan lain dalam project ini seperti :

```python
import pandas as pd
import numpy as np
pd.set_option('display.max_columns', None)
import matplotlib.pyplot as plt
import seaborn as sns
import scipy.stats as stats
from sklearn.model_selection import train_test_split , cross_val_score , GridSearchCV
from sklearn.preprocessing import StandardScaler, MinMaxScaler

from sklearn.neighbors import KNeighborsClassifier
from sklearn.metrics import confusion_matrix,accuracy_score,ConfusionMatrixDisplay,precision_score, recall_score,roc_curve,roc_auc_score
from sklearn.feature_selection import SelectKBest
from sklearn.feature_selection import chi2
from mlxtend.feature_selection import SequentialFeatureSelector
from sklearn.metrics import classification_report
from sklearn.ensemble import RandomForestClassifier
from sklearn.model_selection import GridSearchCV
from sklearn.metrics import accuracy_score, confusion_matrix, ConfusionMatrixDisplay
from sklearn.svm import SVC
from sklearn.metrics import roc_curve, roc_auc_score

import warnings
warnings.filterwarnings('ignore')
```
