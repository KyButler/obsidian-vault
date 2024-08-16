`store={store}` is the same as `{...{store}}`

Use `CRLF` line endings in files.

What I did:
	- Removed `s1color`, `s2color`, `s3color`, `s4color` from `GraphMgmtSidePanel`'s state. (it's a prop).
	- Added `progressBar` .`s1Color`/`s2Color`/`s3Color`/`s4Color` to redux's Global state
	- Moved all Progress Bar related code to `src/features/progress-bar`
	- Created a global state injector (so we can use Progress Bar with or without global state)
	- Updated all calls to `setState` on color to the global store updated state

We'll probably be able to get rid of the global state, but right now this reduces how much information each child needs to understand / pass down, and we can easily refactor it later.
