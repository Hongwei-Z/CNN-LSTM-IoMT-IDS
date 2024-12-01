# CNN-LSTM IoMT IDS
### CSCI 6505 Group Project
### Author: Hongwei Zhang & Koil Jat Chong
#### Enhancing Intrusion Detection in Healthcare IoMT Devices Using the CNN-LSTM Model

Dataset: [CIC IoMT dataset 2024](https://www.unb.ca/cic/datasets/iomt-dataset-2024.html) (Attack Vectors in Healthcare Devices - A Multi-Protocol Dataset for Assessing IoMT Device Security)

Files:    
1. Dataset Preprocessing: [Preprocessing.ipynb](Preprocessing.ipynb)     
2. Under Sampling: [CNN-LSTM_UnderSampling.ipynb](CNN-LSTM_UnderSampling.ipynb)   
3. Multi Classification: [CNN-LSTM_MultiClassification.ipynb](CNN-LSTM_MultiClassification.ipynb)  
4. Binary Classification: [CNN-LSTM_BinaryClassification.ipynb](CNN-LSTM_BinaryClassification.ipynb)

Model Architecture:   
CNN_LSTM_Model(   
(cnn): Sequential(   
    (0): Conv1d(1, 64, kernel_size=(3,), stride=(1,), padding=(1,))   
    (1): ReLU()   
    (2): MaxPool1d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)   
    (3): Conv1d(64, 128, kernel_size=(3,), stride=(1,), padding=(1,))   
    (4): ReLU()   
    (5): MaxPool1d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)   
  )   
  (lstm): LSTM(128, 256, num_layers=2, batch_first=True, dropout=0.2)    
  (fc): Linear(in_features=256, out_features=2, bias=True)   
)

Results:   
Metrics: Multi Classification, Binary Classification   
Accuracy:	0.862394,	0.997873   
Precision:	0.864817,	0.997869   
Recall:	0.862676,	0.997885   
F1-score:	0.863027,	0.997873   


Reference:  
1. [Different ways to combine CNN and LSTM networks for time series classification tasks](https://medium.com/@mijanr/different-ways-to-combine-cnn-and-lstm-networks-for-time-series-classification-tasks-b03fc37e91b6)     
2. [Kaggle CNN+LSTM](https://www.kaggle.com/code/yunsuxiaozi/cnn-lstm)