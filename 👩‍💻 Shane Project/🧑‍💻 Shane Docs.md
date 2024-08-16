- Everything starts at App
- App.jsx (via props) -> SideNav -> SidePanel -> Controls working space (right of SidePanel)
	- All workers / helpers function by calling _something_ in JSX

What I could do:
- Change Props to Context so we don't have to pass them all around

Few other things:
- Logins are goofy
	- JSON file that I read that tracks what graphs belong to which logins
	- [ ] Should be in Relational Database
	- It's either has or does not have access to graph
	- Eventually I want queries against the graph but not modify (roles kinda)
- Login by Postgres database
	- admin@cerescan.com / 3dbrainscan
- Stuff needs to be cleaned up
- Almost everything is ran out of (graph management side panel)
	- Graph management side panel is gross
	- Bunch of functions that probably don't do anything
	- Shane had plans but did not go through with most
	- showRecommendPatient should probably go

- Main Functionality
	- Populate graph
	- query graph
	- create a machine learning endpoint
- Side functionality (used to have)
	- Correlation Engine
	- Query a cohort of patients (set filters on a patient)
	- Could select which vertice or edge you wanted to run statistics against
	- See where correlations exist within the graph

__Get rid of props__

ENV_VARIABLES: