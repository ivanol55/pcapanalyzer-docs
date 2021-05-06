# PCAPAnalyzer Intrusion Detection System

With all the captured data available on the PCAPAnalyzer system, you can use some python scrpting and SQL queries to form an intrusion detection system. This is a feature already implemented in your PCAPAnalyzer backend.

You can access this by creating and editing `probe` files. These are python scripts that, every 30 minutes, will run as a background process on your main server and do whatever task they are programmed to do. In the provided examples you will see a proof of concept of how this can work, which is programmed to, by default, email the `root@localhost` user with a crafted message with the resulting SQL data.

This feature works using the files under **/{your PCAPAnalyzer install folder}/backend/intrusionDetection/**. Here you'll find three things: the `start.py` script, which controls running the service, the `templates` folder with some usage examples for the program, and the `probes` directory. Every script within this last one, by default, will run every 30 minutes.

This intrusion detection system feature can be controlled through a `systemd` service file. You can use `systemctl {command} pcapanalyzer-ids` to start, stop, restart or reload the detection service as you see fit.

To avoid double alerting, and because the data is centralized, this feature is only installed to the machine where you installed your full server install on first setup.
