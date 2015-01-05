MovieClassifier_v1.1
=====================

A programme written in Java to classify a given movie plot ( actually the Storyline of the Movie )in text form into genres like 
Action,Romance, Comedy ...etc

Contents
---------------
1. Introduction
2. How it Works
3. how to Run
4. Conclutions
5. Future Works


1. Introduction
---------------

"Agent Classy" is a movie Classifying programme written using Java based on KNN (K - Nearest Neighbour ) algorithm

2. How it Works
----------------
initially we get a plot.list from ,contains thousands of movie plots in one text file and genres.list ,contains each movie name and its genres from IMDB Website.from these two files we extracted each movie plot into separate text files contains in a folder named as its Genre  which it belongs more than other genres.then we created separate text files for each movie Genre (as action.txt,comedy.txt....) which include all movie plots in each genre folder.  
from those text files we have created the file "dtmfor5Gen.csv" by using a R Script ( using R data mininng  Language ).it contains a Document Term Matrix ( DTM ) which contains WordCount in columns and Genres in Rows. in here we basically use 5 genres ; Action, Comedy , Romance, Sport, Music.
then Agent Classy calculate a distance called "Euclidean distance" for the new movie plot entered by user to each movie genre.by selecting genres ,have least distances we select the genres the movie should goes to.for that purpose we calculate distances as a percentage of total 5 distances and selects genres which have less than 20% .

3. how to Run
-------------

you can clone this project into your IDE easily.and then you shoul do some changes to mainFrame.java file.change String variable "Path" into your current directory where the location of the project.based on the IDE it may be different.in netbeans it is the directory of SRC folder and in IntelliJ Idea it is the directory of project folder.thats All. 
you can upload a text file by clicking Upload Plot button or you can directly copy and paste the plot into text area.
finally Run the programme and enjoy.

4. Conclutions
--------------

in Agent Classy it gives several genres because a movie cannot classify into only one genre as it contains many ideas.also in IMDB they show a mixture of genres.

5. Future Works
----------------

hope to deplop this into more than 5 genres.(in this version it was limited to 5 Genres because of technical issues like cpu speed and memmory..) 


