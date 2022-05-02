# 2022

## February 7th

After consideration I have decided to restructure my future learning process with the hopes that the changes will increase my progress and help realize my dream of landing a job as a software developer.
For this reason, I decided to drop out of the GraphDBi project that I joined with two far more experienced developers to take back those 8 hours weekly to dive deeper and more intensely into understanding the very basics.
Perhaps I can join the project again at a later point once my skills and knowledge has developed.

## February 9th and 10th

These days I've been doing recaps on the very basics of JavaScript by going through the seocond course material on FreeCodeCamp called "Javascript algorithms and data structure"

## March 11th

I have come very far with one of my personal projects which has the goal to imitate a bookkeeping software and some of its functionalities. In essense, it is a CRUD application with additional features such as ability to sort values of data in a grid in decending or ascending order as well as automatic change of credit/debit values depending on which accounts are used when creating an account.

# 2022

## May 1st

During the last couple of weeks I have been going through the introducting part of the Odin Project which provides learning material as to how the internet works, differences between a webpage, website, web server and a search engine is, how the world wide web came to be etc. However, I do not stick to just the provided learning material and find additional sources on information to get more details on the topics.

## May 2nd

### What is a Network?

A network is a system of interconnected things or people

### What is the internet?

The internet is a network of computers (or servers) all around the world. The servers are connected to one another via cables that are underground and traveling underweater between countries and continents. Each server is connected to these cables and thereby connected to each other.

### What is an IP address?

IP in IP address stands for internet protocol address and is a series of numbers that identifies any device on the network, e.g. a computer, a server, printer, smartphone etc. IP-addresses are also used to identify websites and webpages.

### What is a router?

A router is tiny computer that connects multiple devices within the same network. The router's main job is to make sure that a message is sent to the right receiver.

### What is an ISP?

ISP is short for internet service provider. It is a company that provides internet access to client.

### What are packets and how are they used to transfer data?

When data is sent over the internet, they are delievered in small chunks of data from server to client. This is practical for multiple reasons. One reason being that in case of a chunk being damanged or dropped, it is easier to replace rather than one big delievery. Other than that, for traffic purposes: With multiple chunks it is possible to send a lot of data on different paths between the server and the client. This decreases the delievery time and allows for multiple users to download from the same website at the same time.

### What is a client?

A client is a device connected with access to the internet. A device is used by people like you and I to communicate to a server that we want to access a specific website.

### What is a server?

A server is a computer that is usually running continueously and connected to the internet.

### What is a web page?

A web page is a single html-file being reached by a device via the web. The html file may refer to a javascript file in it's script tag and a css stylesheet in its source tag. A website however consists of multiple web pages.

### What is a web server?

A web server is a piece of software that can be run on a physical server. The software uses HTTP which is built on top of TCP/IP protocols. TCP/IP stands for Transmission Control Protocol/Internet Protocol and HTTP stands for Hypertext Transfer Protocol.

### What is a web browser?

A web browser is a piece of software on a client used to display content of webpages. This includes popular choices such as Safari, Google Chrome, Firefox, Internet Explorer or Microsoft Edge etc.

### What is a search engine?

A search engine is a website used to browse content on multiple webpages of other websites and displays web pages.

### What is a DNS request?

DSN stands for Domain Name System.
When 'www.google.com' is typed into a web broser, the user is requesting the root of the Google search which equals typing in the url 'www.google.com.". Yes, there is an invisible dot there. The IP address of the domain might be configured on the device itself or it could be stored in memory/cache.

1. The browser asks the operating system if it knows the IP address of the requested domain. If they both do not know, where the domain of 'www.google.com' is, the operating system is configured to ask a resolving name server for IP addresses that it does not know.
   The resolving name server is the workforce of the DNS lookup. It is either configured manually or aautomatically within the operating system of the used device.
1. When the operating system requests the IP address of a particular domain, the resolving name server will look into its memory/cache first. If it does not know store this information, it knows where to find the root name servers.
1. If the root name server does not know either, the resolving name server stores all the information it got from the root name server inside of its memory/cache and move on to ask the top level domain name servers (short TLD name servers).
1. The com TLD name servers might not know either, but it knows which authoratative name servers to use with help of the domain's registrar. When a domain is being purchased, the registrar will update the authoratative name servers that use that domain should use. Then the registrar updates the top level domain, the registry, and tell them to update the TLD name server.
   The resolving name server stores all the information it got from the server and move on.
1. The authoratative name servers (short ANS name servers) will then know the IP address for. The resolving name server will store this information in cache and gives a reply to the operating system.
1. The operating system will then give this information to the browser
1. The browser then makes a connection between the requested domain to the IP address received.

### Which broswer are you currently using?

I am currently using Google Chrome.

### In your own words, explain what happens when you run a search on google.com

Imagine that you are using an old fashioned wall mounted telephone without a display or internal memory.
