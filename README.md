# Gait classification using smartphone sensors
I used a simple architecture LSTM network to produce activity classification from XYZ accelerometer and gyrometer raw signals.
Visualization of activities for one subject
![](./assets/run.png)
Results of training
![](./assets/train_metrics.png)
Evaluation
![](./assets/confusion.png)

# Data 📊
Data used in this project were created by
```
Jorge L. Reyes-Ortiz(1,2), Davide Anguita(1), Luca Oneto(1) and Xavier Parra(2)
1 - Smartlab, DIBRIS - UniversitÃ  degli Studi di Genova, Genoa (16145), Italy.
2 - CETpD - Universitat PolitÃ¨cnica de Catalunya. Vilanova i la GeltrÃº (08800), Spain
har '@' smartlab.ws
www.smartlab.ws
```
They can be downloaded [here](http://archive.ics.uci.edu/ml/datasets/Smartphone-Based+Recognition+of+Human+Activities+and+Postural+Transitions).

# To be done next 🛠
- [ ] 3D trajectory reconstruction and visualization
- [ ] Hyperparameter optimiszation.
- [ ] Proper evaluation.

 
