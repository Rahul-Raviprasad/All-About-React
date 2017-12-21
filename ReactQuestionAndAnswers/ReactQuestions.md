1. Different ways of defining an Element? (ES2015 class, React.createClass, stateless function — render only)
Ans:
2. What are the differences between state and props?
Ans: Props are shorthand for properties. They are very similar to an argument being passed to a pure javascript function. Props of the component are passed from parent component which invokes component. During component’s life cycle props should not change, consider them as immutable. In React all props can be accessed with "this.props."
```js
import React from 'react';
class Welcome extends React.Component {
  render() {
    return <h1>Hello {this.props.name}</h1>;
  }
}
const element = ;
```

State are used to create dynamic and interactive components in React. State is heart of react component that makes it alive and determines how a component renders & behaves.
```js
// simple state example
import React from 'react';
class Button extends React.Component {
  constructor() {
    super();
    this.state = {
      count: 0,
    };
  }

  updateCount() {
    this.setState((prevState, props) => {
      return { count: prevState.count + 1 }
    });
  }

  render() {
    return (<button
              onClick={() => this.updateCount()}
            >
              Clicked {this.state.count} times
            </button>);
  }
}

export default Button;

```
