## DHTML to CSS Variables
### 

Jr Dev @ Microsoft
keyframe.rs (animations that use as much HTML/CSS as possible, with little JS)

- DHTML
  - Dynamic HTML
  - CSS, JS, CSS-P?
  - Dynamicdrive.com
  - `setInterval` vs `requestAnimationFrame`
- Adding in Frameworks
  - Svelte
  - React
  - jQuery
  - 
- Variables
  - `var`
  - `let`/`const`
- Weird styling
  - CSS expressions (IE7)
  - JSS
- CSS Custom Properties
  - ex `--color-primary: blue`
  - Custom property (`--color-primary`)
  - Value (`blue`)
  - Declar in `:root { --color-primary: blue; }`
  - Specify fallback (`color: var(--color-primary, red);`)
  - Override like other CSS (`h1 { --color-primary: green; }`)
  - Can be used in `calc()` call
  - hammer.js
  - Can set custom properties using JS (`el.style.setProperty('propertyName', propertyVal)`)
  - Codepen examples
- CSS properties vs. JS Setting Properties
  - CSS is really stateful
  - Button example
    - CSS: hover, active, disabled
    - JS: loading, success, failure
  - tympanus.net/codrops
  - DP's personal examples
- Checkbox Example Breakdown
  - No JavaScript
  - Checkboxes: show 0, 1, or more
  - Radios: only 1
- Design inspiraiton/tools
  - origami.design
  - overflow.io
  - invision
- User flows are transitions between UI states due to events
- State Machines
  - Not just for finite state machines
  - WAI-ARIA guidelines for state
    - aria-busy/current/disabled/etc
    - Does not affect essential nature
    - Describes what _can_ happen
  - Data attributes
    - safer than using classnames
  - FSM
    - Loading State, failed, success
    - Transitions
    - `switch`/`case` statements
    - Object mapping
    - DP wrote xstate (xstate.js.org)
- Using FSMs with Animations?
  - Drag-n-drop
  - Applying CSS styles against data-state attributes
  - codepen.io/davidkpiano/pen/vmXErw
- Think in transitions, not just events/states
- links
  - statecharts.github.io
- MAke your code do more
- Easily visualized