# UI

UI is a custom web component that wraps any game and provides base UI controls for the game.

The game can communicate with the ui through events. It has the option to either subscribe to events emitted by the ui or emit its built-in events.

::: details An example of how the interaction with the ui functions
``` typescript
  this.ui.onSpinClick(() => {
    // do my game stuff here
  });

  this.ui.setBalance(200);
  this.ui.spinClick();
```
:::

## UI Integration Steps
1. Install the UI
2. Provide the configuration
3. Subscribe for events
4. Trigger events based on game logic and UI specifications


### Installation via Package Manager

1. Open your project's package.json file.
2. Find the dependencies section.
3. Add a new entry for the ui version as a dependency. It should look like this:
``` json
  "dependencies": {
    "@company/ui": "git+https://git@gitlab.UI_REPOSITORY/ui.git#main"
    // ... other dependecies
  }
```
4. Use npm, to install the UI version along with its dependencies. Open your terminal and navigate to the project directory.
Run the command:
``` bash
  npm install
```

Execute these commands to retrieve the UI from the GitLab repository and integrate it into your project's dependencies

### UI Setup

> The UI is a custom element, which functions like a regular DOM node but with additional features. Therefore, you can access it using the standard DOM query selector method.


#### HTML Setup
Wrap your game DOM elements in a UI custom element:

``` html
<body>
    <ui id="ui">
      // Put here your game DOM elements. For example:
      <div id="game">
        <canvas></canvas>
      </div>
    </ui>
</body>
```

#### Javascript/Typescript Setup
Include the UI's source code in your application:

``` javascript
  require('@company/ui') 
```


#### UI Instance Access
The UI is a custom element, which functions like a regular DOM node but with additional features. Therefore, you can access it using the standard DOM query selector method:

``` javascript
const ui = document.querySelector('#ui');
```
