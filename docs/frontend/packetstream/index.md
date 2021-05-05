# PCAPAnalyzer PacketStream

The PacketStream tab allows you to look at every network packet that is logged on the database. For every packet registered on the system you can see: 

- a UTC timestamp
- the machine ID that provided the data **[!] only available on the `packetstream` database**
- Source MAC address
- Destination MAC address
- Source IP address
- Destination IP address
- Protocol used
- Source port
- Destination port
- packet content info

This data is reverse indexed and ordered by entry id, so retrieval is as fast as possible.

Then, on top of this table, you see a filter set form. In this form, you can input a value for any of the columns stated as a filter. You can use as many filters as you need, but keep in mind they work in an **AND** basis: a packet has to fit all of your filter criteria to appear on the table. Once all of your filters are set, you will need to click **apply filters** to apply them.

If you want to reset all your set filters, you can use the **reset filters** button.
