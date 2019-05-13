# HTTP Requests Workshop

We visit websites and use apps, like Facebook, everyday. But, do you know how that information gets to you in the first place? in this section, we are going to get an overview of what happens when you load a website.

## Workshop
From the moment you press the Enter button to when you view a web page, you are communicating with numerous technologies.

A **server** is a special computer that is always on and is always ready to give you what you ask for. They live to serve information.

### Web Server Setup
The five web servers each receive a name (IP address) and a folder with files in it (which represents files on the server hard drive) and some instructions on how to behave. The servers must stand with their hand on their ear, listening and ready for an HTTP request.

A **nameserver** is a special server that  handles requests regarding the location of a domain name's various services.  Nameservers are a fundamental part of the **Domain Name System (DNS)**. They allow using **domains**, such as "google.com", instead of IP addresses.

In order to receive an HTTP request, this is a protocol:

1. Shake hands with whoever is giving the HTTP request.
2. Look at the request and process it according to their rules.
3. Shake hands and give a return HTTP message.
4. Put hand back on ear.

If a server receives an HTTP request not addressed to it, then it will return an error message.

### The Nameserver Setup
The nameserver does the same as the web servers, except the nameserver gets a database of all the different web server’s names (IP addresses) and which domains they are in charge of.

When they get a HTTP request for a domain, they look up in their table and return the IP address.

Protocol is to always shake hands before transferring the message.

### Browser Setup
The browser gets a whiteboard and a marker and some HTTP request slips.

### User Setup
The user gets a marker and is able to interact with the browser UI which is drawn on the whiteboard.

### Exercise
**The user will ask the browser to load `refcode.com/hello.html` by typing in the URL bar.**
* Browser writes a HTTP request for refcode.com and gives it to the Nameserver.
* Nameserver directs the HTTP request to server 167.99.4.63.
* Server 167.99.4.63 can’t find hello.html, so responds with an HTTP 404 code
* Browser draws “404 Not Found” on the page.

**User asks the browser for `refcode.org/hello.html`**
* Browser writes HTTP request and gives it to the Nameserver
* Nameserver finds the domain in the table, and passes the HTTP request to the host in charge.
* The host reads the HTTP request and attaches the file requested.
* Browser receives the file and draws content. When the browser gets to the image, it writes another HTTP request asking for that file.
* Server gives the files, one at a time.
* Browser finishes drawing page, and user may interact with it.

**User asks browser for refcode.org/hallo.html**
* Same process as above, but the server doesn’t have a file with that filename so it returns a 404 message.

## Resources for the Actors
### Nameserver (8.8.8.8)

Domain Name | Server in charge of this domain (host)
----------- | ---------
`refcode.com` | `167.99.4.63`
`google.com` | `172.217.9.46`
`refcode.org` | `198.20.92.45`
`x.com` | `160.153.63.10`
`stackoverflow.com` | `151.101.1.69`

### Hosts
Stand with your hand on your ear at all times and listen for HTTP requests.
* If you get an HTTP request, try to find the file it is asking for in your filesystem.
* If you have the file, send it back with a Code 200 message attached to it.
* If you don’t have the file, send a Code 404 message back.
