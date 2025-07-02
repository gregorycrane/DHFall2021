# Introduction to the Digital Humanities: Understanding the Human Record

## Instructors: Gregory Crane (Gregory.Crane@tufts.edu), Bella Hwang (mailto:Boyoung.Hwang@tufts.edu), Peter Nadel (Peter.Nadel@tufts.edu), Jake Perl (Jake.Perl@tufts.edu)
## Thanks also to Anna Kijas, Patrick Florance, Micah Saxton 

Format: this is a hybrid class that will be taught, at least initially, in face-to-fae format. We will, however, make regular use of Zoom even when meeting in person. The Zoom link is available on Canvas under the Syllabus section.


The Introduction to Digital Humanities at Tufts can be taken as either CS 52 or as Classics 91. While the default course number indicates that the class is open to undergraduates, graduate students are encouraged to take this class as well by covering more work (primarily readings in secondary sources) and should talk to the instructors.   

The fall 2021 Introduction to Digital Humanities at Tufts University will focus on how we can use computational methods to understand sources that talk about people, individually and as groups, as they move through time and space. While we will focus on historical sources, the methods that we use can be applied to any sources that describe people in time and place. 

Learning outcomes include:

<ol>
<li>Hands-on experience with a range of methods by which members of the class can use Python to explore sources from the human record. While we will focus primarily upon materials in English, we will also explore methods by which to work with sources in languages that we do not know.
<li>Critical assessment of what consitutes research in (one particular area within) the humanities. This assessment will include questions such as: (1) What questions have traditionl scholars posed and how hav they published them? (2) How can we answer those questions with new digital methods? (3) What new questions might we ask beyond traditional research? (4) What new audiences can we reach and how would those audiences change the questions that we pose and the ideas that we publish?
</ol>

The class will focus as a group on one particular source: Edward Gibbon's monumental <a href="https://en.wikipedia.org/wiki/The_History_of_the_Decline_and_Fall_of_the_Roman_Empire">Decline and Fall of the Roman Empire</a>, published from 1776 through 1788 (roughly during the American War of Independence, 1776-1781, and just before the French Revolution, 1789-1799). There are several reasons behind this choice.

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

