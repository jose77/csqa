## Model Name: 

RoBERTa + KE (single model)

## Affiliation:
Anonymous

## Model Description:
We first finetuned RoBERTa masked lm on the Open Mind Common Sense (OMCS) corpus. 
Then we retrived 10 best sentences from wiki docs for each question and option as evidnece. 
The input sequence for RoBERTa is: \<s\> question <\s> option <\s> evidence <\s>.
we finetune the further pretrained RoBERTa model on CommonsenseQA dataset. 
The accuracy is 78.7\% and 73.3\% on dev and test set respectively. 

## Experiment Details:
### Finetuned on OMCS
+ max updates: 100k
+ learning rate: 1e-5
+ batch size: 128
+ max sequence length: 512


### Finetuned on CSQA
+ max updates: 1000
+ learning rate: 1e-5
+ batch size: 64
+ max sequence length: 256
