# Some general points about papers

* In graduate school, you need to write papers.  They are the main job-market signal about you if you want a job in a traditional academic department.    

* The first question you should ask before beginning a research project or collaboration is, "what paper are we going to write?"  This absolutely doesn't mean you shouldn't _also_ use some of your time to any of the following very useful activities: read papers not strictly about your research time, reproduce other people's methods or analyses, doodle math, run exploratory simulations for some random idea, and so on.  You absolutely _should_ do these things.  But I would put those in a fundamentally different category from the business of working on a research project and writing a research paper.  Let's call it "reading group" rather than "research project."   

* You should write your first paper as soon as you can.  
* Every paper must answer a fundamental question: What is my new contribution to human knowledge?  

* To a first-order approximation, there are two different kinds of papers: methods and applications.  "Methods" papers introduce a new method: an novel experimental technique, a new method of analyzing data, and so on.  "Applications" papers---we might also call them "real science" or "empirical" papers---are driven by new scientific findings.  

# Unicorns  

Before we talk about methods and applications papers separately, let's first talk about unicorns.  By a unicorn paper, I mean one that:  
- introduces a [fundamentally](https://tinyurl.com/y7fl5emf) [new methodology](https://www.jstor.org/stable/2346101) that is widely useful, and therefore immediately enters the "standard workflow" of practicing scientists in that area.  
- uses that new method to produce a novel, surprising, high-impact scientific finding.  

In other words, a unicorn is a clear outlier along both the methodological and scientific axes.

The overwhelming majority of papers are not unicorns.  I certainly have never written one.  In fact, when pressed, I can only think of a few examples, despite the fact that this is what every scientist I've ever talked to in some sense strives to write.  (Then again, I'm not a genetist or an astronomer or whatever; if you talk to them they'd probably be able to name unicorns in their field.)

Unicorns are usually sufficient (though not necessary) to make someone's scientific career.  You will probably never write a unicorn.  The rest of this guide will be about the other 99.999% of scientific papers.  


# Methods papers

This is almost surely the "simplest" kind of paper to write.  

1) Introduction
2) A formal problem statement and the lit review  
3) Your method
4) Benchmarking (sim studies)  
5) Real data examples
6) Pro forma discussion (usually pretty useless)  

# Applications papers 

Statisticians have a funny usage of the term "applications paper."  When I think of an applications paper, I think of a paper whose contribution to knowledge consists of new scientific findings.  Let's call this kind of thing a "real science" paper.  We'll discuss these below.

But this is not what an "applications paper" means in a statistics journal.  Here's what the Journal of the American Statistical Association considers an "Applications/Case Studies" paper:

1) For real datasets, present analyses that are statistically innovative as well as scientifically and practically relevant.  
2) Contribute substantially to a scientific field through the use of sound statistical methods.  
3) Present new and useful data, such as a new life table for a segment of the population or a new social or economical indicator.  
4) Using empirical tests, examine or illustrate for an important application the utility of a valuable statistical technique.  
5) Evaluate the quality of important data sources.  


Category 2 certainly sounds like a real science paper, and I suppose you could publish one of those in JASA.  However, the reality is that most "applications papers" are overwhelmingly from category 1.  Applications papers are still, despite the name, _fundamentally about statistical methodology_.  All you need to do is to visit the JASA (or Annals of Applied Statistics) website and see the list of accepted papers.  They are mostly methods papers that are applied in some non-trivial way to a real data set.

This has a couple of corollaries:  
- If you have made a new, interesting scientific discovery in genetics, neuroscience, or astronomy, don't waste that discovery by publishing it in a statistics journal.  
- You are making a grave mistake if you think that your applications paper about e.g. astronomy will be accepted or rejected on the basis of the inherent interest of its empirical findings to astronomers.  It will be accepted or reject on the basis of its inherent interest to statisticians.  Therefore you must write your applications paper with an audience of statisticians in mind.   


# Real applications papers, a.k.a. science papers  

This is a paper with a new scientific finding: some new discovery about stars, genes, financial markets, lemurs whose ancestors rafted to Madagascar, or whatever.  The rest of the scientific community doesn't call this kind of thing a "real applications paper."  They just call it a "paper."  I'll call it a "science paper" to distinguish it from the kind of methods-with-applications paper I described above.  

* Abstract that summarizes everything about the paper.  
* Introduction  
* Materials and methods  
* Results  
* Discussion  






# General advice for writing any kind of paper

### Know what the results are before you start writing the paper.

Nothing is more frustrating than to keep rewriting a paper because the methods and/or results keep changing.  If you are a statistician, you should insist that you collaborators follow this simple principle, and you should avoid collaborators who cannot adhere to it.  They are trouble because they do not respect your time.  If you a scientist, you should not expect your data-science collaborators to provide the methods section or results section of a paper whose results are not yet finalized.

### Write the results first

Once you know your paper's main results.  your paper's key findings first.  In a paper about a new statistical method, this might consist of a theorem or two, a set of simulation studies, and an application of the method to a real data set.  In a paper with new scientific findings, these are the actual findings:  
- Gene X predicts condition Y.  
- Our experiment discovered some cool new stuff about neurons.  
- We observed this star through our telescope and saw that it emitted photons in some unexpected part of the spectrum.  

The findings are the meat of the paper.  Write them first.

### Write the introduction last.

It's the hardest thing to write.  You _really_ need to know what you're going to say before you write an introduction.  If you sit down to write the introduction first, in all probability you'll just spin your wheels.  

### Do a good lit review.  

Actually read the papers you cite.  (Not necessarily front to back in complete detail, but absolutely for the main findings.)  

### Be humble.

Do not overclaim.

### Academic papers are not novels.  

Do not be clever.  Do not be flowery.  Do not be metaphorical.  Good scientific writing is direct, accurate, specific, and concise.  

### You can always tell a novice paper writer from the discussions section.  

### Good writers imitate.  Great writers steal.  

OK, I'm not saying to plagiarize.  But you could do a hell of lot worse than:
- reading lots of papers by someone whose writing you respect.  (I'll nominate Brad Efron as someone who writes great statistics papers.)  
- intentionally trying to write the paper in their style.  

### Software  

If a methods paper isn't worth writing software for, it isn't worth writing.  (This doesn't apply to _scientific_ methods papers.)  