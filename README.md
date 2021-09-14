# Introduction to the Digital Humanities: Understanding the Human Record

## Instructors: Gregory Crane, Bella Hwang, Peter Nadel, Jake Perl
## Thanks also to Anna Kijas, Patrick Florance, Micah Saxton 

Format: this is a hybrid class that will be taught, at least initially, in face-to-fae format. We will, however, make regular use of Zoom even when meeting in person. The Zoom link is available on Canvas under the Syllabus section.


The Introduction to Digital Humanities at Tufts can be taken as either CS 52 or as Classics 91. While the default course number indicates that the class is open to undergraduates, graduate students are encouraged to take this class as well by covering more work (primarily readings in secondary sources) and should talk to the instructors.   

The fall 2021 Introduction to Digital Humanities at Tufts University will focus on how we can use computational methods to understand sources that talk about people, individually and as groups, as they move through time and space. While we will focus on historical sources, the methods that we use can be applied to any sources that describe people in time and place. 

Learning outcomes include:

<ol>
<li>Hands-on experience with a range of methods by which members of the class can use Python to explore sources from the human record. While we will focus primarily upon materials in English, we will also explore methods by which to work with sources in languages that we do not know.
<li>Critical assessment of what consitutes research in (one particular area within) the humanities. This assessment will include questions such as: (1) What questions have traditionl scholars posed and how hav they published them? (2) How can we answer those questions with new digital methods? (3) What new questions might we ask beyond traditional research? (4) What new audiences can we reach and how would those audiences change the questions that we pose and the ideas that we publish?
</ol>

The class will focus as a group on one particular source: Edward Gibbon's monumental <a href="https://en.wikipedia.org/wiki/The_History_of_the_Decline_and_Fall_of_the_Roman_Empire">Decline and Fall fo the Roman Empire</a>, published from 1776 through 1788 (roughly during the American War of Independence, 1776-1781, and just before the French Revolution, 1789-1799). There are several reasons behind this choice.

<ol>
<li>The Decline and Fall, originally published in six volumes (published between 1776 and 1788), is sufficiently large that few will be able to read it in its entirety and fewer still will be able to subject the whole text to traditional close reading. 
<li>The Decline and Fall exists already in multiple digital forms, none of which has, however, been systematically analyzed with digital methods. This includes full scans of the earlier editions (such as <a href="http://access.bl.uk/item/viewer/ark:/81055/vdc_100045279307.0x000001#?c=0&m=0&s=0&cv=5&xywh=-123%2C0%2C3291%2C2459">the 1792 edition at the British Library</a>) along with a first pass at <a href="https://github.com/gregorycrane/DHFall2021/blob/master/texts/K065082.001.xml">transcription and markup</a> that can be freely enhanced.
<li>For statistical analysis, however, bigger is better.  The version of the Decline and Fall available from Project Gutenberg contains 1,594,885 space delimited tokens -- not a large corpus by computational standards but probably large enough to yield interesting results when analyzed quantatively and compared with other sources.
<li>The Decline and Fall captures a critical moment in time. The first volume was published in 1776 and is contemporaneous with the Declaration of Independence as well as with the publication by Adam Smith of the Wealth of Nations. The distance in time makes it much easier for us to sense that Gibbon is looking at the past from a present that is very different from the world in which we live and the world that we may wish to fashion. 
<li>While the Decline and Fall is written in English, it draws upon, and often quotes, sources in languages such as French, Latin, and Ancient Greek. This gives us an opportunity to explore methods by which we can use new digital methods work with sources in languages that we do not know.
<li><a href="http://access.bl.uk/item/viewer/ark:/81055/vdc_100045279307.0x000001#?c=0&m=0&s=0&cv=49&xywh=-154%2C-1%2C3315%2C2478">The citations to primary and secondary sources in Gibbon's footnotes</a> are already, for the most part, those of modern scholarship. Learning how to analyze Gibbon's references teaches us how to learn how to analyze references is contemporary scholarship.
<li>The work of this class can lead to the publication of some, or even all, of the Decline and Fall of the Roman Empire in <a href="https://beyond-translation.perseus.org/">the new version of the Perseus Digital Library</a>.
</ol>

While we will develop a common vocabulary and shared set of skills, members of the class will focus in their course projects on different topics. Ideally, class projects will be produced by teams of two or more students with complementary skills.

Your work during the course will be created as a porfolio that you will create on GitHub (which we will introduce in week 2 for those who are not familiar with it).

## Requirements
<ol>
<li>Weekly blog posts. The first post will be on a Discussion site on Canvas but we will use Github for the others. These would be typically one to two pages (c. 250-500 words). These will comment on what you learned from the classes, from the readings (although we may assign different topics during the semester) and from the assignments. These are due by Midnight each Sunday.
<li>Those students who take the course as Classics 191 (or possibly CS 150) will be expected to read, and summarize for the class, publications from Computer Science and the Humanities.
<li>Six exercises assigned during the semester. In the weeks when you have an exercise, your class blogs will focus on what you have learned from the exercise.
<li>A final project of your that includes (1) code of some kind, (2) information that other people will find useful about Gibbon (or whatever topic you choose), and (3) an explanation of what you did, why you did it and what you learned.
</ol>

## Initial Course Schedule
<ul>
<li>September 8: The human record in a digital age
</ul>

### Introductory topics
#### Required work: 



<ol>
<li>Vannevar Bush. (1945) "As We May Think" The Atlantic. https://www.theatlantic.com/magazine/archive/1945/07/as-we-may-think/303881/ (also on Canvas)  
<li>Crane, Gregory. (2019). Beyond Translation: Language Hacking and Philology. Harvard Data Science Review, 1(2). https://doi.org/10.1162/99608f92.282ad764
</ol>
</ul>
</ul>

