# DL-Cardiac-Signal-Classifier
Cardiac signal classifier using deep learning models, allows categorization between:
- Normal
- Noise
- Arrhythmia.

## Data 
In this project, we work with ECG signals. Each one of these signals is a 1D signal with 2049 elements. 
<p align="center">
  <img src="https://github.com/Konat23/DL-Cardiac-Signal-Classifier/assets/68023761/42326c84-dfa7-4d22-912a-5184a151aae3" width="450" height="300">
</p>

Labels can be 
- 0 for normal signals
- 1 for signals with cardiac arrhythmia
- 2 for signals with noise.
<p align="center">
  <img src="https://github.com/Konat23/DL-Cardiac-Signal-Classifier/assets/68023761/aade0d23-b476-49aa-9aa6-0d7355f8ac29" width="400" height="300">
</p>

## Preprocessing 
Z-score normalization was applied to the ECG signal.

$Z = \frac{x - \mu}{\sigma}$
## Split data 
- Training Data [84205] (72%)
- Validation Data [9357] (8%)
- Testing Data [23391] (20%)
## Model 
El modelo keras esta disponible en es [link](https://drive.google.com/file/d/1DHFXWbuIzwr4dLW_SoMtqhWleBaizDsi/view).
<p align="center">
  <img src="https://github.com/Konat23/DL-Cardiac-Signal-Classifier/assets/68023761/6df4bc74-0b74-476f-b13c-890a9e7b5913" width="500" height="300">
</p>

## Results 
Performance metrics in classification. Macro average. Cross-validation with 5 folder.
| Métrica   | Media  | Desv. Estándar |
|-----------|--------|----------------|
| Precisión | 0.8953 | ±0.00876       |
| Recall    | 0.8731 | ±0.03617       |
| F1-Score  | 0.8819 | ±0.02362       |

Confusion Matrix
<p align="center">
  <img src="https://github.com/Konat23/DL-Cardiac-Signal-Classifier/assets/68023761/67ab6016-b961-47ea-b967-a75f6eb90b3c" width="300" height="300">
</p>
