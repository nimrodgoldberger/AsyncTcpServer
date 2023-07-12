# AsyncTcpServer
Http TCP-IP Non-Blocking Sockets Server in C++ using winsock, with support for large number of connections at the same time.

Supports the following http requests: OPTIONS, GET, HEAD, POST, PUT, DELETE, TRACE.
* GET: Supports Query String in the lang parameter which if it is present and edit he it returns the page in Hebrew, if edited en then returns the page in English and if edited fr then returns the page in French (provided versions in these languages exist for the requested page).
* POST: Assume that these requests will contain strings. The server will display these strings in its console.
* With Text/html support.
* Without using multi-threading.
* If a request is 'stuck' and more than two minutes have passed since the last byte arrived, the connection must be 	closed.
