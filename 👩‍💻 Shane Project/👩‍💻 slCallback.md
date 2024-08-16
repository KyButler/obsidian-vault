

`slCallback` is really silly.

`slCallback` is called when `App.jsx` Updates `graphURL` state.

`graphURL` state is _only_ edited by `this.resetAll` and `setGraphURL`

`setGraphURL` -> `<SideNav` -> both `<SidePanel`'s -> `GraphSettings`/`GraphMgmtSidePanel`... but only used in `GraphSettings`



so let's first get `s1Callback` to not pass down this. . .?