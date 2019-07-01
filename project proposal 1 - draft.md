# Anomaly Detection on Multivariate Time Series Data

## The Problem

Multivariate time series data is common in today's world, in IT, finance, industry, medical, smart devices... There's a need to effectively detect anaomaly with the data, which is collected in real time ranging from a few channels of small dataset to high-requency million-feature industry sensor data. Many times statistical approaches and traditional machine learning methods are good choices, such as in forecasting. However, over the years, deep learning have been explored and it shown better performance in some data from complex domains.

## The Experiment

In this project, I am going to explore traditional machine learning methods and deep learning methods on multivariate time-series dataset(s) to see if it can efficiently detect anomaly. For example, GRU (Gated recurrent units) and LSTM (long short-term memory) can help discover correlations among time sequences; CNN (convolutional neural network) combined with autoencoder can be used to construct signature matrices. A mix and match is also possible.

The data is unlabeled so it is unsupervised learning. It is a classification problem where the model has to decide if there is a anomaly within a given period of time. It is also a regression problem from a forecasting point of view. Data is highly imbalanced and may not come with anomaly. For experiment, I might hand craft some data or find a dataset with known anomaly. A web interface is likely to be included.

## The Data

I will be using the [gas sensor data](https://archive.ics.uci.edu/ml/datasets/Gas+sensor+array+temperature+modulation) from the UCI machine learning repository. There are a few datasets, I might use just one of them or a few of them, here is an example unlabeled dataset, it has 4 million samples. There are smaller and bigger datasets.

```
Time (s),CO (ppm),Humidity (%r.h.),Temperature (C),Flow rate (mL/min),Heater voltage (V),R1 (MOhm),R2 (MOhm),R3 (MOhm),R4 (MOhm),R5 (MOhm),R6 (MOhm),R7 (MOhm),R8 (MOhm),R9 (MOhm),R10 (MOhm),R11 (MOhm),R12 (MOhm),R13 (MOhm),R14 (MOhm)
0.0000,0.0000,49.7534,23.7184,233.2737,0.8993,0.2231,0.6365,1.1493,0.8483,1.2534,1.4449,1.9906,1.3303,1.4480,1.9148,3.4651,5.2144,6.5806,8.6385
0.3090,0.0000,55.8400,26.6200,241.6323,0.2112,2.1314,5.3552,9.7569,6.3188,9.4472,10.5769,13.6317,21.9829,16.1902,24.2780,31.1014,34.7193,31.7505,41.9167
```

## Resources

Domino or AWS with GPU. Details will come later.

## References
- [Anomaly detection](https://en.wikipedia.org/wiki/Anomaly_detection)
- [A Deep Neural Network for Unsupervised Anomaly Detection and Diagnosis in Multivariate Time Series Data](https://arxiv.org/abs/1811.08055)
- [FuseAD: Unsupervised Anomaly Detection in Streaming Sensors Data by Fusing Statistical and Deep Learning Models](https://www.mdpi.com/1424-8220/19/11/2451/htm)
- [Multidimensional Time Series Anomaly Detection: A GRU-based Gaussian Mixture Variational Autoencoder Approach](http://proceedings.mlr.press/v95/guo18a/guo18a.pdf)
- [Deep learning for anomaly detectionin multivariate time series data](https://users.informatik.haw-hamburg.de/~ubicomp/arbeiten/master/assendorp.pdf)
- [NetWalk: A Flexible Deep Embedding Approach for Anomaly Detection in Dynamic Networks](https://www.researchgate.net/publication/329087157_A_Deep_Neural_Network_for_Unsupervised_Anomaly_Detection_and_Diagnosis_in_Multivariate_Time_Series_Data)