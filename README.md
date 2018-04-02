# python-machine-learning-Classification
For the beginners who would like to learn ML/DL.
For more details : https://medium.com/@tim24514/python-machine-learning-classification-66dcdbd41d04

In this example,we can learn how to use sklearn to classify the dataset. 

We can use datasets from lots of website ,and the data can be loaded into the models. Using SVM and KNN,these methods are suitable for classification problems. By comparing the accuracy ,we can choose the better way to processing your data. 

**1.Car Evaluation Dataset** 

+ Dataset: http://archive.ics.uci.edu/ml/datasets/Car+Evaluation
+ Abstract: Derived from simple hierarchical decision model, this database may be useful for testing constructive induction and structure    discovery methods.


**2.Creativity Dataset** 

+ Dataset: http://archive.ics.uci.edu/ml/datasets/Car+Evaluation
+ Set the persional point
    In this part , we will set a new score for the new feature .
    Focus on family , so the car must have enough seats . 
    The 'persons' part is most important , so I set the weights '70%' in the persional_point.
    And the second one is 'doors' part. For some family trip , it will be Convenient to have 
    enough doors. I gave it the weights '30%'.
    
   * point1(doors)
     * 2 doors -> 1 
     * 3 doors -> 2 
     * 4 doors -> 3 
     * 5more doors -> 4
     <br />
   * point2(persons)
     * 2 people -> 1 
     * 4 people -> 2 
     * more people -> 3 
     <br />
     
   * point_final=0.3*point1+0.7*point2
