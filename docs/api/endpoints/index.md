 # API endpoints

You have different data points to request from different API endpoints. The currently available data endpoints are:

- dblist
- insights
- rawnumbers

They are all set up as `.php` files, so to request, for example, the `dblist` API endpoint, you will need to rmake a request to `dblist.php`. The names provided in the titles are all the same as their endpoint file.

Every database endpoint has a similar 2-part structure. first, a code which indicates the success or failure of the request, using the same codes as the `http` protocol, and then, the data requested, if any. In case of a failed request, the API endpoint will only return a status code in `JSON`.

## dblist

The `dblist` endpoint allows you to see a list of the databases  available for data requesting. you will only need to provide authentication to request data to this API endpoint.

## insights

The `insights` API endpoint will provide you with the data seen on the `dataGlance` frontend page, but in a parseable `JSON` response format. To request data from this endpoint, you will need to send in:

- an API authentication token through `apikey`
- the database you want to query with a `database` UTM.

## rawnumbers

The `rawnumbers` endpoint will return the data seen on the web frontend, the aggregated count data, for the database that you request it to, in a parseable JSON format. To request data from this endpoint, you will need to send in:

- an API authentication token through `apikey`
- the database you want to query with a `database` UTM.

See the next page for reference examples.
