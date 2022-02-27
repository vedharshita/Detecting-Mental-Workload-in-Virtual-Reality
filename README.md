# Detecting-Mental-Workload-in-Virtual-Reality-Using-EEG-Spectral-Data: A Deep Learning Approach

**Problem** - 
Virtual reality (VR) is revolutionizing the way we live. One factor that needs careful consideration during VR interactions is the degree of mental or cognitive load users experience while completing their tasks in these immersive environments. Mental workload (MWL), which refers to the amount of mental effort a task requires users to exert, has long been recognized as an important factor in human-computer interaction (HCI) contexts and has been shown to affect users’ well-being and performance. The current study investigated the possibility of detecting MWL levels in VR on the basis of EEG brainwaves using deep learning models. Focused on EEG data because of the strong association between MWL and corresponding brain activity and because of the need to capture changes in brain activity in real-time with high temporal resolution in a non-invasive manner.

**Approach** - 
For this purpose, we used an existing dataset that contains EEG recordings of 15 participants as they completed a variation of the n-back task in VR under different MWL conditions. The overall aim was to build upon the prior work and to classify EEG signals into MWL levels with various traditional machine learning algorithms and deep learning techniques. The contributions of the current study are as follows:
The application of a novel approach to preprocessing and representing EEG signal data as spectrograms for deep learning models
The comparison of multiple traditional machine learning algorithms and modern deep learning techniques with respect to their performance
The availability of the code used to preprocess the data and train and evaluate the machine learning and deep learning models for future exploration and inspiration.

**Research paper**:
Published in IEEE International Conference on Artificial Intelligence and Virtual Reality (AIVR’21) https://lnkd.in/d3WQym5Y

**Code**:
https://github.com/vedharshita/Detecting-Mental-Workload-in-Virtual-Reality

**Key Points**: 
Used Brainwaves as features - 
  Welch’s approach with a 256-point Fast Fourier Transform (FFT) was used to construct the frequency spectrum of the EEG for each 4-second run. This method entailed breaking down the EEG signal into component frequency bands, each with its own set of functional features. Delta (0–4 Hz), theta (4–8 Hz), alpha (8–14 Hz), beta (14–30 Hz), and gamma (30–60 Hz).
Feature Normalization
  Using MinMax Scaling individually for each participant’s recordings in contrast to standardization to end up with smaller standard deviations, which can dampen the effect of outliers.
EEG Signals as Spectrograms
  Produced spectrograms to represent the EEG brainwaves as features in the CNN model.
Best performance - 
  In machine learning classifiers - obtained from SVM, with 33% accuracy, which can be attributed to good generalization properties of the margin maximization. It is roughly equivalent to random classification.
  As for DL architectures, CNN model using spectrograms yielded slightly better results compared to the baseline models, with an accuracy of 35%, which is still not a drastic improvement. This might be happening because the model could be adjusting to the noise in EEG data, and/or requires additional features like hand, head or eye movements recordings.

