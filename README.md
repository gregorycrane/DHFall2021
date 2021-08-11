# Introduction to the Digital Humanities: understanding sources about people and groups in time and space


[Random links to be integrated later: https://news.harvard.edu/gazette/story/2021/06/harvard-library-offers-new-way-to-see-colonial-north-america/ ]


The fall 2021 Introduction to Digital Humanities at Tufts University will focus on how we can use computational methods to understand sources that talk about people, individually and as groups, as they move through time and space. The class will focus as a group on one particular source: Edward Gibbon's monumental Decline and Fall fo the Roman Empire. There are several reasons behind this choice.

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