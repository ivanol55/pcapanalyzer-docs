# Server credentials

On the backend folder of your PCAPAnalyzer server install you'll see a file called `.my.cnf`. This file is the central authentication credential and variable source for the server install. Inside your file you will find five categories:

- `client`
- `paths`
- `interfaces`
- `queryrunner`
- `credchecking`

## client

The `client` category tag stores declarations for data about the current client system:

- `host`: an IP address pointing to the IP address where your PostgreSQL PCAPAnalyzer instance is hosted on.
- `user`: the name that the system uses to login to the database for general tasks.
- `password`: the password for the general tasks user.
- `database`: the name of the main database, generally `packetstream`.
- `machineid`: a unique system name for the packetstream capture system to insert into its data.

## paths

The `path` category tag stores the absolute system paths for needed directories:

- `basedir`: the absolute base filesystem directory where your PCAPAnalyzer install is located.

## interfaces

The `interfaces` category tag stores data about the listening system for `packetstream`:

- `interface`: the interface that the `packetstream` system listens on. it can be set to `any`, but it can only have one value.

## queryrunner

The `queryrunner` category tag stores information needed for the `queryrunner` side of the web frontend:

- `selectuser`: The username on the `PostgreSQL` system that is **only** allowed to select data, from all of the PCAPAnalyzer databases.
- `selectpassword`: the password configured on install for the user mentioned above.

## credchecking

The `credchecking` category tag stores information needed to connect to the database that stores frontend accounts and API keys:

- `user`: the `PostgreSQL` install system user that can work with the `pcapanalyzer_creds` database to check and manage users and API keys.
- `password`: The `PostgreSQL` password for the user mentioned above.
- `host`: the database host where the PCAPAnalyzer install was made. Generally the same as the one on the `client` category tag.
- `database`: the name of the database where the system will look for credentials, generally `pcapanalyzer_creds`.
