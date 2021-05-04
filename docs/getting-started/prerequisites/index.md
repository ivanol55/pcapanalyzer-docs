# Installation prerequisites
Before you can set up a PCAPAnalyzer installation, you need to have a ready environment with the next elements:
## Server install
This is the full server install that sets up the entire environment as front-end and back-end services for data gathering. You need to start with this one.

1. Python3 is installed on your system
2. You're running a system with Debian 10 or greater
3. This system has access to the internet
4. This system has at least 1 gigabyte of ram and a dual-core CPU
5. This system has an active apache2 install, it can be a fresh one.
6. You have administrator credentials to a local or remote PostgreSQL server
7. You have administrator credentials for the machine and you're running the script as root
8. A domain to point this website towards. It can be a local internal name.

## Agent install
If you already have a full server install, you can install the agent on host machines to gather data from them. The prerequisites for the agent are:

1. Python3 is installed on your system
2. You're running a system with Debian 10 or greater
3. This system has access to the internet
4. This system has at least 1 gigabyte of ram and a dual-core CPU
5. You have the agent login credentials given to you during the server install
6. You have administrator credentials for the machine and you're running the script as root

Once this setup is confirmed, you can proceed to installing the server.
