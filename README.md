# List of awesome Svelte stores with stars

There are many very useful svelte stores that might make your life easier without you knowing that they exist. Hence this list to surface those gems.
Just reading through the list might also give you some inspiration for solving your problems more elegantly with a store. PR's welcome.

ℹ️ Many stores are just one small file that you can drop in your project without even having to add a dependency.

## Browser Storage

* [@macfja/svelte-persistent-store](https://github.com/MacFJA/svelte-persistent-store) ⭐ 253 | 🐛 15 | 🌐 TypeScript | 📅 2025-06-29
  * Supports different/custom storage providers
* [persistent-svelte-store](https://github.com/omer-g/persistent-svelte-store) ⭐ 86 | 🐛 0 | 🌐 TypeScript | 📅 2022-04-09
  * Built from scratch in TypeScript. Is reactive across tabs or windows using the Broadcast Channel API.
* [babichjacob/svelte-localstorage](https://github.com/babichjacob/svelte-localstorage) ⭐ 48 | 🐛 5 | 🌐 JavaScript | 📅 2026-06-15
  * SSR support
* [@furudean/svelte-persistent-store](https://github.com/furudean/svelte-persistent-store) ⭐ 37 | 🐛 6 | 🌐 JavaScript | 📅 2024-04-01
  * Saves and loads data from `Window.localStorage` or `Window.sessionStorage`.
* [LocalStorage Custom Store](https://svelte.dev/repl/e6c0e3db7d064d43a7e4559b2862e1f7?version=3.48.0)
  * Very simple persisting to localstorage.

## Browser Navigation

* [svelte-store-router](https://github.com/zyxd/svelte-store-router) ⚠️ Archived
  * Router for Svelte that suggests that routing is just another global state and History API changes are just an optional side-effects of this state.
* [query-store](https://github.com/buhrmi/query-store) ⭐ 43 | 🐛 1 | 🌐 JavaScript | 📅 2021-06-18
  * Writable store that syncs with the browser's search param

## Fetching Data

* [svelte-query](https://github.com/SvelteStack/svelte-query) ⭐ 833 | 🐛 36 | 🌐 TypeScript | 📅 2023-08-25
  * Advanced asynchronous state management including caching, auto-refetching etc. TanStack/query fork?
* [svelte-websocket-store](https://github.com/arlac77/svelte-websocket-store) ⭐ 292 | 🐛 12 | 🌐 JavaScript | 📅 2026-08-21
  * Send/receive data from a websocket
* [svelte-asyncable](https://github.com/PaulMaly/svelte-asyncable) ⭐ 170 | 🐛 8 | 🌐 JavaScript | 📅 2026-01-22
  * Tiny, declarative, optimistic, async store
* [@macfja/svelte-invalidable](https://github.com/MacFJA/svelte-invalidable) ⭐ 4 | 🐛 0 | 🌐 TypeScript | 📅 2021-09-25
  * A store that can be requested to update itself
* [Fetch Store](https://svelte.dev/repl/a74f1ed8e3eb4aec82cb743e13443ee4?version=3.48.0)
  * Convenience wrapper for `fetch()`
* [Periodic Fetch Store](https://svelte.dev/repl/b8fa406464d6434fba97902ac78b5e2b?version=3.48.0)

## Undo

* [svelte-previous](https://github.com/bryanmylee/svelte-previous) ⭐ 83 | 🐛 3 | 🌐 TypeScript | 📅 2023-10-17
  * Remember previous values - helpful for transitions or a quick undo stack
* [@macfja/svelte-undoable](https://github.com/macfja/svelte-undoable) ⭐ 47 | 🐛 0 | 🌐 TypeScript | 📅 2021-02-20
  * Memento design pattern (undo/redo) in Svelte
* [storez](https://github.com/plrenaudin/svelte-storez) ⭐ 27 | 🐛 4 | 🌐 JavaScript | 📅 2024-08-30
  * Writable store with old/new value, change history + undo, debounce, localstorage persist

## Time

* [svelte-damped-store](https://github.com/aredridel/svelte-damped-store) ⭐ 6 | 🐛 0 | 🌐 TypeScript | 📅 2026-06-02
  * derived writable store that can suspend updates while user is still interacting
* [@macfja/svelte-expirable](https://github.com/MacFJA/svelte-expirable) ⭐ 5 | 🐛 0 | 🌐 TypeScript | 📅 2021-12-03
  * A store with items that expire
* [@crikey/stores-temporal](https://www.npmjs.com/package/@crikey/stores-temporal)
  * Time based stores such as debounce and throttle

## Upgraded Stores

* [svelte-store2](https://github.com/vkurko/svelte-store2) ⭐ 4 | 🐛 0 | 🌐 JavaScript | 📅 2023-01-16
  * Adds a `get()` function to writable, derived and readable that returns the actual value without subscribing/ubsubscribing in the background like svelte's normal \[get()]
    (<https://svelte.dev/docs#run-time-svelte-store-get>) function.
* [SvelteStore](https://github.com/gitbreaker222/SvelteStore) ⭐ 2 | 🐛 2 | 🌐 JavaScript | 📅 2023-10-17
  * Track state diffs, Inspect current state, Type warnings, Persistent storage, Infinite loop detection, Testable Actions, Audible activity
* [@crikey/stores-promise](https://www.npmjs.com/package/@crikey/stores-promise)
  * Create stores from promises
* [@crikey/stores-strict](https://www.npmjs.com/package/@crikey/stores-strict)
  * Stores using strict inequality checking

## Stores affecting each other

* [svelte-writable-derived](https://github.com/PixievoltNo1/svelte-writable-derived) ⭐ 88 | 🐛 1 | 🌐 JavaScript | 📅 2025-11-15
  * Two-way data-transforming store
* [svelte-keyed](https://github.com/bryanmylee/svelte-keyed) ⭐ 71 | 🐛 2 | 🌐 TypeScript | 📅 2024-04-03
  * Takes a writable object store and a keypath, and returns a writable store whose changes are reflected on the original store. Properties are accessed with dot notation, and arrays can be indexed with bracket notation.
* [Svelte-nStore](https://github.com/lacikawiz/svelte-nStore) ⭐ 13 | 🐛 0 | 🌐 JavaScript | 📅 2020-12-04
  * Adds `get()` without subsription and recalculation of store value that is dependent on other stores values
* [@crikey/stores-selectable](https://www.npmjs.com/package/@crikey/stores-selectable)
  * Extend stores with selection semantics, allowing for the easy creation of type safe sub-stores
* [@crikey/stores-dynamic](https://www.npmjs.com/package/@crikey/stores-dynamic)
  * Derived stores with dynamic dependency support and natural error handling/propagation

## State Machine

* [svelte-fsm](https://github.com/kenkunz/svelte-fsm) ⭐ 296 | 🐛 3 | 🌐 JavaScript | 📅 2023-02-21
  * Only 1kb, very simple, typescript support
  * [9min video introduction](https://www.youtube.com/watch?v=3_D-3HPUdEI)
* [svate](https://github.com/AlexxNB/svate) ⭐ 15 | 🐛 0 | 🌐 JavaScript | 📅 2021-09-29
  * Set of simple state machines for Svelte application (Flag, Flagset..)
* [xstate-svelte](https://xstate.js.org/docs/packages/xstate-svelte/#quick-start)
  * Wrapper around [xstate](https://xstate.js.org/). Xstate: 30kb, complete suit with visual editor and support for charts.
  * [7min video introduction](https://www.youtube.com/watch?v=NIfQsc5XAzU)

## (Im)mutability

* [svelte-restate](https://github.com/endenwer/svelte-restate) ⭐ 20 | 🐛 1 | 🌐 TypeScript | 📅 2022-02-15
  * Immutable store for Svelte with full Typescript support and Redux Devtools integration
* [svelte-readonly](https://github.com/Crisfole/svelte-readonly) ⭐ 10 | 🐛 1 | 🌐 TypeScript | 📅 2021-01-09
  * Very small store that exposes only a readable interface.
* [svelte-mutable-store](https://github.com/feltcoop/svelte-mutable-store)
  * Mutable values when using  the  svelte `immutable` compiler option
* [@crikey/stores-immer](https://www.npmjs.com/package/@crikey/stores-immer)
  * Immutable Svelte compatible stores using [Immer](https://immerjs.github.io/immer/)

## Inspired State Management

* [stores-x](https://github.com/Anyass3/stores-x) ⭐ 6 | 🐛 0 | 🌐 JavaScript | 📅 2022-05-21
  * State management heaviliy inspired by [VueX](https://github.com/vuejs/vuex) ⭐ 28,320 | 🐛 143 | 🌐 JavaScript | 📅 2024-09-25
* [MiniRx](https://spierala.github.io/mini-rx-store/)
  * RxJS Redux Store that works with TypeScript

## CSS

* [svelte-animation-store](https://github.com/joshnuss/svelte-animation-store) ⭐ 24 | 🐛 0 | 🌐 JavaScript | 📅 2021-05-03
  * Based on Svelte's tweened store, that lets you pause, continue, reset, replay, reverse or adjust speed of a tween.
* [sw-yx/everything-store](https://github.com/sw-yx/everything-store) ⭐ 23 | 🐛 5 | 🌐 Svelte | 📅 2022-06-19
  * CSS related stores for: Tailwind Breakpoints, Media Queries, Dark Mode

## Notifications

* [Notification Toast Custom Store](https://svelte.dev/repl/e166b01bc46149a49895c1622d26ce7e?version=3.48.0)
  * Auto-disappearing notifications/toasts

## 3rd-Party interaction

* [@crikey/stores-rxjs](https://www.npmjs.com/package/@crikey/stores-rxjs)
  * Simple conversion functions to allow interop of Svelte style stores with [RxJS](https://rxjs.dev/) style stores
* [timhall/svelte-observable](https://github.com/timhall/svelte-observable) ⭐ 63 | 🐛 13 | 🌐 TypeScript | 📅 2023-01-03
  * Wrapper for Observables (e.g. [RxJS](https://rxjs.dev/))
* [svelte-ethers-store](https://www.npmjs.com/package/svelte-ethers-store)
  * ethers.js to interact with the Ethereum Blockchain

## Browser Extensions

* [svelte-webext-storage-adapter](https://github.com/PixievoltNo1/svelte-webext-storage-adapter) ⭐ 24 | 🐛 4 | 🌐 JavaScript | 📅 2024-08-30
  * Writable stores for Firefox/Chrome extensions using \`chrome.storage
* [svelte-chrome-storage](https://github.com/shaun-wild/svelte-chrome-storage) ⭐ 22 | 🐛 1 | 🌐 TypeScript | 📅 2022-07-17
  * A lightweight abstraction between Svelte stores and Chrome extension storage.

## Others

* [svelte-entity-store](https://github.com/tony-sull/svelte-entity-store) ⭐ 29 | 🐛 4 | 🌐 TypeScript | 📅 2021-05-23
  * Simple, generic solution for storing collections of entity objects.
* [svelte-lens-store](https://github.com/aredridel/svelte-lens-store) ⚠️ Archived
  * Functional lenses over Svelte stores
* [svelte-xactor](https://github.com/wobsoriano/svelte-xactor) ⭐ 1 | 🐛 0 | 🌐 Svelte | 📅 2021-09-17
  * Middleware that allows you to easily convert your xactor actors (actors from [xstate](https://xstate.js.org/)) into a global store
* [Toggle Store](https://svelte.dev/repl/a3cb054398a94698a4cfe4c44f33b923?version=3.48.0)

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-22._
