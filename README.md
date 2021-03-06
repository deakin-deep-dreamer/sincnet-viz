# sincnet-viz

This source refers to our original paper "Interpretability and Optimisation of Convolutional Neural Networks Based on Sinc-Convolution" (https://ieeexplore.ieee.org/abstract/document/9806184). 

Sinc-convolution was used as a constrained first-layer of a CNN model and Explanation Vector (EV) based joint time-frequency representation was visualised in order to provide domain-specific interpretation. The learned information was used to optimise the sinc-CNN model by reducing the number of sinc-convolution kernels.

The code is unorganised and contains different experimental modules. Readers are encouraged to understand the idea used in the paper instead of trying the code as it is. The sinc-convolution model was inspired by the original sinc-net paper "Speaker recognition from raw waveform with sincnet" [Ravanelli et al]. The files are organised as follows 
* The sincnet.py shows the sinc-CNN model, among others, SincConv1d_fast model was used for model training and validation for the 2 ECG tasks - R-peak localisation, and beat classification. 
* The training for ECG R-peak localisation, and beat classification tasks were shown in train_sincnet.py, and train_beat_classify.py respectively. 
* debug_filter.py shows the generation of explanation-vector by modifying the sinc-CNN model in such a way that it can mask each input sample at a time and measure the delta of the output. 

For rurther communication, send email to the corresponding author or mahabib.deakin@gmail.com
