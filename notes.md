[dog]
- Who Am I?
- Help run the Meteor London meetup group
- Run workshops and sometimes talk about meteor for extended periods of time

[members]
- Why it was started - there wasn't one
- Decided the best way to learn a Meteor was to build a thing
- Became Show & Tell
- And then it became the second biggest in the world

[what is?]
- A full stack framework for building your web app
- A stack of NodeJS, MongoDB, Handlebars and websockets
- Focused on allowing you to build data driven realtime apps
- Traditional vs Meteor apps

[first meetup]
- Oli was worried about nobody coming
- Oli built goto
- I built blackboard

[goto]
- Updates positions live as people move
- Idea to app in 1 day! - Less than

[blackboard]
- Canvas based drawing
- Idea to app in minutes

[blackbird]

[what's happening?]
- We didn't write much code at all
- We didn't design a server side API or use any XHR
- The "magic" Meteor did was to put a database in your browser
- ...and keep it in sync with the server side MongoDB
- All we did was tell Meteor there was a collection of things
- Things in the collection of things in the server appeared in the collection of things on the client
- Adding things to the client database appeared in the server database, and in databases of other connected clients!

[Collection code]
- Define a collection
- Add stuff to it
- in reality it is a tiny bit more complicated: you have to subscribe to a publication
- Find stuff from it
- If you've ever used MongoDB before this'll look familiar
- That's all that is happening in goto and blackboard

[Such wow]
- Seeing that happen for the first time is mind blowing
- Other frameworks typically involve a lot of reading before starting
- Itchy fingers
- Meteor have kept things simple enough that you can pick it up really easily

[And then...]
- We kept doing meetups and created a bunch more demos

[movements]
- Similar to goto
- Demonstrate to a client how one could use websockets to push updates to a client
- Most of the code is for periodically adding a position to the collection
- Client just moves the marker and redraws the polyline

[browpie]
- d3!
- UA string harvester

[Foam]
- d3
- SVG
- Data URI
- Web RTC getUserMedia
- DDoS the DB with Data URIs

[how does it know?]
- All these demos are using the Meteor Deps package
- Deps sets up a _reactive context_ that runs a computation once, and re-runs it when its dependencies change
- Pub/Sub
- Live data sets
- Meteor poll & diff / oplog tailing
- Reduces amount of data sent down the wire by sending data diffs only
- The Protocol Meteor are using is called DDP - an open standard they created

[spotify]
- npm integration again
- node-spotify-applescript
- HTML5 <progress> element FTW

[asciify]
- Gravatar
- Experimentation with npm modules
- Reactive templating
- Chat rooms!

[Template code]
- Define a template
- Uses handlebars syntax
- Template re-renders when the data changes
- Behind the scenes they create a reactive context using Meteor Deps
- Reactive DOM is not a new
- Facebook React, Ractive, AngularJS, EmberJS
- Latency compensation

[Routing]
- Meteor applications are single page apps unless you do something about it
- Asciify uses a budget routing mechanism for chat room implementation
- Still 7 lines is fun
- For serious routing you'll want to use IRON ROUTER

[Atmosphere]
- The place where the Meteor packages live
- Meteorite is the tool that you use to install packages in atmosphere
- You'll come to realise many things made for meteor are tragically named after vaguely relevant "spacey" things

[Meteor packages: accounts]



Access control??