
### Added
- Header (Navbar) now has shadow to differentiate it from the rest of the application
### Changed
- GraphUrl dropdown is now in the `GraphMgmtSidePanel`
- Dropdown for the GraphUrl re-written and now using `react-bootstrap`
	- Was: `src/js/components/GraphSettings.jsx`
	- Now: `src/features/graph/GraphSelectionForm.jsx`
- `text-align: center` is no longer at the .app level. This may affect text in unknown parts of the application, but safer to not assume text is centered and have to center it
- Login now hides the page from view
- 61 props given to Sidebar -> 20
### Fixed
- `paraparse.scss` modified _every_ `<label` element's css. I have instead made the `label` modification a class called `paraparse-label` and applied it to every `<label` so there's visually no difference to the labels, but it's now opt-in in case a label does not want to use it
- Sidepanel navigation items can be clicked even when no database is selected
- Sidepanel now full height
### Removed
- First navigation item (`GraphSettings.jsx`) as it's now moved into `GraphMgmtSidePanel`

### Known Issues
- The second Nav Item (Graph Visualization) gets its available graphs from the currently selected graph. Now that the user can select any tab, it's possible to go into this tab without a graph selected, and the dropdown to be empty. It will be fixed by allowing this dropdown to select any of the available graphs at any time in the future.

TODO: The second tab has a dropdown for graph. I feel like we should be able to make the graph fetch go above both tabs and be passed down so both dropdowns are populated . . .

TODO: This sidebar layout is not mobile friendly __at all__, make it mobile friendly!

each thing should have a menu option
something better than 

toggle json should take jsonobjct summarydata or whatever results are coming back from what you're doing

This should do this


40inch
67inch
38inch

Uhaul van is
9.6 long = 106inch
5'1 x 4'1 opening

61inchx
49inch

