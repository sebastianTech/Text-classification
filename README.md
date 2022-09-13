Exploring Text Data


Computer devices are geniuses in learning from the spread of facts, figures, or information systematically displayed and filled with numerals. 
However, humans communicate with words and not with numerals. Natural Language Processing (NLP) is a notion of empowering computers to communicate in human language. NLP is an interdisciplinary field combining Computer science, Artificial intelligence, and linguistics. Skillful use of Languages is what makes part of a human. Hence, the desire for computers to speak our languages has been a desire, leading to NLP.
Language is symbols, and symbols are not just an invention of logic or classical AI. When a human communicates, it involves symbols, but its communication uses a continuous substrate. Commonly we use
•	Gestures
•	Sound
•	Images (Writing)

The symbol is invariant across different encodings.
However, brain encoding appears to be a continuous pattern of activation, and the symbols are transmitted via continuous signals of sound and vision. 
![image](https://user-images.githubusercontent.com/66043834/133356017-5ff6ed1d-e632-42c1-9bae-573653999ed0.png)

Natural language can be in the form of speech, OCR/Tokenization, etc. In any form, the language represented passes through 4 phases:
•	Morphological analysis
•	Syntactic analysis
•	Semantic analysis
•	Discourse processing
That’s an introduction to NLP. Our focus is on exploring text data. Imagine that you are in a library and the library has a room filled with books on NLP, and you are asked to go into the room since you want to study NLP; where will you start? Or soft copies of about 200 books on NLP were provided, and you are asked to review all. The first question you will ask yourself or your mind is: Where do I start as a beginner?
You will observe that finding insight on text data (unstructured) available on which book to start first will be difficult. Suppose someone comes to advise you on which book to begin. In that case, such a suggestion can be bias because to another person, it may be a different book, and humans are victims of the unconscious bias, especially where there are no tools to get the best insight on where to start. This is one of the challenges faced with NLP. In harnessing the power of text data, a giant stride has been made in this regard. Imagine where you can use unstructured data (text data) to manage the growth of your LinkedIn page, harsh tags of tweets or events on tweeter, many opportunities that such breakthrough has created. Today will be looking at the basics in exploring text data, generating word frequency, word clouds, and look at the need for pre-processing text data all in python programing language.

About the Dataset
To explore text data, we will be using tweet data from the late George Floyd funeral, and it can be found on Kaggle for this demonstration. The link to the dataset is https://www.kaggle.com/jl18pg052/tweets-for-georgefloydfuneral/tasks?taskId=1132

Description of the dataset: 
We want to explore the tweets and see how basic exploring to text data. This article does not cover how to install python, how to run Jupiter notebook or any IDE. I believe you would have known how to do that. In any case, drop a comment if you want a write-up on how to set up your programming environment.  This project is  done on a google Colab; hence you import your data and visualize it, as shown below
![image](https://user-images.githubusercontent.com/66043834/133355839-db77dd2f-6c1a-4b9f-8643-74066b1acaa3.png)

 
The Column text contains the tweets. This article will be in series, and this dataset will be our learning dataset. Don’t worry about the rest column as the future article will explain how to handle it.
Word Frequency
In text mining, the frequency of words is the first call point. However, one can use other concepts, but word frequency comes in handy but is not always the best option. Word frequency is mostly used in sentiment analysis. There are different terminologies associated with word frequency which will see in future series of exploring text data. For now, have in mind that such terms exist.
N-gram: breaking of text into chunks of words, or it could be in letters. U-gram, one word, and Bigram 2 words.
The frequency table for all the words in the text are shown below:
 ![image](https://user-images.githubusercontent.com/66043834/133355851-cf005def-0c0c-4a53-96b9-aaa6ee1f3b32.png)


Text Cleaning:
Looking at the concept of data pre-processing of the steps in the CRISP-DM model, text data contains a lot of noise, especially data from the tweeter. The noise is "RT," "@," Etc. Having such words will affect our output quality and play no role in the insight we want to derive; hence, it's removed. We use the "re" function to remove them, which is the next series to learn. 
Another point to consider is called stop words. They are just constructs of the English language and not attach to any entity. From fig (), we see words like "to," "a," "of," which we use in everyday language. Future series on this topic will address how to customize your own stop words for an effective text cleaning.
![image](https://user-images.githubusercontent.com/66043834/133355871-6610878f-cf0e-4ab4-b352-54db70132304.png)

 ![image](https://user-images.githubusercontent.com/66043834/133355878-02093f2f-2a97-417d-8915-5be4b02b5520.png)

 
Let’s visualize our data with word cloud before text cleaning and after text cleaning.
![image](https://user-images.githubusercontent.com/66043834/133355898-93b27d34-08f9-45a7-8465-26cca7f7464f.png)

           
We have created a word cloud with noise and without noise, and you can see that there is the tendency to lose insight into our text data and what the content of the tweet is, assuming the description of the text was not known. We have "the" and other stopwords.
The insight showed that the tweet talked more about the late George Floyd funeral with #blacklives matters. 
When text cleaning is not done, obviously, the machine learning model in which the dataset will be built will give a wrong output, and also bear in mind that some words can be misrepresented. We will learn other concepts of normalizing text data in future series.
In summary, this article gave a little insight into one of the tasks in NLP and introduced some concepts and terminology which will look into in the future. Follow to get notified and connect with me on LinkedIn, tweeter for a personal tutorial on being NLP certified.

