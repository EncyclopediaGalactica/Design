# Design repository for Encyclopedia Galactica

Encyclopedia Galactica got its name from Isaac Asimov's epic Foundation novel series.

The purpose of this software to provide a solution to be able to store all type of data
in a structured way, so later processing is easier. This Design repo describes how.

## Vision

Let's start with the big words... My intention is to create something which can store all 
data we have (yes, books, documents, video files, html sites, pdfs and all the crap we have 
been producing for a long while) in a format where it is relatively easy to find the 
connections between the information pieces. The less grandiose form of this is the 
following: there are information curators who are building a database representing the 
human race knowledge for another race. Did I tell you that I'm a naive librarian? :)

Imagine that...

you are an investor who manages his/her capital and searches for information. The 
information needed here contains news, economy data including micro and macro, statistics 
and especially consumer and consumer segments and so on. You have a system where all the 
data is available. Moreover, the system feeds the news and looks for connections between 
them using different contextual searches.

There is a system where all the sources are connected, so news, statistics, science papers, 
video feeds and all the nice things are connected. There are algorithms processing these 
sources and looks for connections between content based-on either algorithms or preferences 
you set up. As a result you are able to see, for example, the newest science papers from 
social sciences field and you also get relevant hits to other papers, or you can oversee 
what other papers are available on the given field. You are also able to attach the news to 
the selected topic, youtube videos and so on

You want to organise data in this system, and you can do it because the system has the 
capability to create structures which puts some structure around the raw data. For example, 
using thesaurus you can build up what a science (social sciences) field looks like and what 
connections it has. Using this structure you can organise science papers, news, videos, 
primer and secunder information sources. Moreover, based-on contextual searches the system 
can offer you possible hits and you can decide whether these are relevant or not.

You have to record data, but along certain parameters the data is slightly different. For 
example, you are recording addresses. An address looks slightly different in Germany, UK 
and Hungary. But, the abstract "let's put a textfield there" isn't a good solution, you 
need precision. The system makes possible to describe the data structure you are working 
with, it creates form for it and offers comfortable way to change the input field, so you 
can work easily with your data.

There is the system where to all the data sources are connected, and the system offers the 
capability to describe the input data structure, so the data is stored in a processable format.

## Data structures

- [SourceFormats](./data_structures/source_formats/README.md)

## Software Architecture
