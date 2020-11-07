# Read: 13 - Update/Delete

### Client/server architecture

- At it's most basic, the web uses a client/server architecture that can be summarized as follows. a client (usually a web browser) sends a request to a server (most of the time a web server like Apache, Nginx, IIS, Tomcat, etc.), using the HTTP protocol. The server answers the request using the same protocol.

![client/server](/images/client-server.png)

### Client Side

- The `action` attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page.

`<form action="https://example.com">`

`<form action="/somewhere_else">`

- The `method` attribute defines how data is sent. The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method.

- Get method - used by the browser to ask the server to send back a given resource.

- method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request.

### Viewig HTTP requests

- HTTp requests are never displayed to the user. To check:

1.Open the developer tools.
2.Select "Network"
3.Select "All"
4.Select "foo.com" in the "Name" tab
5.elect "Headers"

# Be paranoid: Never trust your users