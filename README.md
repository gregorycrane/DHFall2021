# Introduction to the Digital Humanities: Understanding the Human Record

## Instructors: Gregory Crane, Peter Nadel, Jake Perl



The Introduction to Digital Humanities at Tufts can be taken as either CS 52 or as Classics 91. While the default course number indicates that the class is open to undergraduates, graduate students are encouraged to take this class as well by covering more work (primarily readings in secondary sources) and should talk to the instructors.   

The fall 2021 Introduction to Digital Humanities at Tufts University will focus on how we can use computational methods to understand sources that talk about people, individually and as groups, as they move through time and space. While we will focus on historical sources, the methods that we use can be applied to any sources that describe people in time and place. 

Learning outcomes include:

<ol>
<li>Hands-on experience with a range of methods by which members of the class can use Python to explore sources from the human record. While we will focus primarily upon materials in English, we will also explore methods by which to work with sources in languages that we do not know.
<li>Critical assessment of what consitutes research in (one particular area within) the humanities. This assessment will include questions such as: (1) What questions have traditionl scholars posed and how hav they published them? (2) How can we answer those questions with new digital methods? (3) What new questions might we ask beyond traditional research? (4) What new audiences can we reach and how would those audiences change the questions that we pose and the ideas that we publish?
<li>A new understanding of how the human record can contribute to the intellectual life of humanity. We view the term Digital Humanities as a helpful but transitional term. In fact, we live in a society in which ideas primarily circulate via digital media. The real topic of discussion is how the Humanities can, and should, evolve within a digital age and how we can reimagine the 
</ol>

The class will focus as a group on one particular source: Edward Gibbon's monumental Decline and Fall fo the Roman Empire. There are several reasons behind this choice.

<ol>
<li>The Decline and Fall, originally published in six volumes (published between 1776 and 1788), is sufficiently large that few will be able to read it in its entirety and fewer still will be able to subject the whole text to traditional close reading. 
<li>For statistical analysis, however, bigger is better.  The version of the Decline and Fall available from Project Gutenberg contains 1,594,885 space delimited tokens -- not a large corpus by computational standards but probably large enough to yield interesting results when analyzed quantatively and compared with other sources.
<li>The Decline and Fall captures a critical moment in time. The first volume was published in 1776 and is contemporaneous with the Declaration of Independence as well as with the publication by Adam Smith of the Wealth of Nations. The distance in time makes it much easier for us to sense that Gibbon is looking at the past from a present that is very different from the world in which we live and the world that we may wish to fashion. 
<li>While the Decline and Fall is written in English, it draws upon, and often quotes, sources in languages such as French, Latin, and Ancient Greek. This gives us an opportunity to explore methods by which we can use new digital methods work with sources in languages that we do not know.
</ol>

While we will develop a common vocabulary and shared set of skills, members of the class will focus in their course projects on different topics. Ideally, class projects will be produced by teams of two or more students with complementary skills.

Your work during the course will be created as a porfolio that you will create on GitHub (which we will introduce in week 2 for those who are not familiar with it).

## Requirements
<ol>
<li>Weekly blog posts. The first post will be on a Discussion site on Canvas but we will use Github for the others. These would be typically one to two pages (c. 250-500 words). These will comment on what you learned from the classes, from the readings (although we may assign different topics during the semester) and from the assignments. These are due by Midnight each Sunday.
<li>Those students who take the course as Classics 191 (or possibly CS 150) will be expected to read, and summarize for the class, publications from Computer Science and the Humanities.
<li>Five exercises assigned during the semester. In the weeks when you have an exercise, your class blogs will focus on what you have learned from the exercise.
<li>A final project of your that includes (1) code of some kind, (2) information that other people will find useful about Gibbon (or whatever topic you choose), and (3) an explanation of what you did, why you did it and what you learned.
</ol>

## Initial Course Schedule
<ul>
<li>September 8: The human record in a digital age
</ul>

### Introductory topics
#### Required work: 
<ul>
<li>https://www.udemy.com/course/git-expert-4-hours/
<li>Read 
<ol>
<li>Vannevar Bush. (1945) "As We May Think" The Atlantic. https://www.theatlantic.com/magazine/archive/1945/07/as-we-may-think/303881/ (also on Canvas)  
<li>Crane, Gregory. (2019). Beyond Translation: Language Hacking and Philology. Harvard Data Science Review, 1(2). https://doi.org/10.1162/99608f92.282ad764
</ol>
</ul>

<ul>
<li>September 12: blog post #1 due (on Canvas): what are your goals from the class?

<li>September 13: Dual track: (1) Python basics; (2) for those comfortable with Python, we work on converting XML and HTML to a suitable plain text format. This can involve discussion of markup (ie., what are we throwing out when we "clean" the text?)



<li>September 15:   Micah Saxton -- Github intro
</ul>

### Distant and close reading (remote sensing vs. ground truth)

<ul>
<li>September 20: Micah Saxton -- text analysis exploration.

<li>September 22: Close reading of passages from Gibbon and one or more of Gibbon's sources.

<li>September 26: Blog #2 due (on Github from now on).
</ul>

### Topic Modelling -- Peter Nadel and Jake Perl

<ul>
<li>September 27:

<li>September 29:  

<li>October 3: Exercise #1 due (with blog #3)

</ul>

### Named Entities Classification and Linking

<ul>

<li>October 4: Use Python and Regular Expressions to identify named entities. Demonstrate the limnitations of SpaCy and systems trained on different corpora. How do we bootstrap named entities for a new genre/topic? Different strategies: find the named entities and then classify them. Do you also want to "identify" them? what is the difference? Strategies: (1) start with the most common and work down; (2) pick a particular chunk and do it thoroughly.

<li>October 6: Evaluating your results: precision, recall, F-measure, limitations of evaluation (there is not always a known answer!). Evaluation in NLP vs. the Humanities. Journalistic prose vs. historical documents. Word sense disiambiguaion (experts disagree).  Assginment is to generate training data for SpaCy.



<li>October 11: HOLIDAY

<li>October 13: Exercise #2 and blog #4 due. Results on cleaned subsets of Gibbon,  we assign chapters and/or (sort of) random subsets (eg., every 100th page) Use the results of our work to train SpaCy and improve automated results. 

</ul>


### Maps and Timelines


<ul>
<li>October 16: Blog due

<li>October 18: 

<li>October 20:

</ul>



Linguistic and Stylistic Analysis

<ul>


<li>October 25:  Introduction to morpho-syntactic analysis with Stanza

<li>October 27:  Dependency grammar and reading texts in unknown languages


<li>November 1: Language Models and Stylistic Analysis

<li>November 3: Exercise #3 due.
</ul>

Text Alignment and Text Reuse Detection

<ul>
<li>November 8: Aligning two versions of a text (e.g., Gutenberg vs. Library of Liberty versions of Gibbon) 

<li>November 10: Finding quotations of one text in another

<li>November 15: Exercise #4 due. Aligning source text and translation
</ul>

### Network Analysis

<ul>
<li>November 17: 

<li>November 22: Exercise #5 due.

<li>November 24: NO CLASS
</ul>

### Music History
<ul>

<li>November 29: Anna Kijas, DH and Music History
</ul>

### Class Projects
<ul>
<li>December 1: 

<li>December 6: 

<li>December 8: 

<li>December 13:
</ul>

###  Final Project

<ul>
<li>December 16: Final Projects Due
</ul>



