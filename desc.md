## Model Name: 

RoBERTa + KE (single model)

## Affiliation:
Alibaba DAMO NLP

## Model Description:
We first finetuned RoBERTa masked lm on the Open Mind Common Sense (OMCS) corpus. 
Then we finetuned the further pretrained RoBERTa model on CommonsenseQA dataset. 
we retrived 10 best sentences from wiki docs for each question and option as evidnece. 
The input sequence for RoBERTa is: \<s\> question <\s> option <\s> evidence <\s>.
The accuracy is 78.7\% and 73.3\% on dev and test set respectively. 

## Experiment Details:
### Finetuned on OMCS
+ max updates: 100k
+ learning rate: 1e-4
+ batch size: 256
+ max sequence length: 512


### Finetuned on CSQA
+ max updates: 1000
+ learning rate: 1e-5
+ batch size: 64
+ max sequence length: 256
