###KE4WoTChallengeWWW2018
The information about this project is described here.

In this folder, there are four comma separated files (.csv) containing tweets related to respiratory diseases and one text file containing 25 questions. We provide a brief description of the files under "Data" folder :

1. Keywords_filtered_tweets_with_keyphrases_with_tid.csv : This file contains 15893 tweets which have been filtered using a lexicon of domain specific keywords. There are 3 columns in this file:
Column A: tid - This column contains Tweet Ids. This the ID returned from Twitter Streaming API. The participants are required to report Tweet Ids along with their responses to the questions.
Column B: text- This column contains the tweet texts. The data in this column will be useful for the participants in building their NER systems.
Column C: keyphrases- This column provides  keyphrases of relative importance in the text. We have utilized a keyphrase extraction module developed at Kno.e.sis for generating this column. 

2. Keywords_filtered_tweets_without_keyphrases_with_tid.csv : This file contain 15893 tweets and tweet IDs excluding the keyphrases. The file has been generated for those participants who want to develop their NER approach without using the keyphrases. 

3. tweets_with_keyphrases_with_tid.csv : This file contains 3 columns:
Column A: Tweet Id (tid)
Column B: Tweet Text (text)
Column C: KeyPhrases(keyphrases) 
The tweet count in this file is 32153. The tweets in this file are not filtered using the domain specific keywords. Extraneous tweets (tweets that present in this file and are missing in files listed in point 1 and 2) will help in validating the NER approach developed by the participants.  

4. tweets_without_keyphrases_with_tid.csv : This file contains tweets and tweet IDs without keyphrases. Tweet count in this file is 32153. The tweet set in this file is same as 'tweets_with_keyphrases_with_tid.csv'. This file contains the raw tweet set that was sent as input to our Kno.e.sis keyphrase extraction module for generating the keyphrases (given in files : 'Keywords_filtered_tweets_with_keyphrases_with_tid.csv' and 'tweets_with_keyphrases_with_tid.csv’).

5. Questions.txt: This file contains few domain specific natural language questions that have been created for this task. This file is one of the inputs to the Question Answering(Q/A) task in WWW-2018 KE4WoT Challenge. There are 26 questions over which the participants have to develop their Q/A model. The participant is allowed to create their own questions having a similar syntactic structure to test and validate their models.  

Note: The participants are allowed to use supportive knowledge sources such as: SNOMED, UMLS, ICD-9/10, LOV4IoT, etc.