## CNN-LSTM IoMT IDS
### Enhancing Intrusion Detection in Healthcare IoMT Devices Using the CNN-LSTM Model
### Author: Hongwei Zhang & Koil Jat Chong

**Abstract:** Intrusion detection in Internet of Medical Things (IoMT) devices presents unique challenges due to diverse communication protocols and evolving security threats. This study proposes a hybrid deep learning approach combining Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks for enhanced intrusion detection in healthcare IoMT devices. Our CNN-LSTM model leverages CNN for spatial feature extraction and LSTM for temporal pattern analysis, particularly suited for IoMT-generated data patterns. Using the recently proposed CICIoMT2024 dataset, which covers three primary IoMT communication protocols (Bluetooth, WiFi, and MQTT), we conducted comprehensive evaluations across 18 different attack types categorized into five major classes: DDoS, DoS, Reconnaissance, MQTT, and Spoofing. The experimental results demonstrate the model's excellent performance, achieving 86.24% accuracy in multi-classification tasks and 99.79% accuracy in binary classification scenarios. The model maintains consistently high performance across other metrics, with precision, recall, and F1-scores of 0.865, 0.863, and 0.863 respectively for multi-classification, and 0.998 across all metrics for binary classification.

**Dataset:** [CIC IoMT dataset 2024](https://www.unb.ca/cic/datasets/iomt-dataset-2024.html)

**Multi Classification:** [CNN-LSTM_MultiClassification.ipynb](CNN-LSTM_MultiClassification.ipynb)  
**Binary Classification:** [CNN-LSTM_BinaryClassification.ipynb](CNN-LSTM_BinaryClassification.ipynb)