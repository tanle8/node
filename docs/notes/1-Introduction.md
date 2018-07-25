# Introduction

## Why Node.js

Let's start by taking a look at why `Node.js` is one of the fastest growing web platforms out there.

Node.js provides you with the following benefits:

- Develop faster due to the vast number of modules and reusable code from npm
- Make fewer mistakes and be more productive (One language across the stack)
- Delight your user with fast response time (YMMV)
- Reduce team size and communication overhead (full stack JavaScript)
- Reduce dependency on other teams (e.g., backend API teams)
- Ability to re-use code on the browser and server

### Node.js Features

Node.js has some distinct features. Here are some examples of those features:

- Non-blocking I/O: performant
- Fast JS engine: browser arms race (Google Chrome V8 and Microsoft Chakra)
- Expressive and interpreted language: don't waste time on setup
- Solid and improving language standard (ECMAScript)
- Built in package manager with a humongous number of packages (npm)

### Node Downsides

Node isn't always the best design choice. Like most things in life, Node.js has some downsides. Node might not be a good fit because of the following reasons:

- Memory leaks in long running processes with Node are worse than in short running browser environments such as browser JavaScript
- The event loop makes asynchronous error handling more difficult than synchronous error handling
- No benefit for CPU-bound tasks
- Need to think about scalability early on to develop stateless scalable distributed systems
- No built-in typing (but possible with TypeScript)

Note: The Event loop is the core of Node.js and it's a genius idea. However, don't use Node.js for blocking, CPU-intensive tasks. Node.js will not give you a performance boost for stuff like that. Node.js is best suited for I/O stuff (like web servers).

## Node in Modern Web Development

Modern web development consists of building front-end applications which connect to servers to submit or get data. The front-end applications use the single-page application approach a.k.a. thick client. In it, a client app communicates with a server backend via JSON, GraphQL, Protocol Buffers, XML, text, binary streams or other formats which are transmitted via HTTP.

The server communicates with databases and other services. In other words, the server acts as a middleman between the front-end application and the database or other services. The server does things which the front-end app cannot do: authentication, data validation, working with a file system, encryption, etc.

The way the server communicates with the front-end app client and vice versa is by having various endpoints distinguished by URLs in accordance to the HTTP standard. Each request for data has URL, headers, and body (a.k.a. payload).

Implementation of servers is where Node comes in. Node is used to implement the backend servers which are often JSON RESTful APIs (but they could be of other formats as well). Node is on par with stacks such as Apache web server+PHP or Tomcat+Java.

Node is not a framework by itself because it offers very low level mechanisms. The Express framework is often used to implement web applications and RESTful API servers in Node.

Adhering to SPA and REST API architectures for your web applications will give you the flexibility to leverage your servers for other clients (mobile, IoT, public) and will allow you to change front-end clients easily because of the loose coupling provided by the API.

