## Model Name: 

RoBERTa + KE (single model)

## Affiliation:
Anonymous

## Model Description:
We first retrived 10 best sentences from wiki docs for each question and option as the context. 
Then we finetune the pretrained RoBERTa model on CommonsenseQA dataset. 
The input sequence for RoBERTa is: \<s\> question <\s> option <\s> context <\s>.
The accuracy is 77.5\% and I 68.4\% on dev and test set respectively. 

## Experiment Details:
+ max updates: 1000
+ learning rate: 1e-5
+ batch size: 64
+ max sequence length: 256
