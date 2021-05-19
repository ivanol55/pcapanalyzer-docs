# Authentication

As to not allow any unauthorized API requests, the PCAPAnalyzer API has implemented an authentication system. With every request, it needs to recieve a valid API key written into the request. If this is not provided, the server will answer with a `403 forbidden` API answer as a status code.

The api key needs to be sent as a GET parameter on the request with the key name `apikey` to be correctly picked up by the system, for example with something like

`curl https://{domain}/api/dblist.php?apikey=APIKEYVALUE`

where `APIKEYVALUE` is an API key you generated on the web frontend.

Once a request is autheticated, it will go on to read your request. Depending on what you want to request, you may need to provide some more data.
