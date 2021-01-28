# NLP_MathProblem  
Since it is an Industry-University Cooperation Project,  
no longer access to the dataset as the project ended :)  
 
Note the project was worked as a team,  
and I was mainly in charge of Text pre-processing / machine learning methods (XGBoost) / Ensembling / Result Analysis

#### Implementations:  
1. Processing dirty text  
2. Machine Learning methods to classify math word problems with equations (Korean + English + Math Symbols + Numbers)  
3. with the help of pretrained KoBert and KoELECTRA models, classification used with fine tuning
4. Ensembling  
5. Analysis of results: wrongs and rights   
 
 
#### Results:  
1. Comparison of different text preprocessing before applied in CountVectorizer and then XGBoost  
- From ex1 ~ ex4 the level of removing text and substitution increases  

![NLProject_graphTextPreprocessingCompare](https://github.com/laphisboy/NLP_MathProblem/blob/main/NLProject_graphTextPreprocessingCompare.PNG)


2. Comparison of different Models with fixed text preprocessing  
- Ensemble method is aggregation of outputs from different selected models with weights
- After comparing...  
 1. using all model outputs and using a small neural network to learn the best way to combine the outputs  
 2. using only the best performing models for each type of method, best weight is found through trial and error  
![NLProject_graphModelCompare](https://github.com/laphisboy/NLP_MathProblem/blob/main/NLProject_graphModelCompare.PNG)
