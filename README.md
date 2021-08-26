# Introduction to the Digital Humanities: understanding sources about people and groups in time and space


[Random links to be integrated later: https://news.harvard.edu/gazette/story/2021/06/harvard-library-offers-new-way-to-see-colonial-north-america/

http://www.cs.cmu.edu/~ark/SEMAFOR/

https://stanfordnlp.github.io/CoreNLP/openie.html

 ]

The Introduction to Digital Humanities at Tufs can be taken as either CS 52 or as Classics 91. While the default course number indicates that the class is open to undergraduates, graduate students are encouraged to take this class as well by covering more work (primarily readings in secondary sources) and should talk to the instructor.   

The fall 2021 Introduction to Digital Humanities at Tufts University will focus on how we can use computational methods to understand sources that talk about people, individually and as groups, as they move through time and space. While we will focus on historical sources, the methods that we use can be applied to any sources that describe people in time and place. 

Learning outcomes include:

<ol>
<li>Initial exposure to the Digital Humanities as a field of study in its own right. We will treat the Digital Humanities as a space where ideas from the computational sciences and from the many subjects and disciplinary approaches of the Humanities interact. We view the term Digital Humanities as a helpful but transitional term. In fact, we live in a society in which ideas primarily circulate via digital media. The real topic of discussion is how the Humanities can, and should, evolve within a digital age.
<li>Hands-on experience with a range of methods by which members of the class can use Python to explore sources from the human record. While we will focus primarily upon materials in English, we will also explore methods by which to work with sources in languages that we do not know.
<li>Crtical assessment of what consitutes research in (one particular area within) the humanities will include questions such as: (1) What questions have traditionl scholars posed and how hav they published them? (2) How can we answer those questions with new digital methods? (3) What new questions might we ask beyond traditional research? (4) What new audiences can we reach and how would those audiences change the questions that we pose and the ideas that we publish?

</ol>

While we will develop a common vocabulary, members of the class will focus in their course projects on different topics. Ideally, class projects will be produced by teams of two or more students with complementary skills. 

<ol>
<li>September 8: Introduction to the course

<li>September 13: Micah Saxton -- text analysis exploration: the goal is to give students a hands-on example where a few lines of code generate visualizations that immediately illustrate differences between two texts. Default would be a comparison of Gibbon's Decline and Fall with Adam Smith's Wealth of Nations. We could simply use volume 1 of Gibbon, since volume 1 and Weath of Nations were both published in the same year, or we could just include all six volumes of Gibbon. Alternately, we could use an English translation of one of Gibbon's sources (such as Ammaianus Marecellinus). Then we would  probably want to select the sections of Gibbon that overlap with Ammianus. The differences would probably not be as dramatic and we would have the issue of the English translation (produced decades after Gibbon had died).

<li>September 15: Close reading of passages from Gibbon and Smith/Ammianus in light of the results. The point here is for students to see how they need the close reading to complement the exploratory data analysis (and to contextualize this with practices such as "ground truth" vs. remote sensing).

<li>September 20:  Micah Saxton -- Github intro

<li>September 22:

<li>September 27:

<li>September 29:

<li>October 4:

<li>October 6:

<li>October 11: HOLIDAY

<li>October 13:

<li>October 18:

<li>October 20:

<li>October 25:

<li>October 27:

<li>November 1:

<li>November 3:
<li>November 8:

<li>November 10:

<li>November 15:

<li>November 17:

<li>November 22:

<li>November 24: NO CLASS

<li>November 29: 

<li>December 1:

<li>December 6:

<li>December 8:

<li>December 13:
</ol>

The class will focus as a group on one particular source: Edward Gibbon's monumental Decline and Fall fo the Roman Empire. There are several reasons behind this choice.

1. The Decline and Fall, originally published in six volumes, is sufficiently large that few will be able to read it in its entirety and fewer still will be able to subject the whole text to traditional close reading. 
2. For statistical analysis, however, bigger is better.  The version of the Decline and Fall available from Project Gutenberg contains 1,594,885 space delimited tokens -- not a large corpus by computational standards but probably large enough to yield interesting results when analyzed quantatively and compared with other sources.

Sources for comparison include:

* Adam Smith, the Wealth of Nations (1776 -- the same year as volume of the Decline and Fall): this provides a comparison of genre but it also allows us to see if we can detect the places and periods that Smith mentions and compare them with those in Gibbon.

* English translations of the 19th century historical novels by Felix Dahn, which portray, from a German nationalist perspective, conflicts between Rome and group such as Goths, Vandals, and Huns. Can we detect differences in how different groups and historical figures are treated in Gibbon vs. Dahn? We could also explore issues of translation.



Here are some questions that we will pose.
<ol>
<li>What are the most common words in the Decline and Fall as a whole?  
<ol>
<li>Technical Questions
<ol>
<li>Stopwords -- do we want to view all words (including "the", "and" etc.) or do we want to create list of words that we ignore for the present (stopwords)
<li>Proper nouns will tell us a lot about content. What happens when we separate proper nouns from common nouns? How do we do so? How might the problem of excluding proper nouns differ in other languages?
</ol>
<li>Intellectual Questions
<ol>
<li>What do we learn from comparing the most frequent words in Decline and Fall with those of the reference corpus.
<li>What do we learn from comparing the most commmon words as we move from volume to volume and from chapter to chapter in Decline and Fall?
<li>What do we learn if we view frequencies in tabular form vs. word clouds? What might the impact of these varying formats be on more general audiences?
</ol>
</ol>
<li>Topic Models are <a href="https://en.wikipedia.org/wiki/Topic_model">a type of statistical model for discovering the abstract "topics" that occur in a collection of documents</a>. We address Topic Models now because we can implement them in a relatively straighforward way with existing libraries. 
<ol>
<li>Technical Questions
<ol>
<li>What different options do we have to implement Topic Models?
<li>Ideally, the class splits into different groups, each of which implements a different Topic Model library, evaluating ease of implementation, the speed of the service and any other issues that occur.
</ol>
<li>Intellectual Questions
<ol>
<li>Compare what we learn from topic models to what we learned from simple vocabulary analysis. This includes analysis of Decline and Fall as a whole, exploration of differing topics as we move through the text, and comparison of topics with those in the reference corpus.
<li>How do we manage proper names if we want to compare topics with and without proper names?
</ol>
</ol>
<li>Named Entity Recognition (NER) -- rule based approaches. Named Entity Recognition is a subtask of information extraction that recognizes and classifies names entities: e.g., does "Alexandria" in a particular context designate a place or a personal name? We will look at machine-learning based methods to perform this task but first we will look at rule based approaches. The reason for this is that existing NER systems are trained on recent documents (often newspaper collections) and the results can be quite noisy. If you are going to do serious work with sources that do not look like the default training set, you are going to have create a new training set to augment or replace that default training data that the ML-based system uses.
<ol>
<li>Look for key phrases that can identify particular classes of named entities, e.g., "<em>the River</em> Phasis" or "<em>the emperor</em> Hadrian." 
<ol>Evaluate how effective such phrases prove to be.
<li>Learn how to measure precision and recall.
<li>Consider both how many types of entity that
</ol>
<li>Identify the most frequent proper nouns and then manually classify the most important. 
<ol>
<li>How do you distinguish words in English that are capitalized because they show up at the start of a sentence from true proper names?
<li>How many names woud you need to classify before you have 50% of all the names in your corpus? 80%? 95%?
<li>What kind of visualizations could you use create if you only classified the most common N names in your corpus?
</ol>
</ol>

</ol>