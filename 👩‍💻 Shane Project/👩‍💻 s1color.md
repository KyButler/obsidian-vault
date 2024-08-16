
I am trying to reduce prop passing. Let's see where `s1color` goes

`s1color` is a state in App.jsx
default: `'info'`

`slCallback` modifies s1Color based on `message.status` which is the first argument on `slCallback`
`resetMLProgress` modifies s1Color to be `'info'`

`s1color` is passed down to `SideNav`
`s1color` is passed down to `SidePanel`
`s1color` is passed down to `GraphSettings`, `GraphMgmtSidePanel`, `QueryGraphSidePanel`, `DefineCorrelationsSidePanel`, `ShowCorrelationsSidePanel`, `ShowRecommendationSidePanel`, `LitSearchSidePanel`

Out of those, only `GraphMgmtSidePanel` actually uses `s1Color`

`GraphMgmtSidePanel` actually has its own state called `s1Color`. It also pulls s1color off of the props

`s1color` is then passed to `ProgressBar`
`ProgressBar` finally uses it.

What is `s1color`? 
No idea.

It is used by literally only `<ProgressBar`, modified by `slCallback` and `resetMLProgress`.


```
s1pctval: 0,

s2pctval: 0,

s3pctval: 0,

s4pctval: 0,

s1style: '',

s2style: '',

s3style: '',

s4style: '',

status1: '',

status2: '',

status3: '',

status4: '',

s1color: 'info',

s2color: 'info',

s3color: 'info',

s4color: 'info',
```
