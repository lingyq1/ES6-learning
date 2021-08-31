## 1. React JSX
### definition: JSX is used to declare elements in React
```
    const element = <h1 className="foo">Hello, world</h1>;
	ReactDOM.render(element, document.getElementById('root'));
```
## 2. react component
### definition: use component to output messages easily
```
function HelloMessage(props) {
    return <h1>Hello World!</h1>;
}
```
## 3.react parent/child component
### definition: Components can be separated out and easier to write
#### main.js:
```
function App() {
    return (
        <div>
            <nav>
                <h1>Hello a third time!</h1>
                <ul>
                    <li>Thing 1</li>
                </ul>
            </nav>
            <footer />
        </div>
    )
}

export default App
 ```
 #### footer.js
 ```
 function Footer() {
    return (
        <footer>
            <h3>This is my footer element</h3>
        </footer>
    )
}

export default Footer
 ```
## 4. react todo App 
### definition: can create a new todo list app
#### index.js
```
import React from "react"
import ReactDOM from "react-dom"

import App from "./App"

ReactDOM.render(<App />, document.getElementById("root"))
```
#### App.js
```
function App() {
    return (
        <div>
            <input type="checkbox" />
            <p>Placeholder text here</p>   

            <input type="checkbox" />
            <p>Placeholder text here</p>
        </div>
    )
}

export default App
```
#### index.js
```
  <body>
        <div id="root"></div>
        <script src="index.js"></script>
    </body>
```