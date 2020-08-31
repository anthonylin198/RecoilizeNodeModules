<meta name='keywords' content='Recoil, Recoil.js, Recoil Dev Tool, Recoilize, Chrome Dev Tool, Recoil Chrome'>

<p align='center'>
<img src='./src/extension/build/assets/cover-photo-logo-recoilize.jpg' width=100%>
</p>

# [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/oslabs-beta/Recoilize/blob/staging/LICENSE) [![npm version](https://img.shields.io/npm/v/recoilize)](https://www.npmjs.com/package/recoilize) ![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

<p>
Recoilize is a Chrome Dev Tool meant for debugging applications built with the new Recoil.js state management library!
</p>
<p>
Get Recoilize on the <a href='https://chrome.google.com/webstore/detail/recoilize/jhfmmdhbinleghabnblahfjfalfgidik'>Chrome Store!</a>
</p>

<h1 align='center'>
State Debugger for Recoil (Still in Beta)
</h1>

<h2 align='center'>Shows the difference in atoms and selectors from the previous render</h2>
<h1 align='center'> 
<img src='./src/extension/build/assets/state-diff.gif' width=600 />
</h1>

<!-- <h2 align='center'>View your atoms and selectors in a collapsible tree</h2>
<h1 align='center'>
<img src='./src/extension/build/assets/state-tree.gif' width=600 />
</h1>

<h2 align='center'>Visualize all your atom and selector values in a graph</h2>
<h1 align='center'>
<img src='./src/extension/build/assets/state-graph.gif' width=600 />
</h1>

<h2 align='center'>Display how all your atoms and selectors relate to each other</h2>
<h1 align='center'>
<img src='./src/extension/build/assets/atom-network.gif' width=600 />
</h1>

<h2 align='center'>See which of your React components are subscribed to certain atoms and selectors</h2>
<h1 align='center'>
<img src='./src/extension/build/assets/component-graph.gif' width=600 />
</h1> -->

<h1 align='center'>
Installation
</h1>

#### Install Recoilize Module

```js
npm install recoilize
```

### ** IMPORTANT **

#### Import RecoilizeDebugger from the Recoilize module

```js
import RecoilizeDebugger from "recoilize";
```

#### Recoilize requires you to create a variable that grabs the HTML element where you inject your React application

```js
const root = document.getElementById("root");
```

#### You must import all Atoms and Selectors and pass them into the Recoilize component as shown above

```js
import * as nodes from "./store";

<RecoilizeDebugger nodes={nodes} root={root} />;
```

#### Example:

```js
import RecoilizeDebugger from "recoilize";
import RecoilRoot from "recoil";
import * as nodes from "./store";

const root = document.getElementById("root");

ReactDOM.render(
  <RecoilRoot>
    <RecoilizeDebugger nodes={nodes} root={root} />
    <App />
  </RecoilRoot>,
  root
);
```

#### Open your application on the Chrome Browser and start debugging with Recoilize!

##### (Only supported with React applications using Recoil as state management)

<h2 align='center'> 
We will continue updating Recoilize alongside Recoil's updates!
</h2>

<h1>
 Contributors
</h1>

<h4>Bren Yamaguchi <a href='https://github.com/brenyama' target="_blank">@github </a><a  href='https://www.linkedin.com/in/brenyamaguchi/' target="_blank">@linkedin</a></h4>

<h4>Saejin Kang <a  href='https://github.com/skang1004' target="_blank">@github </a><a  href='https://www.linkedin.com/in/saejinkang1004' target="_blank">@linkedin</a></h4>

<h4>Jonathan Escamila <a  href='https://github.com/jonescamilla' target="_blank">@github </a><a  href='https://www.linkedin.com/in/jon-escamilla/' target="_blank">@linkedin</a> </h4>

<h4>Sean Smith <a  href='https://github.com/SmithSean17' target="_blank">@github </a><a  href='https://www.linkedin.com/in/sean-smith17' target="_blank">@linkedin</a> </h4>
