# Basic-Needs-Basic-Rights-BNBR-Kenya---Tech4MentalHealth
5th place solution of Zindi.africa challenge https://zindi.africa/competitions/basic-needs-basic-rights-kenya-tech4mentalhealth
## Model
Single fine-tuned RoBERTa-base using Huggingface Transformers library with PyTorch.

NB: Not doing text preprocessing/cleaning performed better than doing so. All I had to do was remove duplicated texts.

### Hyperparameters

3 epochs.  
Learning rate of 5e-5.  
Batch Size of 8.  
0.1 weight decay.  
0.6 Multi-Sample Dropout.  
Learning rate scheduling (Linear).  
Max text length of 35.  

### Training.  
5 cv folds run 5 times with different seeds used in sampling data making a total of 25 runs. This was done in order to reduce variability in predictions as the data was very small. Test data predictions were done between folds, and later averaged in total.


NB: Not doing text preprocessing/cleaning performed better than doing so. All I had to do was remove duplicated texts.
