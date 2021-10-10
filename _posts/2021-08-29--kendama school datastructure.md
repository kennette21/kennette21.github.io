---
Created: 29.08.2021
Tags: #kendama #kendama-school #projects
---

# kendama school datastructure

```
This is the fallback Template.
Create your own template, see help!
```

I have been wanting to create an application where new comers to the world of Kendama can learn how to step through the wonderful activity.

The first priority being absolute beginers, because many people pick up a kendama and all they think to do is Big Cup. Without someone explaining other begginer tasks, or you looking up endless youtube videos, it is difficult to figure out where to go next. So the app should help a new beginers learn to grow into kendama.

The second priority would be to help experienced players keep the sport lively and fresh. The app should help you discover and see tricks that you may not think of on your own.

## The Technical Solution

The project really kicked off after a few conversations wtih a friend from work about how to structure the data for this kind of project. I always wanted to create a visual data graph where each node is a kendama trick and edges connect related tricks. This way, as you improve, you can traverse deeper into the graph and learn more challenging tricks.

[include links to some of the data exploration here]

I soon realized that this is more of a higher level concept and cannt be implimented at the data layer. Kendama tricks are constructed by moving from resting state to resting state with a variety of different transitions. My thinking: it is more efficient to impliment a description of how to construct a vlid kendama trick, rather than enumerating all the tricks in a graph.

From any given state, the application can show you a path to another state, and so on. Some paths will have names (e.g [ken-grip, big cup] -(to)> [ken-grip small cup] -(to)> spike == Around Japan).

Once we have a data structure, we can start building a user experience around this structure

## The User Experience

Here is a figma with the conceptual UI progression laid out

### Fun Extras

I also used this project as a way to learn building animations with SVGs and CSS Transitions. I wanted to create little transitions for major kendama tricks so when you land on one of those nodes, you will get a fancy little animation as a reward/easteregg :)

For now I only have one transition and it will probably just function as a loading screen.

[Show transition here]

## Technical learnings

-   CSS Grid
-   SVG animation transitions
-   (?) however I store this data structure.
