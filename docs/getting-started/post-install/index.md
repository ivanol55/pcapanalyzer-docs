# Installing the agent
When you already have a full server install, you may want to install the agent on host machines to gather data from them. The install steps for the agent are:

1. `git clone` the [PCAPAnalyzer installer repo](https://github.com/ivanol55/pcapanalyzer)
2. `cd` to the cloned repo on the `pcapanalyzer` folder
3. Navigate to the `install` folder
4. Run the `installer.py` script with `python3 installer.py`
5. when prompted for a confirmation, choose `y` or `Y` to enter the install script
6. When prompted, enter `a` or `A` to perform an agent install. 
7. Input the `postgresql` database manager host IP that has the PCAPAnalyzer database install from your server.
8. input the password that the server install generated for your PCAPAgent user.
9. You will be asked to input a machineid. Choose a unique identifier for the host, like its hostname.
10. input the absolute path where you want to install the agent. The team's recommendation is `/opt/pcapagent/`.
11. From the listed options, provide the system name of the interface you want the network sniffer to listen on. **[!] you can input `any` to listen on all of the system's interfaces, but you can only have one entry.**
12. Enable the data logging with `service packetstream start`.

Once this installation is complete, you will have a functional PCAPAnalyzer install to use.
