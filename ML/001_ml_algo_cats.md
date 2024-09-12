# 1 | ML Algo Cats
    What is Machine Learning?

    In layman’s terms Machine learning is the study of a group of computer algorithms that can learn 
    and adapt to new data without human intervention 
    and improve automatically through experience in an (almost) unbiased way.

-- ---

We can classify the popular Machine Learning approaches into broad categories based on their explicit characteristics.

I. Degree of Human Supervision

    There are  four  major  categories that we need to talk about when we gauge the degree of human intervention 
    in the process of model training:
    
    * Supervised Learning
    * Unsupervised Learning 
    * Semi-Supervised Learning 
    * Reinforcement Learning

    
In supervised learning, the training data you feed to the algorithm includes the target features, called labels

    It can be divided broadly into:
      Classification (Predict a discrete dependent variable)
      Regression (Predict a continuous dependent variable)
      
      
In unsupervised learning the training data is unlabeled.

    It can be divided broadly into:

    Clustering(Division of data into meaningful clusters)
    Visualization and Dimensionality Reduction(simplification of the data without loss of important information)
    Anomaly Detection(Detecting outliers in data)
    Association rule learning(Discovering interesting relations between features in a large pool of data)
    
Semi Supervised Learning

    Algorithms that deal with partially labeled training data, usually a lot of unlabeled data 
    and a little bit of labeled data are classified as semi supervised algorithms

Reinforcement Learning

    Here the learning agent can observe the environment then select and perform actions 
    and get rewards in return.(or penalties as in case of negative rewards). 
    It must then learn by itself the best strategy to get the most reward/least penalty over a period of time.
    This strategy is called policy. 
    It defines the action the agent chooses when it lands in a given situation.

-- ---

II. Degree of Reusability

This pertains to ability of the model to learn on the fly when supplied with a number of new training examples.

Batch Learning

    * These algorithms are incapable of learning incrementally and must be trained using all the available data
    * Traditionally called offline learning.(Offline means that you have a static dataset)
    * If you want a batch learning algorithm to take new data into account you need to train 
      a new version of the algorithm from scratch on the complete dataset
    
Incremental Learning

    * Traditionally done online.(Online means that you have a dynamic data input)
    
    * One main advantage of these algorithms is that they can be used for out-of-core learning 
      (Useful for huge  datasets  that don't fit  into main memory)
      
    * Most important parameter of online learning algorithms 
      called the learning rate which controls how fast they adapt to 
      changing data: 
      
         If you set a high learning rate, then your algorithms
         will  rapidly  adapt  to  new data,  but they will  also  
         tend to  quickly  forget  the  old data.
        
         Conversely, if you set a low learning rate, the algorithms
         will learn more slowly but it will also be less sensitive 
         to noise/anomalies in the new data.
         
    * A  big  challenge  with  online  learning  is  that  if  
      bad  data  is  fed  to  the  system,  the  system’s
      performance  will  gradually  decline.

-- ---

III. Mode of Generalization

Generalization means that given a number of training examples the algorithms should be able to perform well on unseen data.

Instance-based learning

       In this type of learning the algorithm learns the  training examples
       by heart and then generalizes to new cases using a similarity measure.
   

Model-based learning

    In this type of learning we either define a utility function that measures how good your model is 
    or you can define a cost function that  measures  how  bad  it  is and use it to generalize on unseen data.
    
-- ---
