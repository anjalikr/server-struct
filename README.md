http.ListenAndServe was called to run HTTP servers, which does not allow to customize HTTP server configuration. 
The http package provides a struct named Server that enables  to specify HTTP server configuration.
This struct allows to configure many values, including error logger for the server, maximum duration before timing out read of the request, maximum duration before timing out write of the response, and maximum size of request headers.
The server behavior is customized by creating a Server type object and calling the Server ListenAndServe method.