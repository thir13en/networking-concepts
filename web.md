# The Web


### Building blocks
* `HyperText Markup Language (HTML)`: language for specifying the contents and layout of pages as they are displayed by web browsers.
* `Uniform Resource Locators (URLs)` / `Uniform Resource Identifiers (URIs)`, which identify documents and other resources stored as part of the Web `client-server system architecture`, with standard rules for interaction.
* `HyperText Transfer Protocol – HTTP`: by which browsers and other clients fetch documents and other resources from web servers.

### Deeper into HTTP
* `Request-reply interactions`: `HTTP` is a `request-reply` protocol. The client sends a request message to the server containing the URL of the required resource. The server looks up the path name and, if it exists, sends back the resource's content in a reply message to the client. Otherwise, it sends back an error response such as the familiar `404 Not Found`. `HTTP` defines a small set of operations or methods that can be performed on a resource. The most common are `GET`, to retrieve data from the resource, and `POST`, to provide data to the resource.
* `Content types`: Browsers are not necessarily capable of handling every type of content. When a browser makes a request, it includes a list of the types of content it prefers – for example, in principle it may be able to display images in `GIF` format but not `JPEG` format. The server may be able to take this into account when it returns content to the browser. The server includes the content type in the reply message so that the browser will know how to process it. The strings that denote the type of content are called `MIME types`, and they are standardized in RFC 1521 [Freed and Borenstein 1996]. For example, if the content is of type `text/html` then a browser will interpret the text as HTML and display it; if the content is of type `image/GIF` then the browser will render it as an image in `GIF` format; if the content type is `application/zip` then it is data compressed in `zip` format, and the browser will launch an external helper application to decompress it. The set of actions that a browser will take for a given type of content is configurable, and readers may care to check these settings for their own browsers.
* `One resource per request`: Clients specify one resource per HTTP request. If a web page contains nine images, say, then the browser will issue a total of ten separate requests to obtain the entire contents of the page. Browsers typically make several requests concurrently, to reduce the overall delay to the user. Simple access control: By default, any user with network connectivity to a web server can access any of its published resources. If users wish to restrict access to a resource, then they can configure the server to issue a `challenge` to any client that requests it. The corresponding user then has to prove that they have the right to access the resource, for example, by typing in a password.

### Other important blocks
* `Common Gateway Interface (CGI)`: a program that web servers run to generate content for their clients.

### Websockets
A Websocket uses a long-running `TCP/IP` connection so transferring data `back and forth` does not include the *setup cost* of a `TCP/IP` connection each time, unlike the case of an `Ajax` Request. 
Also with a `websocket` if you want to send an object over the wire, you only pay the payload cost of the object, and not all the standard `HTTP` headers that the `browser` automatically includes in a normal `Ajax` request. Those headers can actually be many times larger than the data itself (for small payloads).  
If you just want to send a counter over the wire, you might be transferring a payload hundreds of times larger than what you would expect due to these extra headers.  