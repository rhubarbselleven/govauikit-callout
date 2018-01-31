# govaukit-callout

Sample react app using `@govau/callout@next`

To recreate (most vanilla way possible):

```sh
npx create-react-app govauikit-callout
cd govauikit-callout/
yarn add @gov.au/callout@next
yarn start
```

Edit `src/App.js` to the following:


```
import React, { Component } from 'react';

import AUcallout from '@gov.au/callout';

import logo from './logo.svg';
import './App.css';

class App extends Component {
  render() {
    return (
      <div className="App">
        <header className="App-header">
          <img src={logo} className="App-logo" alt="logo" />
          <h1 className="App-title">Welcome to React</h1>
        </header>
        <p className="App-intro">
          To get started, edit <code>src/App.js</code> and save to reload.
        </p>

          <AUcallout description="This is a callout."/>

      </div>
    );
  }
}

export default App;
```

Error message created:

```
Element type is invalid: expected a string (for built-in components) or a class/function (for composite components) but got: undefined. You likely forgot to export your component from the file it's defined in, or you might have mixed up default and named imports.
```
