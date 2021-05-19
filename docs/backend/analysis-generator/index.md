# PCAPAnalyzer Analysus generator

This is the backend code for the dbCreator frontend system. It packages all the necessary tools for you to generate new databases to analyze data on. you will find two folder structures, `script` and `files`

## Script

Under the `script` folder you'll find the python code that runs through the process of generating the new database. It is essentially a compressed version of the `packetstream` data transformation workflow, as in, it reads `.pcap` files, in this case your uploaded ones, into csv files, it transforms them into standard contents, and puts them into a new database.

## files

The `files` folder separates its workflow into two different folders: `pcaps` and `csvs`. on the first one, every time you create a new database, it creates a folder to store all the needed `.pcap` files inside of. Then the script reads them and, when transformed, moves the data into its proper `csvs` subfolder, where the system will read it into the database.
