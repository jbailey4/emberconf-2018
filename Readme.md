![oh no](https://user-images.githubusercontent.com/914228/37348426-431dcaa6-2691-11e8-9e41-91fb5a5f0e5c.png)

# EmberConf 2018

A collection of links (and notes) that summarize the events of EmberConf 2018. Please submit a PR if you'd like!

Inspired by [**@poteto**](https://github.com/poteto)'s past EmberConf repos. See [2017](https://github.com/poteto/emberconf-2017), [2016](https://github.com/poteto/emberconf-2016), and [2015](https://github.com/poteto/emberconf-2015) for previous years!

## Livestream

> <img alt="" src="https://user-images.githubusercontent.com/914228/34072730-9d2d0bcc-e25a-11e7-9ab5-405ddce05303.gif" width="25"> <img alt="" src="https://user-images.githubusercontent.com/914228/34072749-07a8ab50-e25b-11e7-80ba-d0f6250aad11.png" width="20.5">

- [Official live stream](https://www.youtube.com/watch?v=qfnkDyHVJzs&feature=youtu.be)

## Day 1

### Talks

#### Keynote

_Overall, lots of API improvements, as well as exciting advances in Glimmer.js._

- New filesystem layout
- Optional jQuery
- Codemods
  - `async`/`await` in tests
  - JS module api
  - Computed properties, use es5 getters
  - ES6 classes
    - TypeScript
  - Decorators
- Editor integration
  - [VSCode](https://code.visualstudio.com/docs/languages/typescript)
- Fragment components, empty tagName
- `@tracked` properties, autotracking dependencies
- `@args` syntax in templates
- Experimental
  - Angle bracket syntax
  - Single word component names
  - Named blocks RFC
- [LinkedIn feed in Preact and Glimmer](https://engineering.linkedin.com/blog/2018/03/how-we-built-the-same-app-twice-with-preact-and-glimmerjs)
- https://schedule.emberconf.com - uses rehydration
- https://schedule-wasm.emberconf.com - uses WASM
  - [Glimmer written in Rust](https://github.com/glimmerjs/glimmer-vm/pull/752)

#### Brief interlude from sponsor [Percy.io](https://percy.io) by [Mike Fotinakis](https://twitter.com/mikefotinakis?lang=en)

- [percy-web](https://github.com/percy/percy-web), open source front-end
- [Example of PR integration](https://github.com/percy/percy-web/pull/459)

#### Ambitious for All: Accessibility in Ember by [Melanie Sumner](https://twitter.com/melaniersumner?lang=en)

> Be magnanimous.

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- WAI-ARIA
- WCAG 2.0
- [Color-blind glasses](https://www.google.com/search?q=color+blind+glasses)
- https://include.ai
  - Add alt text to images on the web
- [ember-a11y](https://github.com/ember-a11y)
- Problems
  - Route transitions
  - Modal focus
  - `aria-*` support
  - Clicks
  - Passwords
- Easy wins
  - Use HTML5 elements
  - Link for routing, button for everything else
  - Keyboard nav, arrow keys
  - [Color contrast](https://a11ywins.tumblr.com/post/167324368213/google-chromes-color-contrast-debugger)
  - Image alt text
    - `<img src="elmo.png" alt="" role="presentation" />`
- [`ember-component-attributes`](https://github.com/mmun/ember-component-attributes)
- [\#topic-a11y](https://embercommunity.slack.com/messages/C06MC4CG6/)

#### Everything they didn't tell you about the Ember Community by [Jessica Jordan](https://twitter.com/jjordan_dev)

_Jessica provides an exhaustive overview of the Ember.js ecosystem and Emberista subculture._

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Subculture
  - Emberistas, subset/subculture of JavaScript community
- [Growth in `@angular/cli` download counts](https://npm-stat.com/charts.html?package=%40angular%2Fcli&from=2017-03-01&to=2018-03-13)
- Top addons on [Ember Observer](https://emberobserver.com/lists/top-addons)
- [`ember-rickroll`](https://github.com/nucleartide/ember-rickroll) :troll:
- [Ember Request For Comments (RFC) process](https://github.com/ember-cli/rfcs)
- Quest issues concept
  - Example: [Ember Data](https://github.com/emberjs/data/issues/5292)
- [Ember.js status board](https://www.emberjs.com/statusboard/)
- [Adoption of RFC process by React](https://reactjs.org/blog/2017/12/07/introducing-the-react-rfc-process.html)
- [Ember.js Slack Community](https://embercommunity.slack.com)
  - [`#give-wrjblue-a-beer`](https://embercommunity.slack.com/messages/C05599BQX/)
- [Rapidly growing `ember-cli-typescript` adoption](https://github.com/typed-ember/ember-cli-typescript)
- Email newsletters
  - [Ember Weekly](http://www.emberweekly.com/)
  - [Ember.js Times](https://the-emberjs-times.ongoodbits.com/)
- Offline
  - EmberConf
  - EmberFest
  - EmberCamp
  - Meetups
- [Ember Women Helping Women program](http://emberwomen.com/)
- (not part of talk, related essay) [Melancholy of Subculture Society](https://www.gwern.net/The%20Melancholy%20of%20Subculture%20Society)

#### The Next Generation of Testing by [Tobias Bieniek](https://twitter.com/tobiasbieniek?lang=en)

_Tobias introduces new, elegant testing APIs in Ember._

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- `.andThen()` vs `async`/`await`
- [`ember-native-dom-helpers`](https://github.com/cibernox/ember-native-dom-helpers)
- [`@ember/test-helpers`](https://github.com/emberjs/ember-test-helpers)
- [Grand Testing Unification RFC](https://github.com/rwjblue/rfcs/blob/42/text/0000-grand-testing-unification.md)
- Codemods
  - [`ember-native-dom-helpers-codemod`](https://github.com/simonihmig/ember-native-dom-helpers-codemod)
  - [`ember-qunit-codemod`](https://github.com/rwjblue/ember-qunit-codemod)
  - [`ember-test-helpers-codemod`](https://github.com/simonihmig/ember-test-helpers-codemod)
- Test loading states: `await waitFor('.loading-spinner');`
- [`ember-test-selectors`](https://github.com/simplabs/ember-test-selectors)
- DOM assertion library: [`qunit-dom`](https://github.com/simplabs/qunit-dom)

#### Say More by [Jamie White]()

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links:
  - ...

#### Who Moved My Cheese? Ember's New Filesystem Layout by [Matthew Beale]()

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links:
  - ...

#### Mastering the Art of Forms by [Danielle Adams]()

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links:
  - ...

#### How To Build A Bonfire: On Training and Hiring New Devs by [Taylor Jones]()

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links:
  - ...

#### Living Animation by [Edward Faulkner]()

- Video - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Slides - Not uploaded yet. Submit a [PR](https://github.com/nucleartide/emberconf-2018/pulls) if you find it!
- Links:
  - ...
