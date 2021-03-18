# What makes a good story? 

For my final project, I'd like to explore the age old question from the perspective of a data scientist - what makes a story good? 

Stories have been around since humans have been around, passed down from generation to generation, told around the campfire, theaters, movie screens, books - storytelling is what makes us human, what makes us connect with one another in our shared humanity. Stories are how we interact with each other, how we inherit legacies. And they are important for that reason alone. 

But they're also a powerful tool for organizing, for persuading. Organizers have known this forever, but the story we tell of a better world is how we attract people to the cause - get them to volunteer, knock doors, and donate. And digital organizers, especially, are tasked with connecting those on the ground with the larger mission and vision - a better world is possible, and we can build it. 

My love for stories is part of why I wanted to take this class, but I also wanted to explore something more - what makes a good story? It's not a new question - people have been asking it since stories themselves were created. Is it characters? Structure? Plot? Language? The right answer is, of course, some combination of all of those. And it's not just an existential question, either. If we can figure out what makes a good story, organizers would be able to use these arcs and these indicators to tell better stories and be able to get more people on board for all of the issues affecting our world right now - climate change, police brutality, and more. 

Since I started exploring this concept, I started consuming so much content on what exactly makes a good story. One of the books I picked up (through my screenwriting class last semester) was Syd Field's seminal work <i>Screenplay</i>. In it, Fields talks about the three act structure - the narrative arc of story, and how all good stories fit into that. 

So I was curious - does that hold up? And is there more that we can pull out, using data, that tells us what good stories look like? 

# Data and Output

For my dataset, I'm going to need to walk through a couple of different steps. Because this question is so broad, I want to make sure to really hone in on a very finite amount of data to make sure to not get lost in the question I'm asking. First, I want to focus on movies for now. Part of this is because the data for this is easier to find, and part of it is because screenplays are built around visual language more than they are text - which translates better, I think, to digital organizing in the real world. Second, I'll focus on two different indicators for what makes movies "good," by looking at a list of 2019 Oscar winners vs what was top on Rotten Tomatoes. 

Then, I'll put those names into [this website](https://imsdb.com/), and scrape the full script of that movie using a webscraping package like Beautiful Soup. This will be my main source of data, and I'll have to pull in other things like lists of common words, etc (which are easily found through a quick google search) so that I'm only focusing on unique words. I'll then use machine learning tools and the tool Voyant to look for patterns in the data that point to trends, but also look for patterns in the narrative structure of movies that work for viewers. 

If I have time, I'd like to add a section of looking at the narrative structure of certain campaigns (BLM, for example), but that's harder to find data for, and would only be if I had time and could easily replicate the work I've done for the previous part. 

Once I'm done, I'll present it in a Shorthand presentation. 

# Outline

My outline looks very similar to the way this write up is structured:

1) Why are stories important?
2) How does this translate to the real world/organizing? 
3) What makes a good story? (Lit review)
4) Overview of data 
5) Analysis
6) (Optional) Real world example 
7) Conclusion
8) Call to action - important to keep in mind narrative strucutre in organizing, not just language 

# Sketches

These are couple of the different ways that I'm hoping to show what's important to creating good stories and how they might translate to real world organizing.

### Story Format

![First](Paper.telling_stories.9.png)

![Second](Paper.telling_stories.12.png)

### Examples of analysis

![First](Paper.telling_stories.10.png)

![Second](Paper.telling_stories.11.png)

![Third](Paper.telling_stories.13.png)

# Storyboards and Wireframes 

During the user research phase after the first part of this project, I decided to refocus onto Shakespeare plays instead of movie databases. The reasons for this was multi-fold: it was brought up that movies have a lot more to them than the script can identify (acting, props, music, etc) that would make them "good," and plays (especially Shakesperian plays, that usually played very minimal) have a lot less going on outside of the script; Shakespeare plays all follow a very basic 5 act structure that follows the structure of a digital campaign pretty well; and the data for Shakespeare plays tends to be a little easier to find pre-processed. Shakespeare plays also are usually seen as an "everyman" kind of play - he invented new, new ways of doing things, and iambic pentameter is always written about as holding the human heartbeat within its words. Given digital organizing's role as the "heartbeat" so to speak of issue campaigns, the parallel makes sense to draw. 

