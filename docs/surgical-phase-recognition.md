# Intro

Evolution of the state-of-the-art AI models for phase recognition:
- Support Vector Machines, Hidden Markov Models and Dynamic Time Warping.
- Deep learning techniques + RNN
- ...?

1. OperA: Attention-Regularized Transformers for Surgical Phase Recognition, 2021, TU Munchen

Methodology:
- CNN: ResNet-50 feature extractor.
- Transformer: Transformers have the capabilities to model long sequences in a parallel manner using self-attention by relating every input feature with other input features regardless of
their distance in the sequence.

Pros and Cons:
- Outperforms other temporal refinement methods (LSTM)
- Evaluate OperA on two challenging surgical video datasets (Cholec80, MitiSW)

Data:
- Cholec80
- MitiSW



2. Deep learning for surgical phase recognition using endoscopic videos, 2020

Methodology:
- InceptionV3 network with ResNet50 backbone.

Pros and Cons:
- Cons: No temporal information about the progress of the procedure was provided to the network. It only used visual information contained in the frames of the videos.

Data:
- 33 laparoscopic cholecystectomies (LC)
- 35 total laparoscopic hysterectomies (TLH)