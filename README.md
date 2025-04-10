# EMOTION-BASED-MUSIC-RECOMMENDATION-SYSTEM-USING-GRAPH
# Emotion-based-Music-recommendation-system

The flow Diagram of the system:
![flow diagram](assests/flowchart.png)



The system mainly consists of 2 parts:
a)Real time facial emotion detection & prediction using CNN
b) Recommendation of songs from the knowledge graphs

a) Real time facial emotion detection & prediction using CNN
-The model used was a CNN Sequential model for predicting emotion of user's real time facial expression input.
-The model was trained on 28,000 training images with 7 annotated emotions: sad, happy, fear, neutral, surprise, disgusted & anger.
-Later, the model was validated on a dataset of over 7,000+ greyscale annotated images.
-The Training accuracy was 72.32% and the validation accuracy was 61.34%.
-The plotss for accuracy and loss are:
![accuracy   loss graphs](assests/graphs.png)


b)Knowledge Grapg Representation & Song Recommendation
-The knowledge graph is created on the csv file containing over 1 million spotify tracks.
-The threshold value for adding the edge between the nodes can be changed accordingly and also the similarity metrics(cosine similarity can also be used)
-As of now, for easier visualization and easier understanding, we have created a seperate csv file of 100 songs, named as "small.csv". The knowledge graph is created on this smaller dataset.
-The predicted emotion from the CNN model is fed as input to the graph for recommending the songs.


The outputs of the system are:
![detect emotion 2](assests/output.png)
![list of recommended songs](assests/image.png)

![image](assests/knowledege.png)