My question, however, was still a little opaque, and I wasn't entirely sure what really could be gleaned from the data I was able to find. So I ended up making a R Shiny dashboard to start, where my users could play with the data and help me suss out different ways to visualize it or help me find connections I was missing. This is a hard question to ask, and a hard connection to make (between narrative structure of a play and digital organizing), so I needed a little help. You can see the Shiny dashboard below, or find it in an [external window here](https://satvika-neti.shinyapps.io/shakespearedata/). 

<iframe src="https://satvika-neti.shinyapps.io/shakespearedata/" width="100%" height="800px"></iframe>

I also created a [draft preview storyboard on Shorthand](https://shorthand.com/organisations/JSrgFWI7zn/stories/XNpz8VehDO) to share with them, but this ended up changing a lot through the process so it looks different now (and a lot emptier), since I've decided to restructure a good chunk of it. 

<iframe src="https://preview.shorthand.com/ChLXnTktQROe7IBF" width="100%" height="800px"></iframe>

## User Research 

I then sent some friends this google feedback form with a short overview of the project and some questions I had about it, and also got some feedback from classmates during the critique. I picked the people to send it to from a mix of folks with experience in Shakespeare/storytelling but not data, experience in data but not Shakespeare/storytelling, and friends that didn't really have a background in either but just wanted to help me out. This was helpful to get a wide range of viewpoints and feedback from different perspectives. 

<iframe src="https://forms.gle/ewXTSRh8AQhx44WK6" width="100%" height="800px"></iframe>

### Questions  

- Anything in particular stand out to you? About narrative structure, or anything else? 
- What would make these graphs easier to read/understand? 
- How would you want to see stage directions? 
- How might you gauge "good" vs "bad" plays? Or should I forgo this entirely and do genres instead? Or something else? 
- Are you intrigued by these graphs? Are you interested in learning more about a particular piece of them at all that I could try and delve deeper into? 
- A lot of these graphs look the same - does that work for or against the overall story? 
- Do you have a sense of how these graphs/visualizations might be used to gain info about digital organizing structuring? Or is that connection still opaque? 
- What am I missing? 
- Anything else you want to tell me? 

### Feedback

A lot of the feedback was centered around three main ideas: the connection to digital organizing was too opaque, the graphs were both not saying enough and saying too much, and I needed more of a qualitative lens in all of this data. 

Disembodied from the larger story of why they're important, the graphs felt jarring and unnecessary to folks. People couldn't figure out the connection between what they were seeing and what makes a "good" story, or how this translated to digital organizing at all. This helped me realize that I needed to really explicitly drill down on that question a lot more in my storyboards - the connection is obvious to me, but might not be to everyone else. This helped me really drill down on my end user: I was thinking about this person very abstractly, but drilling down on the fact that my end user _is_ a digital organizer helped me slot all the pieces in place in my head. I was telling _them_ how to do their job better, and that was the call to action. From there, I was able to work backward to find out how to structure the rest of this. First, make the current structure of campaigns clear. Second, draw the connection to Shakespeare. Show what works and what doesn't. Then draw the conclusions to how to make your work better. 

The graphs, because they were trying to focus on way too much, were also very busy and hard to interpret. Here, the feedback consisted of focusing on lines over words, lessening the amount of characters focused on (group into protagonists, antagonists, etc), and just generally making the plots a little easier to interpret. What seemed to be the most intriguing to folks was the last one on scene length, because then you can kind of see the different story structures.

The biggest piece of advice and feedback was that the quantitative data just wasn't enough - there needed to be a more qualitative piece to this, whether it was focusing on one or two plays (or one from each genre) and really pulling out the main big scenes, etc, or focusing around the hero's journey story structure and putting this into those archetypes we already know for stories and building from there. 

## Next Steps

I have a _lot_ of ideas for next steps given this info!! I think I will spend some time in going through the dataset more fully and piecing together the protagonists and antagonists, and picking out max 5 plays to analyze. I definitely want to do the one where I pull out specific scenes with the larger overall structure, because I think that would help us glean much insight into how that might map onto digital organizing. I think, again, focusing really hard on which pieces of the digital organizing puzzle I want to solve and then answering that question through the data is going to be the important step, rather than just seeing what the data says first. 

For example, we're generally not sure how long each "act" is supposed to take. Is there info we can pull from the scene length graph to show up how to do that? We're never sure when to introduce in important characters - when does it work for Shakespeare? And when would we do long form content vs short form? Can we map this to soliloquies? 

Overall, the feedback process was super helpful in getting me to really hone down the initial big idea, so I'm excited to delve back in! I'm definitely planning on asking the same people for advice that I did before, and some new ones to get a fresh perspective. 




