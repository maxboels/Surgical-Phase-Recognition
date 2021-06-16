Why not using LSTM for surgical phase recognition or why should we use them?

1.	Intro

In recent years, surgical phase recognition has gained more interest from researchers and the industry with new state-of-the-art results. CNNs have now since almost a decade outperformed most of previous computer techniques. While Long Short-Term Memory (LSTM) models, a special type of RNN, have brought new state-of-the-art results in video recognition. Recently, new types of architectures have arisen from research, called Transformers which are using Attention mechanism to look at particular tokens in sequential data. This approach is therefore very effective on video data. Here we are discussing the evolution of those different techniques to see which one should be good candidates for surgical phase recognition in the field of surgical data science.

2.	Long Short-Term Memory (1997)

LSTMs are a special type of Recurrent NN with gated parameters to choose what to remember. They mitigate the exploding and vanishing gradient problem of RNN. With three gates:
-	Input gate: update the cell state.
-	Forget gate: how much should we forget or keep.
-	Output gate: what the next hidden state should be.
Those gates allow to select what to remember in previous layers. All have sigmoid or tanh activations. 
Pros:
-	Capture long term dependencies through time while avoid vanishing gradient problem.
-	Good for sequential patterns.
-	Good for information embedded in time.





3.	Nicolas Padoy’s LSTM for Surgical Phase Recognition
⮚	
3.1.	Less is More: Surgical Phase Recognition with Less Annotations through Self-Supervised (2018)

Pros:
-	Semi-supervised approach
o	Self-supervised pre-training
-	Scalable for different surgeries.
-	Pre-trained CNN and LSTM (EndoN2N).
3.2.	Weakly Supervised Convolutional LSTM Approach (2019)

Pros:
-	Weakly supervised on binary presence of tools.
-	CNN + Convolutional LSTM.
-	ConvLSTM outperforms the CNN baseline tracker for spatio-temporal coherence of sequential image frames (surgical video).

4.	Conclusion

Based on the selected papers, it seems that during those last few years the research community has shifted its attention towards Transformers in spite of the good performance of CNNs for computer vision tasks. Indeed, Transformers have shown good results for NLP and are now also very suitable for visual tasks. While, LSTMs are still showing competitive performance, they haven’t really evolved as much as other new architectures.
Another trend is going towards self-supervision learning. Some models have shown comparable performances (DINO) to supervised learning approaches. Giving the time and cost of labelling large data set, searching for new self-supervised ways seems more relevant.

5.	Some References

1.	LONG SHORT TERM MEMORY, SEPP HOCHREITER, 1997
2.	ADDRESSING SOME LIMITATIONS OF TRANSFORMERS WITH FEEDBACK MEMORY (2020)
3.	SWITCH TRANSFORMERS: SCALING TO TRILLION PARAMETER MODELS WITH SIMPLE AND EFFICIENT SPARSITY (2021)
4.	LONGFORMER: THE LONG-DOCUMENT TRANSFORMER (2020)
SCALES LINEARLY WITH THE SEQUENCES LENGTH VS. QUADRATICALLY.
5.	RETHINKING ATTENTION WITH PERFORMERS (2020)
NEARLY UNBIASED ESTIMATION OF THE ATTENTION MATRIX.
6.	NYSTRÖMFORMER: A NYSTRÖM-BASED ALGORITHM FOR APPROXIMATING SELF-ATTENTION (2021)
7.	ROBERTA: A ROBUSTLY OPTIMIZED BERT PRETRAINING APPROACH (2019)
8.	PERCEIVER: GENERAL PERCEPTION WITH ITERATIVE ATTENTION (2021)
9.	BIG TRANSFER (BIT): GENERAL VISUAL REPRESENTATION LEARNING (2019)
GOOD FOR TRANSFER LEARNING PROBLEM, CNN.
10.	MLP-MIXER: AN ALL-MLP ARCHITECTURE FOR VISION (2021)
11.	INVOLUTION: INVERTING THE INHERENCE OF CONVOLUTION FOR VISUAL RECOGNITION (2021)


