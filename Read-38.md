## Conditional Rendering
 - Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.
 - You can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.
 - You may embed any expressions in JSX by wrapping them in curly braces.
 - Another method for conditionally rendering elements inline is to use the JavaScript conditional operator condition ? true : false.
 - In rare cases you might want a component to hide itself even though it was rendered by another component. To do this return null instead of its render output.

## Lists & Keys
- Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity
- Keys used within arrays should be unique among their siblings. However they don’t need to be globally unique. 
- Keys serve as a hint to React but they don’t get passed to your components. If you need the same value in your component, pass it explicitly as a prop with a different name:

## Forms
- In HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().
- You can pass an array into the value attribute, allowing you to select multiple options in a select tag:

## Lifting State
- In React, sharing state is accomplished by moving it up to the closest common ancestor of the components that need it. This is called “lifting state up”
- Usually, the state is first added to the component that needs it for rendering. Then, if other components also need it, you can lift it up to their closest common ancestor. Instead of trying to sync the state between different components, you should rely on the top-down data flow.

## Composition vs Inheritance
- Props and composition give you all the flexibility you need to customize a component’s look and behavior in an explicit and safe way. Remember that components may accept arbitrary props, including primitive values, React elements, or functions

## Thinking in React
- Step 1: Break The UI Into A Component Hierarchy
- Step 2: Build A Static Version in React
- Step 3: Identify The Minimal (but complete) Representation Of UI State
- Step 4: Identify Where Your State Should Live
- Step 5: Add Inverse Data Flow