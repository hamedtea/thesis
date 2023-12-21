# thesis
This is the repository of my codes that I build for my thesis project. this readme will be improved in the future. </br>
Title: AN ENSEMBLE ML MODEL DESGIN TO CLASSIFY LOS/NLOS PROPAGATION CHANNEL
subtitle: Signal design for 5G NR InF. propagation channel scenario
Abstruct: LOS/NLOS channel classification has numerous applications in wireless communication engineering. It
can enhance the positioning accuracy since it is required to employ a LOS radio channel for highly accurate
location estimation. There are several statistical and data-driven method for this purpose but it seems that the
application of heterogeneous parallel ensemble learning (EL) is not thoroughly investigated for 5G NR signals
and Indoor factory (InF.) channel propagation scenarios. This research gap is addressed in this thesis by
simulating the essential transmission and reception signal and implementing a stacking ensemble learning to
predict LOS/NLOS received signals.
To reach the above achievement, Firstly, the positioning reference signal is generated based on 5G NR TS to
be used as the transmitted signal. Secondly, channel effects are simulated by using a deterministic raytracing
dataset, provided for 5G DH-Inf. channel scenario and received signal is generated accordingly. Thirdly, a
collection of level-one pipelines are selected, including preprocessing and classification functions. By execution
of exhaustive search, 9 top pipelines are ranked according to multiple performance metrics and their hyper
parameters are tuned afterward.The best level-two classifier is chosen by search for the best classifier among
level-one classifiers. Finally, the best structure is used for investigating the effects of physical parameters such
as SNR on LOS/NLOS prediction accuracy.
The results indicate that two-level heterogeneous parallel EL outperforms the single level classification
even when sequential or homogeneous EL (boosting) classifiers are used, both in term of model performance
metrics and prediction accuracy since the worst True LOS and NLOS label prediction is more than 90% AND
80% respectively. In addition, EL provide a straightforward solution to classify imbalanced binary samples as it
uses an internal cross validation algorithm to fit the model. Thus, it can be considered as a novel ML-assisted
method for positioning accuracy enhancement.
Keywords: positioning reference signal, LOS/NLOS classification, heterogeneous parallel ensemble learning,
InF. propagation channel, 5G NR
The originality of this thesis has been checked using the Turnitin OriginalityCheck service.

Notes: 
- The essential input data for this repository can be find in channel_data.npy
- Other data structures can be generate inside .ipynb files (but some minor modificatio is required, I am sure that you are pythonic enough to do that ;-)
- PRS_maker.ipynb includes two function objecs for generating PNS and PRS. There are relevant codes mainly for visualization and output purposes
- RX_maker.ipynb includes three class objects to generate receive signals, correlation and interpolation values and statistical feature generation (more info. can be find inside the notebook)
- CIR_based_ML_model.ipynb includes neccessary operations for ML LOS/NLOS classification.  
CIR_based_ML_model conveys some NN/DL code for future development
- To access to the whole raytracing dataset for InF. channel env., contact aamir.mahmood@miun.se
- To access to more info. about almost everythin, visit www.trepo.tuni.fi (If you cannot see my thesis text in this platform, be patient :-) ; Popular access will be provided soon) 


