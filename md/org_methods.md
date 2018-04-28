# Organizing methods talks  

So you've invented a new method and now want to tell people about it.  Cool!  Here's a suggested outline.  
- Title slide.  
- One motivating example.  
- Take-home messages: key claims about your method.  
- Description of the new method.  
- Evidence that the method works.    
- The end.  

I'll describe each of these sections in turn.  Again, the bias here is toward short talks, although I think the same broad outline works for long talks.  I'll mention some differences at the end.  

Note: this outline won't necessarily cover _all_ methods talks.  Still, it would certainly be appropriate for most of them that I've ever seen, which is a lot.  If you have some experience giving talks, you might find some of this organizational advice to be overly prescriptive.  In that case, feel free to disregard or modify it.  But remember, my goal here is to provide a plug-and-play guide for PhD students in data-science, not for seasoned scientific communicators.  

## The title slide

All this needs is the title of the talk, your name and affiliation, the names (and affiliations, if there's room) of your collaborators/funders.  Don't be a dick by failing to acknowledge your collaborators.  

## One motivating example  

I am a strong advocate of beginning every methods talk with a single clear, compelling example.  In a short talk especially, I think this should start from slide 2, immediately after the title slide.  No need for an outline.  

### Why start with an example?  

You should assume that your audience has a default skepticism of the need for a new method in the first place.  ("Stop telling me my old things don't work, and get offa' my lawn!")  Even if they don't hold this view, assuming that they do is a powerful rhetorical strategy anyway.  Therefore your primary duty is to _melt away their skepticism._  You might as well do it from the very beginning.  There is no clearer way than an awesome motivating example to establish _why_ there is a need for your method in the first place.

The perfect motivating example has the following properties:  
- you can explain the example in a picture or two, with maybe one slide of text  
- there is some clear off-the-shelf procedure that reasonable people might reach for in order to approach this problem  
- But there are some issues with this off-the-shelf procedure that you can articulate, or even better, see in a picture.  
- Your method, on the hand, addresses these issues, or most of them, without trouble.  

### Organizing your "motivating example" section  

The archetypal "motivating example" section of a talk has three sub-parts.

First, explain the scientific problem and the data set.  Ideally you can do this in no more than 2-3 slides -- on occassion maybe more, but only if the problem is really complicated _and_ those complications are essential for understanding what comes next.  (Remember, keep it simple.)  For example, one slide might describe the scientific problem (text or pictures.  A second slide might provide some key facts about your data set. (This would be a reasonable a reasonable use of a bulleted list, so that people can read some facts about it as they listen to you describe stuff.)  Then a third slide might be a picture of the data.  You might not need all three.  

Second, you should show the results from applying an off-the-shelf, existing method to this data.  If you can do this in one picture, great.  This is your "straw man": the thing your method should beat.

In this context, you can also briefly mention other existing methods that might be appropriate for your problem, other than the one you've shown.  But this is mainly to telegraph to people that you've done your work.  You should explain that comprehensive benchmarks are the paper, and that your choice of Existing Method X on your motivating example is only intended to be illustrative.  

Third and finally, you should explain what's wrong/suboptimal with the off-the-shelf method.  This tells the audience why they should pay attention when you introduce your new method.  Again, try to do this in one slide at most.

### "I can't think of a motivating example where I can show all three of those things."   

Then why, exactly, did you write your methods paper?  

OK, I suppose the exception might be if you've invented a method for a brand new type of data-collection protocol in some scientific field, where there is no pre-existing state of the art for data analysis.  That's rare -- but if that describes your situation, then just explain the problem and give a concise summary of the statistical issues you found yourself needing to address.  

## Take-home messages

OK, we've just seen the motivating example, and we've learned that it has some features that aren't well handled by existing methods.  So what are the key improvements on this example that your new method is capable of delivering?

The "take-home messages" section should be very short. The goal here is to **summarize your key claims,** not to provide extensive evidence for those claims.  Keep this section to one or two slides.  Bulleted lists are good here, for "information redundancy" purposes.  Ideally, these bullets should map in a fairly clear way to the summary you just gave -- the one about why existing methods don't work so great on your motivating example.  

For instance, not too long ago I worked Wesley Tansey on a technique for [multiple hypothesis testing that improves power by exploiting spatial structure](https://arxiv.org/abs/1411.6144).  Wes's take-away messages for talks about this method went something like this:    
- Our method exploits spatial structure in the test statistics.  
- It respects the nominal FDR while improving power.  
- It is scalable to very large graphs, with 10^6 nodes or more.  
- It outperforms other methods across 20 simulated and 5 real data sets.  

I also recently worked with another student, Oscar Padilla, who invented a new technique for [linear-time spatial smoothing across a large discrete lattice](https://arxiv.org/abs/1608.03384), called the DFS fused lasso.  Oscar's take-home messages were something like this:  
- The DFS fused lasso can estimate a noisy signal on an arbitrary graph in linear time.  
- It exploits a key property of depth-first search on graphs.  
- The error rate improves upon existing error bounds for noisy signals on arbitrary graphs.  

I also remember a talk from Jennifer Hill at ISBA 2014 about causal inference using Bayesian ensemble methods.  Here take-home messages went something like this:  
- Our method models both the treatment assignment and the response variable nonparametrically.  
- It yields full posterior distributions for heterogeneous treatment effects without strong assumptions.  
- It also provides state-of-the-art performance for estimating average treatment effects.  

I could list dozens or hundreds of examples.  The point is, you should have one slide summarizing the few key messages that you want the listener to take away from the talk.  Make specific claims that you can back up in your subsequent slides.  Some claims might be about the method itself (e.g. it's key source of advantage).  Others will be claims about its performance.  

Once you've got that out of the way, you might give a "teaser" slide about your method's results for your motivating example.  After summarizing your method and it's advantages.  

## Description of the new method  

In progress.  Basic idea: explain the method as simply as you can.  The key question here is _why_: specifically, why the method works better.  What is the minimum amount of detail necessary for people to appreciate the nature of the improvement you've made?  Use pictures where possible.  Defer key details to the paper.  

I also like to finish the "description of method" slide with a single bulleted list that mentions two or three key details that I've omitted.  These show the audience that you've anticipated their questions, but that you simply haven't had the time to cover them right there and then.  

## Evidence that the method works

This could take many forms.  But in short talks, I like to do this in three parts:  
- a toy example that clearly illustrates the way your method improves upon the existing state of the art.  Pictures are better than formal performance metrics (although both are good).  
- your motivating example from the introduction of the talk.  How does your method actually do here.  
- a single easily understood table of simulation results.  Maybe this is simulated data, maybe it's out-of-sample performance on real data -- whatever.  Just make it simple!  

I like my three-part approach because I've found it to be rhetorically effective as an audience member.  When someome shows you how their method works on a really simple example, you are likely to "get it" more readily.  ("Oh, I see why that works so well.")  Once you're there, you're primed to see the more complicated (real) example.  Finally, it's also nice when someone goes on to show you: hey it's not just these two examples!  Here are some simulation studies.  Then they show you a table of results.  (You know the kind I mean: the kind where every data set is a row, every method is a column, and the bolded entry wins that row.)    

But you have to know how to handle this table in your talk.  Its key purpose is to telegraph to the listener that you have done some comprehensive benchmarking on the method, and to remind them that the full details are in the paper.  In a short talk especially, there is simply no time to go into those details right now.  Therefore, emphasize on of two things, depending on context:  
1) _Variety_.  Suppose the sim study is a total run-away victory for your new thing.  Look how many bolded entries are in your column!  Look how much smaller the errors are!  In this case, don't bother emphasizing the precise details of the data sets or simulation settings.  Instead, emphasize the _range_ of simulation studies you considered (whether it's a range of real data sets, or a wide range of known ground-truth settings).  
2) _Contrast_.  In most well-designed sim studies, sometimes your methods wins and sometimes it doesn't.  Here, again, don't well on the individual details of the simulations.  Try to make some broad generalizations about the cases where your method works well, and the cases where it doesn't work so well.  

Either way, I recommend limiting yourself to a single table from simulation studies.  A single such table can be rhetorically effective, in the manner I've just described.  Any more than two is frankly just boring as hell.  Have the rest of your tables as backup slides. 

## The end

Your last slide should have a reference (or maybe even a scannable QR code) to your paper and/or software package.  If you have room, include the names of your collaborators/funders again on the final slide.

When you get to your last slide, verbally conclude by doing three things: 
1) Remind the audience of the few take-home messages from the beginning of the talk.  A sentence or two is all.  
2) Remind tthem that the details you've omitted are in the paper.  
3) Thank the audience for their attention.

Congratulations, you're done!  


## What's different about a long talk  

I've geared this advice toward short talks.  But I still like the same broad outline for longer talks in the 45-minute range.  The main difference is the amount of detail you can convey.  For example:  

- You can tell the scientific story behind the motivating example in more detail.  
- You can do a more comprehensive overview of pre-existing methods.  
- You can do a better post-mortem on why those pre-existing methods don't work as well as yours.  What are their failure modes?    
- You can include more than one motivating example at the beginning, if you'd like.  
- You can have a more comprehensive results/evidence section -- although please, not too many tables.  
- You have time to talk in some detail about future directions, unsolved problems, etc.  
- You can give more detail on the method itself -- though not as much as you'd think!  Most people just won't be super interested in the nitty-gritty details of your method.  For example, in a Bayesian talk, it is almost useless to put up a bunch of Gibbs sampling full conditionals in a slide.  Do you really expect people to grok all those in the 30-60 seconds you're giving them?  That's what the paper is for.  (The exception, of course, is if your method is a new kind of sampler.)   