<ul>
<li>September 12: blog post #1 due (on Canvas): what are your goals from the class? And you can also talk about what experiences you have, whether in programming, studying the humanities or any other area, that you think would be helpful in this class. 
<br/>
<li>September 13: https://colab.research.google.com/ and Python basics 
The first exercise will be very easy for those with experience programming. For those who have little or no such experience, this will require more work. Course staff members will work with those who are just getting started. The goal is that everyone has a working Python Script in Google Colab that we can discuss and modify in class.
<ol>

<li>Write a Python script to count and then sort from most common to least common all words in Gibbon's <a href="https://en.wikipedia.org/wiki/The_History_of_the_Decline_and_Fall_of_the_Roman_Empire">Decline and Fall of the Roman Empire</a> and in Adam Smith's <a href="https://en.wikipedia.org/wiki/The_Wealth_of_Nations">Wealth of Nations</a>. What do we learn when we compare the two lists about the content of the two works?
<ul>
<li>https://raw.githubusercontent.com/gregorycrane/DHFall2021/master/texts/declineandfall-gut.txt
<li>https://github.com/gregorycrane/DHFall2021/blob/master/texts/wealthofnations-gut.txt
</ul>
<li>Now produce sorted lists of <strong>upper-case</strong> words. What do we learn from these lists about the content of the two works?
</ol>




<li>September 15:   Micah Saxton -- Github intro
<ul>
<li>Required (if possible do this before class):
<ul>
Set up a <a href="https://github.com/">github</a> account if they don't already have one. 
Pro tip:  choose a "professional" sounding username as it will appear in public urls you share with others.
<li>Download a basic text editor (not a word processor). We highly recommend
<a href="https://code.visualstudio.com/">Visual Studio Code</a>.
<li><strong>Windows Users</strong>: 
Download and install <a href="https://git-scm.com/downloads">git</a>  (Follow installation prompts with all default options)
</ul>
<li>Recommended (Read and/or follow along to prepare)
<ul>
<li><a href="https://guides.github.com/activities/hello-world/">Basic introduction to GitHub</a>
<li><a href="https://pages.github.com/">Basic introduction to GitHub Pages</a>
<li><a href="http://literaturegeek.com/2015/12/08/WhyJekyllGitHub">Introducing Static Sites for Digital Humanities Projects (why & what are Jekyll, GitHub, etc.?)</a>
<li><a href="https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages">Building a static website with Jekyll and GitHub Pages</a>
</ul>
</ul>
We will be going through this in class together, so just read through to make yourself familiar.  It's okay if you don't understand much from this. NOTE: We will not be using the Github Desktop App. We will use the command line instead.

</ul>



<ul>
<li>September 19: post the Python script that you prepared for September 13 on your Github site.

</ul>

### Distant reading (remote sensing vs. ground truth)

</ul>

<li>September 20: Micah Saxton -- text analysis exploration.

</ul>

### Named Entities Classification and Linking

<ul>

<li>September 22: Use Python and Regular Expressions to identify named entities. Demonstrate the limnitations of SpaCy and systems trained on different corpora. How do we bootstrap named entities for a new genre/topic? Different strategies: find the named entities and then classify them. Do you also want to "identify" them? what is the difference? Strategies: (1) start with the most common and work down; (2) pick a particular chunk and do it thoroughly.

<li>September 26: Blog #2 due (on Github from now on).




<li>September 27: Evaluating your results: precision, recall, F-measure, limitations of evaluation (there is not always a known answer!). Evaluation in NLP vs. the Humanities. Journalistic prose vs. historical documents. Word sense disiambiguaion (experts disagree).  Assginment is to generate training data for SpaCy.

<li>September 29: Results on cleaned subsets of Gibbon,  we assign chapters and/or (sort of) random subsets (eg., every 100th page) Use the results of our work to train SpaCy and improve automated results.

<li>October 3: Exercise #1 due (with blog #3)

</ul>

### Topics from the professional humanists

<ul>


<li>October 4:  What questions do Gibbon scholars ask? Can we pose them in a more systematic way using digital methods? Can we represent the topics more effectively in a digital medium than with print (or print surrogates)? What other questions might we ask that the professional scholars have not asked?
</ul>

### Topic Modelling -- Peter Nadel and Jake Perl

<ul>
<li>October 6: 



<li>October 11: HOLIDAY

<li>October 13:  

<li>October 17: Exercise #2 and blog #4 due. 
</ul>


###  Timelines, mapping and textual visualizations


<ul>


<li>October 18: 

<li>October 20:
<li>October 24: Exercise #3 and blog #5 due.
</ul>



### Linguistic and Stylistic Analysis

<ul>


<li>October 25:  Introduction to morpho-syntactic analysis with Stanza

<li>October 27:  Dependency grammar and reading texts in unknown languages

<li>October 31: Blog #7 due.
<li>November 1: Language Models and Stylistic Analysis

<li>November 7: Exercise #4 and blog #8 due.
</ul>

### Text Alignment and Text Reuse Detection

<ul>
<li>November 8: Aligning two versions of a text (e.g., Gutenberg vs. Library of Liberty versions of Gibbon) 

<li>November 10: Finding quotations of one text in another; Aligning source text and translation

<li>November 14: Exercise #5 and blog #9 due. 
</ul>

### Network Analysis

<ul>
<li>November 15: 

<li>November 17:


<li>Blog #10 due

<li>November 22:

<li>November 24: NO CLASS

<li>November 28: Exercise #6 and blog #11 due.
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



