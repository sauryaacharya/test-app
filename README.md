This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `yarn build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify

### `yarn build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify


# Coding Standard and Guidelines

This coding standards and guidelines are aimed for clean, readable and consistent coding among the developers.

## React Guide

React application uses `eslint` for linting and `prettier` for formatting. The linting and formatting rules are defined in `.eslintrc.json` and `.prettierrc`. For VSCode integration, add `eslint` and `prettier` extension.

### Naming Convention

- Always use PascalCase for component's file name as well as component name. e.g. `LoginPanel.js`

  ```jsx
  class LoginPanel extends React.Component {}

  export default LoginPanel;
  ```
  
- Always use camelCase for redux related file name.
  ```
  applicationAction.js, applicationReducer.js
  ```

- Always use camelCase for prop names

  ```jsx
  <UserDetails
    userName="dave"
    firstName="David"
  />
  ```

- Always use camelCase for variable names
  
  ```jsx
  const myVar = 'hello';
  ```

- Always use camelCase for method names

  ```jsx
  const updateSomething = something => {
  };
  ```
  
- Event handler method should follow the below convention
  
  ```
  // The first part indicates the event and the last bit is the context. In this case, the context is Login
  const onClickLogin = () => {
  }
  
  <Button onClick={ this.onClickLogin } label="Login" />
  ```
  
### Alignments
  
- Props and attributes should be in each line if very long (Use formatter to auto correct)
  
  ```jsx
  <Foo
    superLongParam="bar"
    anotherSuperLongParam="baz"
  />
  ```
    
- if props or attributes fit in one line then keep it on the same line
    
  ```jsx
  <Foo bar="bar" />
  ```
    
### Quotes
  
- Always use double quotes ("") for JSX attributes, but single quote for all other JS
  
  ```jsx
  <Foo bar="bar" />
  ```
  
  ```jsx
  <Foo style={{ left: '20px' }} />
  ```
  
### Spacing

- Always have spacing on curly braces if an object literal is a single line
  ```jsx
  { a: 1, b: 2 }
  ```

### Misc

- Always have a trailing commas for multiline
```jsx
{
  a: 1,
  b: 2,
}

[
  'a',
  'b',
]
```
