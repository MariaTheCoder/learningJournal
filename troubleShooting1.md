
# July 2021

## 25

Today I fixed an issue regarding a function in my JuneProject. The function was to remove an item on a list of connected clients, given than a certain statement is true, and immediately update the list of active clients.   
I managed to solve this issue by using splice on the array of active clients which was available due to a socket.emit from the server side. After using the splice method, I called the update client status update function that I had already coded and tested on multiple occasions.

I tested if my solution works according to my liking and so far it does. 
The next steps of the project is to work on the front-end using front-end framework as well as adding fun features to the websocket project. 

I also looked up the a topic of basic JavaScript that I wanted to brush up on - the terms 'thruthy' and 'falsy'. I heard the terms recently and realised I barely remembered what they meant anymore so I looked it up this morning. 