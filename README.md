TwitterWordCloud
================
Welcome to twitterWordCloud

Description:TwitterWordCloud is an application that takes the recent tweets from the twitter server and then extracts the Important
words and value of information form the tweets and depending upon the number of occurance in the tweet data the word gets apt weight.

In the end the word is displayed on graphical interface of processing IDE. The word that has heigher weight is displayed in big fonts.

Version 1.0

Author Nilesh Singh, Nikhil Jukar, Charu Mittal.

Contributors

*Ritter, Alan and Clark, Sam and Mausam and Etzioni, Oren (University of Washington), https://github.com/aritter/twitter_nlp



Tools:

Twitter NLP.
Processing IDE
Python
Java
OS: Linux(Ubuntu), Winddows 7 


Instruction:

This project has two different way to access twitter recent tweets.

1:Twitter search API 1.0 (deprecated) Does not requires Authentication, anonymously gets the data from server. 2:Twitter REST api 1.1 (GET Search/tweets) Does require oAuth authentication.

JSON.org: I am using JSON.org`s JSON parser to parse the received data(JSON) into JSONArray and then process the data.

Note: Modified the JSON parser file( JSONObject.java) method getString. Problem: In the Twitter application sometimes the User-url value is null then the default implementation was throwing an exceptiong.Modified the method int he library to suit the application requirement.

Twitter Search API 1.0

How to use:

Steps:

1:Compile and run searchTwitter.java 2:enter the Hashtage value when prompted on the Screen 3:Done, The application will print the output result on the console and option to Quit or try another Search

Output: The source and Image URLs from the tweet data (Unigue values)

Prints all the Source URLs Prints all the user profile image URLs Prints all the user profile image HTTPs URLs

prints the total number of tweets processed, total number of source and image URLs printed.

Twitter REST API 1.1

How to use:

Steps:

1: compile and run twitterTweet.java

Output: 

This java program will require you to provide a hastag to twitter server to collect the recent tweets. 
The tweets are returned in the form of JSON object that is parsed into text and saved as .txt file.


The output of this program is passed to Twitter NLP running in Linux enviroment.

The output of the twitter NLP then passed to twitterWord.java to extract the relevent information.

The output of the twitterWord.Java is then passed as the input file to processing to display it on the GUI.
