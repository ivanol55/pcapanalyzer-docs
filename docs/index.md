# PCAPAnalyzer project documentation

Welcome! This is the site where you'll find reference documentation for all things [PCAPAnalyzer](https://ivanol55.github.io/pcapanalyzer/), from frontend usage, to backend management, to API interaction.

## Documentation structure
- **getting started** - your starting point 
	- **prerequisites** - what you need to setup first
	- **installation** - let's set you up
		- **main server** - The base install
		- **agent** - gather data from other sources
	- **post-install** - what you should know
- **frontend** - Where you'll find documentation about UI interaction and features.
	- **login** - web authentication
	- **homepage** - a quick summary
	- **packetStream** - data filtering
	- **dataGlance** - quick, usually needed info
	- **queryRunner** - roll your own SQL
	- **dbCreator** - analyze your own pcaps
	- **database picker** - manage database usage
	- **About** - manage internal tokens
		- **User management** - manage webUI users
		- **API management** - manage API tokens
- **backend**
	- **.my.cnf** - application information
	- **packetStream** - constant data gathering
	- **PCAPAnalyzer IDS** - get attack warnings by mail
	- **analysisGenerator** - generate custom database reports
- **API**
	- **authentication** - allowing requests
	- **endpoints** - what can you do?
		- **dblist** - listing databases
		- **rawnumbers** - quick data for dashboards
		- **insights** - dataGlance in JSON format
	- **reference** - Quick query and answer manuals
