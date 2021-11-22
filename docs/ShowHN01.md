# Show HN: An open-source fully-featured scalable chat app

In any form of collaborative application, chat will usually worm its way in somewhere. While a simple chat example is functional, it's usually not enough for production-level applications. You start to need to consider:

* How to store & retrieve messages
* Authentication, authorization, and roles
* How to handle complex messages
* User information and presence

But, if you're making a chat app, you're not necessarily interested in making different kinds of guarantees about connectivity or message delivery, and you're not interested in making different levels of communication protocols or designing and managing a database. 

You're just interested in making a chat app. 

Here at Ably, we're writing an open-source demo chat app with a complete feature set. (We've called it the fully featured scalable chat app (or FFS for short). It's currently in progress, and as we go, we're putting the code in Github and writing a series of posts about it. Anyone can use it for chat integration in their apps. 
 
We'll be using Ably in combination with other services to store, manipulate and share data ([here's a diagram of the stack](https://ik.imagekit.io/ably/ghost/prod/2021/11/fully-scalable-chat-app-architecture.png?tr=w-1520)):

* Web Application that is hosted in Azure Static Web Apps (React)
* "BFF" API built to run in Azure Functions (Node.js)
* CosmosDB database to store metadata (user accounts, chat channel metadata)
* Ably Realtime account to send and receive chat messages
* Archive API to receive events from Ably Reactor and maintain a chat history
* Storage bucket to store the Chat Archive.

However, this is just our current plan. We want our work to be as beneficial for anyone making a chat app as possible. If you have any features of chat applications you'd like us to investigate, requests for us to look at different technologies, or simply want to let us know what you think, please let us know!

## Resources

* [Introductory blog post](https://ably.com/blog/fully-featured-scalable-chat-app)
* [Github repo](https://github.com/ably-labs/fully-featured-scalable-chat-app)
* [Ably](https://www.ably.com)
* [Ably on Twitter](https://twitter.com/ablyrealtime)
* [email us](mailto:devrel@ably.com)
