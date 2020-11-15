---
layout: project
projectTitle: Jarvis
tag: jarvis
--- 
Yes, the Jarvis from Iron Man. No, it is not original. Yes Jarvis from Iron Man deserves to be envied. 

[Repo, much in development, and MUCH DIRTY CODE, appologies.](https://github.com/kennette21/jarvis)

I want to utilize computer voice interaction to tackle analysis paralyis when trying to decipher what possible plan resonates with my current moode the most. E.g. what to cook, where to eat, or what activities to do on the weekend. 

## How to Collect Activity Candidates
Idealy I would construct a structured list of candidates from a variaty of sources like my Google Map favorites, go-to recipies, regular activities, etc. To start I can just use any nearby places and food on the internet, but I think it would be most effective if it was personal.

## Outstanding Issues
- incorprating proper recursion, and nailing the audio steam window to not pick up too many extra words
- reconsilign wake word detection and STT microphone loops into one. Using the snowboy configuration with Pythons SpeechRecognition library is not working on the Rasbery Pi 4. I could dig into the SpeechRecognition code and submit a fix, but not super motivated.
- the list goes on...


## How to pick it back up?
- Extend the damn reccomendation lists (recipies, restaurants, and ...)
- Incorprate recursion so the user can stop in the middle of the list.
- use mycroft...

# Upate! Nov 15 2020
<iframe 
    width="420" 
    height="315"
    src="https://tbportfolio.imfast.io/portfolio/jarvis/jarv_update.mp4"
    frameborder="0"
    allowfullscreen>
</iframe>

Enter [MYCROFT.AI](https://mycroft.ai/). I found this company last night while doing some research around this project and I would like to make the leap into this direction. I have had some fun playing with the Linux OS and messing with Microphones and ALSA sound, but I am mostly interested in diving into the world of Voice Interaction programs. Mycroft seems to lower the barrier to achieve a relatively robust and sophisticated system which I can extend with my own programs.

I would love to incorperate my rudimentary Phillips Hue helper file into a Mycroft Skill as their are no Philips Hue skills yet.

I would also love to bring in my

# Update! Nov 16 4:30 AM 2020

<iframe 
    width="420" 
    height="315"
    src="https://tbportfolio.imfast.io/portfolio/jarvis/mycroft_working.mp4"
    frameborder="0"
    allowfullscreen>
</iframe>

finally got mycroft to work with respeaker 6 mic array. Helpful setup to install the mic drivers properly on the picroft raspi distro: [praise](https://github.com/adelhult/respeaker-with-picroft)

next steps:
- write a skill for reccomending what to cook/eat based on a list of your favs and allow you to save more favs with your voice.
- hook into the messaging bus to turn on the lights on the respeaker mic array to give some visual feedback to mycroft
