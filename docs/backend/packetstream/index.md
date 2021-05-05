# Packetstream data capture system

To capture data into the `packetstream` database for analysis, PCAPAnalyzer uses the `packetstream` packend system. This is a python tool that will capture network data with wireshark in a constant loop as a background service, and will continually move it to a folder system for treatment.

The streamlined data treatment workflow is as follows:

1. `Wireshark` reads all closed `.pcap` files into a text file in a readable format, stripping away the binary format of the original `.pcap` file
2. `Python3` reads this csv file and does some data changes:
	- merges the empty port columns 
	- inserts a column with the value of the local `machineid` credential entry
	- transforms dates from linux `epoch` time into UTC ISO date format
	- moves it to the last step

3. In this last script, the data is copied into `PostgreSQL` with the `psycopg2` connector for Python.

This process is the same either if you are in the server where the frontend is installed, or in a system with the agent, with the difference that there has been some minor modifications in how the last step copies the data from the agents to the `packetstream` database.

You can control this data gathering with `systemd`, thanks to the service file that was installed when you set up the environment. Just use `systemctl {command} packetstream`.
