## The Humble Radio Button
### Estelle Weyl

@estellevw
@standardista
@perfmattersconf
estelle.github.io/flashback

- Examples of Radio Buttons
- Addepar Ember "Radio" Component
  - No input
  - Doesn't render associated label
- Tools are free
  - "Someone has to pay"
  - As devs, tools are free
  - Users pay in downloading scripts, APIs, etc
  - WebPageTest demo
  - Bundlephobia
- HTML
  - HTML actually _is_ free
  - HTML is by default accessible
  - " " fast
- Accessibility
  - Make links with appropriate text
  - Alistair Duggin "disability" tweet
    - > Disability: a mismatch in interaction b/w the features of a person's body and hte features of the environment in which they live
  - We all benefit from the ADA
  - Spectrum of disability/impairment
    - permanent --> temporary --> situational
    - blind --- broken leg --- stillettos
    - quadrepeligic --- reading glasses --- holding a baby
  - ARIA
    - Accessible Rich Internet Applications
    - Adds roles to non-semantic HTML elements
    - Only add ARIA if you cannot use semantic HTML tag
- Radio Button Spec
  - +25 yr old (1994)
  - HTML 2.0
- Reviewing HTML Markup
  - Forms
    - Action can be determined by input attributes
  - Fieldset
    - A lot of people don't use the fieldset because it's ugly
  - Legend
    - Stylable (" ")
  - Submit input type
    - "reset" type can clear radio button values
  - Label
    - Explicit label: `for` attr that matches `id` of its `<input>`
    - Implicit label: wrapped around a nested `<input>`
    - Implicit labels can only wrap around the form control that it's associated with
- Radio Button
  - Represents a boolean choice
  - One-of-many choice field
  - All radio buttons same name
  - `name`/`value` attributes are required
  - Only checked radio input will submit
  - `required` needed in at least 1 of the radios in a group
    - *only the input with that attr will match `[required] {}` CSS selector
  - ARIA `radiogroup`, `radio`
  - Stylable by `-webkit-appearance: none` 
- Replaced Radio Buttons
  - Position native input on top of SVG
  - Style radio button `opacity: 0; position: absolute;`
  - Style label with `input[type="radio"]:checked + label {}`
  - Use `:before/:after` with `-webkit-appearance: none`
- Examples
  - Radio button-only calendar
  - Carousel with radio buttons
    - Image is label
    - Button is radio button
    - JS that changes class to selected label
  - Language selector