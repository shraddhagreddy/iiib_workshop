### GENAI
workshop by K Aditya in IIITb

## Discriminative AI

## Introduction to AI
- what is programming?
    - simplify any given task
    - electrical->electronics(0/1s)->assembler
    - converting ur instructions into 0s and 1s 
    - how are u trying to solve ur problem? (logic and implementation)
        eg: even and odd 
        what is even?
        - if a value is divisible by 2
        - implementation- conditional statement
        - sequentially, conditionally and iteratively (effectively any given problem statement is broken down based on these three)-> traditional way of programming
        - another way: statistically 
        - face detection - cannot curate for all faces, take a subset and train it on that
        - there is a diff between the two where u take a problem statement and then try to solv eit (syntax and semantics) and the other one is the subset.
        - fundamentally AI is data driven- where data is consolidated and a pattern is established
        - want to undestand the mathematical behaviour between i/p and o/p

## ML in layman's terms
- field of study that gives computers the ability to learn without being explicitly programmed.
- # tb def:
    - a hypothetical function computed on the basis of currently available inputs and outputs to predict a probable output to futuristic outputs
    - what % is correct?
    - so predicting+probablity 
    - output is not certain- predicted and probable 
    - you have a training part and deployment part
    - training set->modal->deployment
    - training is automated but steps to train needs to be coded

## Traditional programming vs Machine Learning
- data --->|        |-> output
  program->|computer|

- data --->|        |-> program
  output-->|computer|
- ML data driven
- tarditionally- should breakdown logically


## Demystifying DS,AI, ML, DL
- GenAI is part of DL
- AI 
    - any piece of algorithm that can imitate human intelligence
    - requires data
    - eg: overhead water level detection program, face recognition

- ML
    - a statistical learning which enables a machine to improve its experience
    - data driven learning
    - eg: KNN, Kernel SVM
    -i5/i7 processor is also fine

- DL
    - involves using neural networks for solving problems
    - inspiration: human brain (neurons- uses stimulus) - perception
    - eg: speech recognition, image recognition
    - RNN
    - GPU

- DS
    - deals with munging, cleaning, visualsation and finding useful data samples
    - draw meaningful conclusions from data
    - look at the existing data, visualise and then make a decision

- if problem statement is to visualise - DS
- if problem statement is to be more certain- DL


## Classification of ML

- Five core ML Steps:

    data acquisition (ds)-> data preprocessing(ds)-> choose algorithm (ml)<-> testing/validating (ml) -> deployment
    - choosing the algorithm depends on the deployment
    - also depends on who you are serving

- # Types of ML
    - 1) Supervised Learning
        - predictive model
        - labeled data
        - types: regression, classification
        - eg: image recognition
    - 2) Unsupervised Learning
        - descriptive model
        - unlabeled learning 
        - types: clustering, association
        - eg: netflix/youtube recommendation system
    - 3) Reinforcement Learning
        - continuous training algorithm which are trained on previous outcomes
        - time series data trained model
        - learns only until model is deployed
        - eg: weather reporting, stock price prediction

    - Supervised Learning
        - Classification and Regression
        - Classification 
            - an algo trained to classify things into diff classes based on input
            - catgorical in nature
            - eg: shape detection, face detection, speech detection, cancer detection, spam/not spam
        - Regression
            - an algo trained to predict a continuous value
            - analogous in nature
            - eg: boston house prediction, height to weight calculation, real estate price, sales of an item from inventory

# chatgpt and deepseek undergo supervised and unsupervised learning. Starts with unsupervised and then supervised followed by reinforcement learning
# reinforcement learning is a kind of reward system
    
    - Unsupervised Learning
        - we are given a data set and which has got no labels/ results
        - we can derive the structure by clustering the data based on relationships among the variables in the data
        - with unsupervised learning there is no feedback based on the prediction results
        - eg: computer clustering , market segmentation, social media (friend suggestions)

https://tinyurl.com/2s3d57be
https://drive.google.com/drive/folders/1zUzhOcj_Ybomba8QQLxK2xriSm5C2xFq


# kmeans.html
- here when we upload the image
- it will be split according to the R,G,B 
- feature vector
- midpoint of a line x1+x2/x2+y2 :- linear geomtery
- elbow plot
- image- rgb 

# Neural network
- brings non linearity to data 
- neuron/ network node: 
- blue: input layer
- orange: hidden layer
- green: output layer
- H1= sigmoid (i0 * w 0_oo + i1 * w0_01 + H1.0 (bias))
- weight - proportionate thing driving ur output
- weights discovery is starting which is the learning
- if the ouput is not good as the estimated output it starts fine tuning the weights
- y pred = fun(i) - sigmoid, log, customised - there are diff kinds of functions that brings about the non linearity
- y actual - yact - ypred =error
- after getting error u try to adjust ur weights
- w new = w old - Ir*error
- # watch andrew ng machine learning algo
- # micrograd - back propagation algorithm lecture by andrew ng
- # dr raj - ??
- # mira muratis discriminative model
- learning rate:- 
    - high: footsteps is high
    - low: 
- based on architecture the neural network changes 
- loss and accuracy


# there is no searching or db in generative models - uses weights
# they are auto regressive models

# Tensorflow playground
- explore more and learn

https://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=4,2&seed=0.67753&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false


# vocabulary 
- Types of datasets:
    - train dataset - corpus of text used to adjust weights
    - test dataset - used to discover the right hyper parameters
    - validation dataset