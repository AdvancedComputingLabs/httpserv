# Advanced Computing Lab's Golang based http/https server.

## Usage:

### Starting http server:
```
http_server := aclabs_httpserv.NewHttpServ(httpPort, homeDirectoryForWebsite, httpRequestHandler)
```

### Starting https server:
```
https_server := aclabs_httpserv.NewHttpServTLS(httpPort, homeDirectoryForWebsite, httpRequestHandler, certFile, keyFile)
```

### Shutting down server:
```
http_server.SignalStop()
http_server.WaitToFinish()
```

## TODO:
- Test cases.
- Server error callback handler.
- Passing app's logger.
- Add example.
- Add tutorial to create ssl cert.
