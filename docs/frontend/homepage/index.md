# Web frontend homepage

THe homepage presents a table with quick information about data on every database on the PCAPAnalyzer data management system. For every logging database, you get information about: 

- The total number of stored packets on the database
- The number of data sources or `agents` logged (only available for `packetstream`)
- The number of external IPs contacted
- How many different MACs have been found on the registry
- How many of the total packets were multicast 
- How many different protocols were registered in the system

This table is generated again every time you reload the homepage. This data is also available through the `API`.
