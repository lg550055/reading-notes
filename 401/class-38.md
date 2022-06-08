# React 2

### Conditional rendering

Use `condition && component`
Or JS ternary operator

To prevent a component from rendering (but not from its lifecycle methods) return `null`

### Lists and Keys

Use `map` to return multiple elements, e.g. `<li>` or to assign a 'key' to each element.

Note: React requires unique keys to keep track for changes.


### Forms

HTML Forms are special components because they have their own state and default functionality.  To better use them in React, make the React state be the single source of truth (e.g. input value={this.state.value}).  To control functionality, use form-handling functions, e.g. onChnage={this.handleChange}.


### Lifting state

Lift state to the closest common ancestor when multiple components reflect the same changing data.

Given that state only flows from parent to child, use a parent function passed to the child to reflect changes made in a child.


### Composition vs Inheritance

> React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.

---

### Bonus: Heroicons
> Beautiful hand-crafted SVG icons

The quickest way to use these icons is to simply copy the source for the icon you need from heroicons.com and inline it directly into your HTML, for example:

<svg class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
  <path
    stroke-linecap="round"
    stroke-linejoin="round"
    d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"
  />
</svg>

Set the color CSS property, either manually or using utility classes like text-gray-500 in a framework like Tailwind CSS.

##### To use heroicons with React
Install @heroicons/react : npm install @heroicons/react

Import each icon as a React component: import { BeakerIcon } from '@heroicons/react/solid'

function MyComponent() {
  return (
    <div>
      <BeakerIcon className="h-5 w-5 text-blue-500"/>
      <p>...</p>
    </div>
  )
}

The 24x24 outline icons can be imported from @heroicons/react/outline, and the 20x20 solid icons can be imported from @heroicons/react/solid.

Icons use an upper camel case naming convention and are always suffixed with the word Icon.

---

### Resources

- [React -Conditional rendering](https://reactjs.org/docs/conditional-rendering.html)
- [React -Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)
- [React -Forms](https://reactjs.org/docs/forms.html)
- [React -Lifting state](https://reactjs.org/docs/lifting-state-up.html)
- [React -Composition vs Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)
- [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)
- [React - Comprehensive Guide](https://ui.dev/react)
- [heroicons](https://heroicons.com/)

---

[Back to table of contents](../README.md)
