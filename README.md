# CMSI3801 Final -- Educational Webscraper #
### Created by Gage Messner and Thomas Powell ###

## Overview ##
For our final project, we wanted to implement a webscraper of some sort. We eventually settled on a webscraper that the user can interact with seamlessly and use for educational purposes. So, we first made an web application using Anvil, an easy-to-use webApp builder that cuts out the dirty work of wrestling with HTML. Our application looks for a topic, or list of topics, within a URL. You give our application both the topics and URL. Once it is satisfied with the findings, it then hops on over to ChatGPT with it's findings and in return, ChatGPT gives us a concise summary of the topic (or topics) from that webpage. For example, I want to find out more about the consequences of artificial intelligence from a specific source and I don't have time to look through a whole peer-reviewed article. So I open my webApp, give it the URL of my source and give it the topics "health care, automobile innovation and education." The result is a short summary of what our bot found on those topics.

## Our Goal ## 
You might ask, "why can't I just ask ChatGPT itself, and cut out the middle-man?" This is a great question. We all know that ChatGPT can spit out loads of misinformation. Our aim is to cut down the amount of data that ChatGPT can pull from in such a large data set, such as a peer-reviewed paper. This way, we are not contaminating the output with false information from other sections that may not be relevant to our topics. Concurrently, we also look to eliminate the amount of work the user has to do in order to find good results.

## Specs ##

### Class ScrapedData:

1. Contains our webscraper

### def raw_data(url):


1. Takes in the URL given by the user
2. Works with the html from the URL, parses through and finds the topic that the user gives
3. Outputs the paragraph under said topic