## Revised Course Schedule as of November 15, 2021
### Introductory topics
* September 8: The human record in a digital age

    Required:
    1. [Vannevar Bush. (1945) "As We May Think" The Atlantic.](https://www.theatlantic.com/magazine/archive/1945/07/as-we-may-think/303881/) (also on Canvas)  
    2. [Crane, Gregory. (2019). Beyond Translation: Language Hacking and Philology. Harvard Data Science Review, 1(2).](https://doi.org/10.1162/99608f92.282ad764)


* September 12: blog post #1 due (on Canvas): What are your goals from the class? And you can also talk about what experiences you have, whether in programming, studying the humanities or any other area, that you think would be helpful in this class. 
* September 13: [Google Colab](https://colab.research.google.com/) and Python basics.

    The first exercise will be very easy for those with experience programming. For those who have little or no such experience, this will require more work. Course staff members will work with those who are just getting started. The goal is that everyone has a working Python Script in Google Colab that we can discuss and modify in class.
    1. Write a Python script to count and then sort from most common to least common all words in Gibbon's <a href="https://en.wikipedia.org/wiki/The_History_of_the_Decline_and_Fall_of_the_Roman_Empire">Decline and Fall of the Roman Empire</a> and in Adam Smith's <a href="https://en.wikipedia.org/wiki/The_Wealth_of_Nations">Wealth of Nations</a>. What do we learn when we compare the two lists about the content of the two works?
        * [Decline and Fall of the Roman Empire txt](https://raw.githubusercontent.com/gregorycrane/DHFall2021/master/texts/declineandfall-gut.txt)
        * [Wealth of Nations txt](https://github.com/gregorycrane/DHFall2021/blob/master/texts/wealthofnations-gut.txt)
    2. Now produce sorted lists of <strong>upper-case</strong> words. What do we learn from these lists about the content of the two works?

    Colab Notebook: [Sorted Word Frequency in Gibbon and Smith](https://colab.research.google.com/drive/13IINBTQI-LYZyC8HIUPcQSIrHiFExQ-0?usp=sharing)

* September 15: Micah Saxton -- Github intro
    * Required (if possible do this before class):
        1. Set up a <a href="https://github.com/">Github</a> account if you don't already have one. 
        
            Pro tip:  choose a "professional" sounding username as it will appear in public urls you share with others.
        2. Download a basic text editor (not a word processor). We highly recommend <a href="https://code.visualstudio.com/">Visual Studio Code</a>.
        3. <strong>Windows Users</strong>: Download and install <a href="https://git-scm.com/downloads">git</a>.  (Follow installation prompts with all default options)
    * Recommended (Read and/or follow along to prepare)
        * <a href="https://guides.github.com/activities/hello-world/">Basic introduction to GitHub</a>
        * <a href="https://pages.github.com/">Basic introduction to GitHub Pages</a>
        * <a href="http://literaturegeek.com/2015/12/08/WhyJekyllGitHub">Introducing Static Sites for Digital Humanities Projects (why & what are Jekyll, GitHub, etc.?)</a>
        * <a href="https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages">Building a static website with Jekyll and GitHub Pages</a></br></br>

    We will be going through this in class together, so just read through to make yourself familiar.  It's okay if you don't understand much from this. NOTE: We will not be using the Github Desktop App. We will use the command line instead.

    Before class on September 22 [don't wait until Tuesday!]: As we finish work on the Jekyll blogs, add comments to the Canvas discussion list.

    Read and comment on a chapter of Gibbon. [The version of [the Decline and Fall at the Online Library of Liberty](https://oll.libertyfund.org/title/lecky-the-history-of-the-decline-and-fall-of-the-roman-empire-12-vols) is nicely presented for reading but feel free to use any version you choose]. 

    You can pick any chapter that catches your eye -- there are 71 to choose from and you can see summaries of their contents at the beginning of each volume. Chapters XV and XVI are famous because of their attack on Christianity. Chapter XXXI describes the invasion of Italy and the first sack of Rome by a figure named Alaric. Chapter LI goes beyond Europe and describes the Arabic conquest. There are many choices!

    You don't need to labor over every word. Read through the chapter quickly, get a sense of what is in it, looking to to do the following.
    1. Pick one story that stands out to you that you found particularly impressive.
    2. Summarize the main story and consider how you might be able to use maps, timelines, or other visualizations to tell that story in a way that makes it easier to follow.
    3. Identify two or more sentences where the language of Gibbon struck you as different from 21st century academic prose. You might focus on the complex sentence structure, vocabulary that seems odd to you or any other feature. We will talk about how to identify and explan such features automatically going forward.

### Distant reading (remote sensing vs. ground truth)

* September 19: post the Python script that you prepared for September 13 on your Github site. 

* September 20: Micah Saxton -- text analysis exploration.

    Colab Notebooks: 
    
    * [Text Analysis Exploration](https://colab.research.google.com/drive/1vutble1yuVizojMy3sR32N8Q2lkQxVjo?usp=sharing)

    * [Preparing Text for Analysis](https://colab.research.google.com/drive/1MuqaZC-P09-ykYXNt2AHJThF7B7QtQ24?usp=sharing)

### Named Entities Classification and Linking

* September 22: <strong>NB: Bring a charged laptop to class -- we will use Zoom to share screens so that you show members of the class your work. I will also use the Zoom chat to ask questions to which you can individually reply during class.</strong>

    * We will go over what you found when you analyzed the most frequent words in Gibbon and Smith.
    * Use Python and Regular Expressions to identify named entities. Demonstrate the limnitations of SpaCy and systems trained on different corpora. How do we bootstrap named entities for a new genre/topic? Different strategies: find the named entities and then classify them. Do you also want to "identify" them? what is the difference? 
    
        Strategies: 
        1. Start with the most common and work down.
        2. Pick a particular chunk and do it thoroughly.

    Colab Notebook: pending

    [Notes for Class](https://docs.google.com/document/d/1sLdtlOXbT2HV4cluLcpNbncHrB3SY0QxddPEZfwIlTM/edit#)
* September 26: See details on [Canvas](https://canvas.tufts.edu/courses/30895/assignments/200582).

* September 27: Evaluating your results: precision, recall, F-measure, limitations of evaluation (there is not always a known answer!). Evaluation in NLP vs. the Humanities. Journalistic prose vs. historical documents. Word sense disiambiguaion (experts disagree).  Assginment is to generate training data for SpaCy.

* September 29: Results on cleaned subsets of Gibbon,  we assign chapters and/or (sort of) random subsets (eg., every 100th page) Use the results of our work to train SpaCy and improve automated results.

    [Notes for Class](https://docs.google.com/document/d/171Q8PdtHHZgN2Aa1yY6dwmB8NYqjmDKc5-OYwREZ2ug/edit)
* October 3: Exercise #1 due (with blog #3)

### Topics from the professional humanists

* October 4:  What questions do Gibbon scholars ask? Can we pose them in a more systematic way using digital methods? Can we represent the topics more effectively in a digital medium than with print (or print surrogates)? What other questions might we ask that the professional scholars have not asked?

    [Notes for Class](https://docs.google.com/document/d/1NDLYRYoyw3zjLKzU1qPHCLQrOoT0kvCA_xRUvyfPRVA/edit)

### Topic Modeling -- Peter Nadel and Jake Perl

* October 6: Introduction to Topic Modeling
    * Required: "Spaces of Meaning: Conceptual History, Vector Semantics, and Close Reading" (on Canvas)

    Colab Notebook: [Intro to Topic Modeling](https://colab.research.google.com/drive/1G8utcCpXXw0Ovub8Pz7M5lRA3m2xSeVf?usp=sharing)

    Files Needed: gibbonfortm.xml (on Canvas)

* October 11: HOLIDAY

* October 13: Beautiful Soup Tutorial

    Colab Notebook: [Beautiful Soup Tutorial](https://colab.research.google.com/drive/1FD_z9H5vu96DHgJzyYN-V14Cb-1a8w2a?usp=sharing)

    Files Needed: 
    
    * [Hume html](https://www.gutenberg.org/cache/epub/10574/pg10574.html)

    * [Smith html](https://www.gutenberg.org/cache/epub/3300/pg3300-images.html)

* October 17: Exercise #2 and blog #4 due. 


###  Timelines, mapping and textual visualizations

* October 18: Mapping Place Names

    Colab Notebook: [Mapping Place Names](https://colab.research.google.com/drive/1CXveE89VqYLTTfEJsieY4ygffJUPvNRl?usp=sharing)

* October 20: 
* October 24: Exercise #3 and blog #5 due.




### Linguistic and Stylistic Analysis

* October 25: Carolyn Talmadge -- Introduction to GIS

    [Presentation Slides](https://tufts.app.box.com/v/Crane-GeoHumanitiesPowerPoint)
    
    Files Needed: all files under the "geospatial example data" folder on Canvas

* October 27: Text Classification

    1. Work with the corpus of chapters from Gibbon and Bryce we saw in class today and restructure it so that you have the same number of documents for each author. You can experiment with different numbers of documents to see what works best. (I have uploaded the whole text of each author, as in not segmented by chapter, to Canvas in case you find that easier to work with).

    2. Use the restructured corpus to train a new classification model using the notebook we looked at in class today.

    3. Post your accuracy results, confusion matrices and/or any issues you run into to Canvas.

    4. Try bringing in different test texts from other works of Gibbon/Bryce to see if your model can correctly guess the author.

    Colab Notebook: [Intro to Text Classification](https://colab.research.google.com/drive/1i5xrLQ2FT7hdzwe4QD-_FWRT0Z8OLIM9?usp=sharing)

    Files Needed: all files under the "text_classification" folder on Canvas

* October 31: Blog #6 due.

* November 1: Mapping Timelines

    Colab Notebook: [Mapping Timelines in Gibbon](https://colab.research.google.com/drive/1ldpUi-C4-g5clUT3cUPKC42Bs6tWaTWa?usp=sharing)

    [Notes for class](https://docs.google.com/document/d/1n_wO6f0kJ6rOqGkUhNgQdP_2OFTCZs1fHGPNTkTAEaI/edit#)

* November 3: Introduction to morpho-syntactic analysis with Stanza

    Colab Notebook: [Intro to Stanza](https://colab.research.google.com/drive/1McJeN1kz8OeZmSJlaL55Inl622WlvvyB?usp=sharing)

* November 7: Exercise #4 and blog #7 due.

### Text Alignment and Text Reuse Detection

* November 8: Aligning two versions of a text (e.g., Gutenberg vs. Library of Liberty versions of Gibbon) 

    Colab Notebook: [Manual Text Alignment](https://colab.research.google.com/drive/1XvU5fbwiPbCyEWAxOgqOchtgx4Rbd8UD?usp=sharing)

* November 10: Dependency grammar and reading texts in unknown languages 

    Colab Notebook: [Dependency Trees](https://colab.research.google.com/drive/1uxK61hP3_k4tdQIHv9KHIW8iPmnDw5P2?usp=sharing)

* November 14. 

### Network Analysis

* November 15: 

* November 17.

* November 22: [Notes for Class](https://docs.google.com/document/d/1DuGuKIdvMRIxXXkruDGqtepk04rv2lpcW2YoE5nP8Cw/edit)

* November 24: NO CLASS

* November 28: Exercise #6 and blog #10 due.

### Music History
* November 29: Anna Kijas, DH and Music History

### Class Projects
* December 1: 

* December 6: 

* December 8: 

* December 13:

###  Final Project

* December 16: Final Projects Due