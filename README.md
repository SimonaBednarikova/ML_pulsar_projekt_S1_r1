# Rozpoznanie pulzaru od rádiového šumu

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SimonaBednarikova/ML_pulsar_projekt_S1_r1/blob/main/pulzary_projekt.ipynb)

Projekt z predmetu Machine Learning. Binárna klasifikácia kandidátov z rádioteleskopu: **pulzar (1)** alebo **šum (0)**.

## Obsah
| Súbor | Popis |
|---|---|
| `pulzary_projekt.ipynb` | celý projekt: EDA, príprava dát, 4 modely, ladenie hyperparametrov, porovnanie |
| `pulzary_projekt.pdf` | spustený notebook vo formáte PDF |

## Spustenie
Klikni na tlačidlo **Open in Colab** a daj *Runtime → Run all*. Dáta sa stiahnu automaticky z Kaggle cez `kagglehub`, bez prihlásenia.

## Modely
Logistická regresia, KNN, SVM a Random Forest, ladené cez `GridSearchCV` podľa F1 skóre.

| Model | Accuracy | Precision | Recall | F1 |
|---|---|---|---|---|
| KNN | 0,982 | 0,940 | 0,854 | **0,895** |
| SVM | 0,981 | 0,933 | 0,851 | 0,890 |
| Random Forest | 0,980 | 0,919 | **0,863** | 0,890 |
| Logistická regresia | 0,980 | **0,954** | 0,820 | 0,882 |

## Dáta
Kaggle: [Predicting a Pulsar Star](https://www.kaggle.com/datasets/pavanraj159/predicting-a-pulsar-star). Pôvodný zdroj: R. J. Lyon, *HTRU2*, University of Manchester, [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/372/htru2).
