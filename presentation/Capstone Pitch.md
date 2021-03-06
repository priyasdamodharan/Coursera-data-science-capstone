Data Science Capstone: Predicting the Next Word
========================================================
author: Priyadharshini D
date:  9th October, 2020
autosize: true
transition: rotate
transition-speed: slow
incremental: true
font-import: http://fonts.googleapis.com/css?family=Helvetica
font-family: 'Helvetica'

<div>
<img src="coursera.png" style="width:15%"
</div>

Overview
========================================================

<small>People may now stay connected on the go thanks to recent advancements in mobile technology. However, without any language prediction, communicating by text quickly and accurately using a smartphone keypad is quite difficult.</small> 

<small>Against this backdrop, the purpose of the Data Science Capstone project was to develop a data product that uses natural language processing to predict the next word a user may want to type. A shiny application serves as the final product for this project.</small>

<small>The application is available at the following link:
<a href="http://45.55.48.122/" target="_blank">Shiny App</a>.</small>

Model and algorithm
========================================================

<small>An N-Gram Language Model was used to create the prediction algorithm. This approach is based on the Markov Assumption, which states that each word in a string of text is only dependent on the previous N words. A set of four N-gram models has been built for this project:</small><small>

* Unigram: previous words do not matter
* Bigram: only the previous word matters
* Trigram: only the previous two words matter
* Quadgram: only the previous three words matter.</small>

<small>
Given this dictionary of N-grams, the probability for possible next words is calculated through Maximum-Likelihood Estimation combined with Good Turing Smoothing. Depending on the length of text input, the prediction algorithm selects candidates from appropriately ranked N-grams. This mechanism is known as the "The Stupid Backoff algorithm", a highly efficient and inexpensive algorithm proposed by Thorsten Brants et al (2007). </small>   

<small>Next Word Predict is a Shiny app that uses a text prediction algorithm to predict the next word(s) based on text entered by a user.

The application will suggest the next word in a sentence using an n-gram algorithm. An n-gram is a contiguous sequence of n words from a given sequence of text.

The text used to build the predictive text model came from a large corpus of blogs, news and twitter data. N-grams were extracted from the corpus and then used to build the predictive text model.

Various methods were explored to improve speed and accuracy using natural language processing and text mining techniques.</small>

The Application
========================================================
left: 55%
incremental: true
<div>
<img src="CapstoneApp.png" style="width:105%"
</div>
<small>
The user is presented with a text input box which when filled out with a word or short phrase returns:
* A top prediction 
* A dynamic table suggesting possible next words 
* A word cloud visualizing the predictions.</small> 

***
<small>
The Shiny app dashboard:
* Offers an intuitive and simple graphical user interface 
* Can easily be adapted for educational and commercial uses.</small>

Thanks!
========================================================
incremental: false

<small>
Shiny App    
<a href="" target="_blank">Link</a>.

Shiny App Source Code on Github    
<a href="https://github.com/priyasdamodharan/Coursera-data-science-capstone" target="_blank">Link</a>.

Data Science Capstone on Coursera    
<a href="https://www.coursera.org/learn/data-science-project" target="_blank">Link</a>.


**References**
<small>
Thorsten Brants, Ashok C. Popat, Peng Xu, Franz J. Och, Jeffrey Dean. (2007), Large language
models in machine translation. In Proceedings of the 2007 Joint Conference on Empirical Methods
in Natural Language Processing and Computational Language Learning, pages 858-867.</small> 
