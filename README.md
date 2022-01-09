# Gait classification using smartphone sensors

I used a simple architecture LSTM network to produce activity classification using raw signals from accelerometer and gyrometer of a smartphone.
This can de used to enchance people mobility
## Data content
### Data source 📊
Data used in this project were created by
```
Jorge L. Reyes-Ortiz(1,2), Davide Anguita(1), Luca Oneto(1) and Xavier Parra(2)
1 - Smartlab, DIBRIS - UniversitÃ  degli Studi di Genova, Genoa (16145), Italy.
2 - CETpD - Universitat PolitÃ¨cnica de Catalunya. Vilanova i la GeltrÃº (08800), Spain
har '@' smartlab.ws
www.smartlab.ws
```
They can be downloaded [here](http://archive.ics.uci.edu/ml/datasets/Smartphone-Based+Recognition+of+Human+Activities+and+Postural+Transitions).
### Class content
<img src="./assets/classes.png" alt="drawing" width="800"/>

### Visualization of activities for one subject
That might be an error in the processing of raw data since there are many non-labelled sequences. It might be also caused by technical check of the user while doing the record, which are not labelled (something like 'sensor/signal check by operator').
![](./assets/run.png)
## Training
### Training metrics
  Train/val loss steadily decreasing. Good F1-score (0.926) for such a simple model without additionnal data care (over/under sampling)(normalization off signal was already done by data operator).
![](./assets/train_metrics.png)
### Evaluation
Since we have a high class imbalance, F1 score is more relevant for evaluation than ROC AUC because a high F1 score considers both precision and recall. Higher ROC AUC does not necessarily mean a better classifier in case of class imbalance.
![](./assets/confusion.png)

# To be done next 🛠
- [ ] Data balancing and re-training.
- [ ] Scripts.
- [ ] User classification.
- [ ] 3D trajectory reconstruction and visualization.
- [ ] Hyperparameter optimization.
- [X] Training and evaluation metrics check. 
