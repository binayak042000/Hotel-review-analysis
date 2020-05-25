# Hotel-review-analysis

This is a project where I have used NLP and Machine Learning techniques to classify hotel reviews into various categories and through that find the reason for sub par performance of some hotels of popular brands .

First I categorized reviews with the help of Latent Dirichlet Allocation (LDA). It works as an unsupervised algorithm which classifies text documents . Instead of classifying all the reviews at once , I distributed them as per the rating given by the user and then for eah rating I classified the reviews into various types . 
The various categories I could generate are :

1 star hotel reviews :
Focus on room and service ,focus on overall stay and manager , focus on the room , hotel and booking 

2 star hotel reviews :
Focus on overall stay and staff , focus on room specially the cleanliness 

3 star hotel reviews :
focus on room , bathroom ; focus staff and breakfast ; focus room , staff and parking  ; focus on room and overall stay at night ; focus on hotel location ; heavy focus on room specially cleanliness and floor .

4 star hotel reviews :
Focus on location ; focus on room ,staff , breakfast ; focus on overall stay ; focus on pool area and parking ; focus on hotel services

5 star hotel reviews :
Focus on hotel , room, location and staff ; focus on cleanliness and staff ; focus on room , breakfast ; focus on overall stay especially location and staff ; focus on comfort of the hotel beside room , breakfast , staff 

Of course the topics do not seem to be clearly distinct but the weightage given to particular entity in various topics varies . 
Next I created a dataframe where I stored the name , average rating , mode of ratings , hotel parent brand and hotel category(premium or luxury or budget) .
The parent brand was found through research outside the dataset with the help of wikipedia . 
This dataframe helped find out under-performing hotels ( hotels in premium/luxury category but having low average and mode of rating) . The reason of under performance can be the categories of most of the reviews generated with the help of LDA . 
