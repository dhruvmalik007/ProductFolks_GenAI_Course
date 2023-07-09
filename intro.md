## GenAI introduction course and overview by SRK. 
- In general description of the history of TPF. 
- Major sponsors from the space : LlamaIndex, MS founders hub, H20.ai, postman etc.
- Description of the genAI challenge and the prizes.
- 2 weeks ;( (given that olast week will be in the ethcc, but you can try to join and atleast audit the course).
- Week 1 :
    -  Higher level overview of the various machine learning / DL techniques 
    -  Dissecting the various real life use cases implementation (from the aspects o the system design and how the UX workflows are to be planned and developped for the frontend).
    - Multimodal (image and video generation) fundamentals usinng GAN / transformer , various benchmark techniques and applications

- Week 2: 
    - Generative AI for communication workflows: optimizing the operations across CRM /ERP and other industrial tools ecosystem

Various modules / components of the cohort:
    - workshops
    - framework based workshops for the prominent generative AI services.
    - courses covering 


## SRK course describing the introduction of the generative AI ecosystem: 


- evolution of the generative models with their architecture (LLM) and in the various domains. 

in general , following black box: 


```mermaid
 
graph LLM:
    input-text --> LLM;  as prompt
    LLM --> Output; generated result
    LLM --> Numerical embeddings;  
```


and the model can understand based on : 

- Prompting by instruction. 
- Prompting by example.



diffusion models: 

1. removes the noise from the pixelated image.
2. takes the text prompt and then converts to the 


## history: 

understanding the NLP models evolution in three phases :
    - initial phase: using bag of words techniques that compares the relative presence of the word in the given text in order to predict the sentiment and generate the predicted phrase in the sentence etc.
        - Was not scalable for the articles of various domains, you need to correlate every word to the dictionary/given corpus.

    - Then using the vector dimension to plot the word into the higher dimension vector space (each dimension being generated based on the frequence of word or correlation) and their comparison with the other word helped the model to do generative/ predicting tasks.
        - but still faced issues that it didnt store more contextual information regarding the context off the particular word , specialy if the word is not defined to the model before (eg using apple interchangably as the fruit or the MNC).

    
## LLM training process:

1. Pre-training: 
    - predicting the next word/ sequence of tokens in the given input prompt
        - based on the temprature parameter (that defines whether your )


2. Supervise finetuning :
    - then selecting which of the outputs that are generated in the course of the pre-training are correct based on the nature of the question asked.




3. Reward modelling:
    - once the reviewers generate the responses for the given user, the model will rank the responses from the prompt feedback.





## various challenges : 

- Inconsistency for the same qeury and input:


- Managing the challenges of the hallucination.


- Challgences of the privacy information: either using the homomorphic encryption / ZK or other techniques to convey the nature of the input in a way that the host of this model can inferr the PII details of the user.

- Challengrs of the performance and cost optimisation.


- Generation of the result of type reasoning and arithmetic computation.




## Doing application system design for LLM / genML applications:
There are following levels of LLM application components based on the lifecycle of the input prompt processing to the result. 


### 1. Prompt engineering: 
    - this defines the science of defining the queries for the better task completion by the laguage model. there are various techniques , some of them are explained [here](https://www.promptingguide.ai).





### 2. vector databases: 

Its the caching layer of LLM, where we store the embeddings of the various dataset in order to fetch the relevant context in case the user queries wanted to ask about the detail that is not in the current context by the model.



### 3.  LLM training model frameworks : 

These are the frameworks that allow users to train model from scratch or pretrain the existing benchmark models for the given dataset.




## Then finally the application demo by SRK (from the langchain): 

