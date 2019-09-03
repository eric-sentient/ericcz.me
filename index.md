## Generating chord progressions with a recurrent Autoencoder architecture
*August 8, 2019*

This is my first foray into machine learning! I've always been excited by this stuff and found myself wanting to jump in.

Before this, I hadn't had much hands-on experience with ML. I took a few online courses, some of which had example exercises, but the task of writing this thing completely by myself proved to be daunting. This also ended up being pretty difficult; in retrospect I probably would have started myself off with something simpler, as I had to get through the initial mental hurdle of being able to write anything at all.

But enough about me. Lets talk about what I did!

So I watched a lot of people on YouTube try their hand at generating music with neural networks. Most people tried to train their networks to generate melodies specifically, or otherwise didn't distinguish between melodic and harmonic information in their training data (i.e. they fed whole MIDIs with both chords and melody into their network).

I think that there is definitely value teaching a neural network to generate chord progressions. Harmony tends to follow general rules and guidelines. As with music in general, these rules aren't hard-coded: there is no such thing as an objectively good or bad chord progression, but there are lots of qualities that are common to chord progressions that people tend to like, such as 

* cadences
* chord inversions
* voice leading

I want to train my network to learn these qualities, as well as some general intuition as to which chords lead well into which.