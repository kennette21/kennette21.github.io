
---
layout: post
author: tom
tag: culture-blog
---

# event-sourcing-adventures
## Primary goal:
setup the culture blog's data based solely on an event collection in Firebase

### step 1
create events collection in firestore

### step 2
consider what kind of events will be needed:
- publish: when a user publishes a piece
- view: when a user views a piece
...
probably many more, but just these two are fine for now.

__question__: every event will need an event type... I guess i would do this by creating a base event type and then all events extend that type.. hmm another case for typesciprt 

-- note: I should really introduce typescript so i can type these events so they always have the same shape

#### publish 
needs to contain all piece information:
- event_type
- reference/link (content)
- why (250 words max)
- who (author)
- created_at
- category
- emotional_tag ??? (in development) 
- title (maybe)

#### view:
- piece_id
- user_uid

### step 3
send respective events  on create and view

#### 3.1 publish
publish event is trivial, just upate the create function

#### 3.2 view
less trivial because showing a random piece does not work yet. So first step, make random page work with publish events.

plan of attack:
1. get all publish events
2. get all view events of current user
3. filter publish events with piece ids

another trouble: how to get a "piece_id" if i am creating an event, not a piece..? for now i can use the event_id as the id of hte piece because publish event = piece right now... but in the future this should be resolved.

... almost there, current problem is the queries returnd from firebase are objects, not arrays.

...
so it works now, but there is what I would consider some not so good hacking to turn the firebase query response into an array

I think that is all we have time for now! Taaa taaa! This has been a great exercise!
