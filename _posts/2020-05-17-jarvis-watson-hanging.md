---
layout: post
author: tom
tags: jarvis
---

## Discoverd Watson Speech to Text Service
Easy enough to use. things to figure

- [x] How to get from audio in mic to watson.

Things to consider:
watson detect options:
- Speech detector sensitivity
- keywords. how does the api return dems? Lets see.


Lets call it a night, it is 00:27. Not too late but certainly later than is great. Would like to be going to sleep earlier these days to have more productive mornings. To summarize this evenings progress and what is to come:

## This Evening:
# Progress:
1. Doing Speech to Text translation completely on The Raspbery Pi with the 6 mic Array
2. Using IBM Watson S2T
3. Identify Ability to send Keywords to Watson Request

# Ideas:
1. Go? Seems really simple to use th Watson API in go
	- worth a 20 minute delve into go. It was 3 lines

2. Be sure to check up on Watson S2T API docs. Many cool filtration methods.

# Up Next:
1. Consider how to bring the tiered activation word arrays over.
- do you just cat all the arrays together and pass to watson? (i think the limit is 1000)
- Start with simple phrases.
	- _IDEA_ oh could have an add phrase function!! 
- *e.g.* activate words = [LIGHTS_ACTIVATE,NOTES_ACTIVATE,AUDIO_BOOK_ACTIVATE...] 
action words = [ON, BEGIN, ] ** are all action words unique to the category though... this certainly needs it's own time

2. Doing the speech detection LIVE!

3. Using python to get an Audio Stream!
- sending that Audio stream to Porcupine to notice Jarvis word
4. On recognize Jarvis: send the -5s +5s time window from Jarvis to IBM Watson wthe keyword request
- 1st step: save the audio file, end the file (probably slow)
- 2nd step: stream the audio file

5. On API response, do the proper action. Control the lights.

6. Once lights are working, next steps would be:
- recording audio notes -> transcribing (interesting quality analysis..?)
- Food recomendation (hurdle here is content collection. Collect sophisticated list of stuff)
- Video Record start and stop
	- 3D print mount for PI HQ Cam, or Pixel. (BOTH?)


## P.S.
Working on this little pi is kind of fun. I do not know how to use the system as well as the mac and it is a bit lower lever. Using Vim and thi bare bones Thonny Editor. Feels good. Kind of get lost on some tangents trying to improve my process. Also makes me settle for simple productivity like Vim. Would like to get to the point where I am most efficient with tools like this.

