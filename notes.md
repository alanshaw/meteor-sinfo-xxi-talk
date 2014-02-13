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
- A client AND server side framework for building your web app
- A stack of NodeJS, MongoDB, Handlebars and websockets
- Focused on allowing you to build data driven realtime apps
- Traditional vs Meteor apps

[how we built our first apps]
- Worried about nobody coming
- Oli built goto
- I built blackboard

[goto]

[blackboard]

[what's happening?]
- We didn't write much code at all
- We didn't design a server side API or use any XHR
- Meteor put a database in your browser
- And keeps it in sync with the server side MongoDB
- All we did was tell Meteor there was a collection of things
- Things in the collection appeared in the client database
- Adding things to the client database appeared in the server database, and in databases of other connected clients! OMG!

[Collection code]
- Define a collection
- Add stuff to it
- Find stuff from it

[Such wow]
- Seeing that happen for the first time is mind blowing
- Other frameworks typically involve a lot of reading before starting
- Itchy fingers
- Meteor have kept things simple enough that you can pick it up really easily

[movements]

[asciify]

[how does it know?]
- Pub/sub
- Live data sets
- Meteor poll & diff / oplog tailing
- Reduces amount of data sent down the wire by sending data diffs only
- The Protocol Meteor are using is called DDP - an open standard they created
