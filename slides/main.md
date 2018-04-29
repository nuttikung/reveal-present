# Who am I?
<p>Name : Nat</p>
<p>Education : B.Sc(IT KMITL)</p>
<p>Work : Sharmble Technology</p>

[Sharmble Web](https://sharmble.com)



# Award
![Activator Award](https://preview.ibb.co/iv4gRx/award_act.jpg)



# Award
![All Award](https://preview.ibb.co/kTmBRx/award_all.jpg)



# Award
![Award insur](https://preview.ibb.co/fJzgRx/award_tech.jpg)



# What's about today?
How about technology to develop website?



# MERN

MERN comprised of the JavaScript technologies as below.

-  **Mongo**  [Official Link](https://www.mongodb.com)
-  **Express** [Official Link](https://expressjs.com)
-  **React** [Official Link](https://reactjs.org)
-  **Node** [Official Link](https://nodejs.org/en)



## Mongo
- Database
- NoSQL
- Open-source



## Express
- Web application framework
- Open-source



## React
- JavaScript library for building user interfaces
- Maintained by Facebook, Instagram and etc.
- Virtual DOM



## Node
- Open-source
- Cross-platform JavaScript run-time.



# Let's start!



# Memorable ?
- **HTML**
- **CSS**



# HTML Example
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
<body>
  
</body>
</html>
```

```
<h1>Hello HTML</h1>
```



# CSS Example
```
.hello-world{
  color: palevioletred;
}

<h3 class="hello-world">
  Welcome to CSS.
</h3>
```


## Result 
![css example result](https://image.ibb.co/d9rxGx/CSS_EXAMPLE.png)



# React JS
- **JSX**
- **Component**
- **Virtual DOM**



## Virtual DOM



## JSX
**JSX** is designed as an ECMAScript feature and the similarity to **XML/HTML** is only at the surface



## Component
![component design](http://vitalflux.com/wp-content/uploads/2015/08/reactjs_ui_design_by_components.png)



## Hello World
```
<div id="app"></div>
```
```javascript
class HelloWorld extends React.Component {
  render() {
    return (
      <div>
        <h3>Hello World</h3>
      </div>
    )
  }
}
ReactDOM.render(
  <HelloWorld />,
  document.getElementById('app')
)
```



## Result
![react hello world](https://image.ibb.co/efE4eH/React_Hello_World.png)



## With CSS
```
.hello-world {
  color: palevioletred;
}
```
```javascript
class HelloWorld extends React.Component {
  render() {
    return (
      <div>
        <h3 className="hello-world">Hello World</h3>
      </div>
    )
  }
}
ReactDOM.render(
  <HelloWorld />,
  document.getElementById('app')
)
```



## Result
![react hello world style](https://image.ibb.co/mvbgtc/React_Hello_World_Style.png)



## Props
```javascript
class Hello extends React.Component {
  render() {
    const { name = '' } = this.props
    return (
      <div>
        <h3 className="hello-world">Hello {name}</h3>
      </div>
    )
  }
}
ReactDOM.render(
  <Hello name="Nat" />,
  document.getElementById('app')
)
```



## How to know props?
```javascript
<Hello name="Nat" />
```
|   Key   |   Value   |
|:--------|:---------:|
|   name  |   Nat     |



## Result
![react hello prop](https://image.ibb.co/n1QSzH/Screen_Shot_2018_04_27_at_23_34_08.png)



## State
```javascript
class Hello extends React.Component {
  state = {
    count: 0
  }
  render() {
    const { name = '' } = this.props
    const { count } = this.state
    return (
      <div>
        <p>{count}</p> 
        <h3 className="hello-world" onClick={() => this.setState({ count: count+1 })}>Hello {name}</h3>
      </div>
    )
  }
}
ReactDOM.render(
  <Hello name="Nat" />,
  document.getElementById('app')
)
```



## Must know!
State need initialize value



## Result
![react state count](https://image.ibb.co/hVCt6x/React_State_Count.png)



## Reuse Component
```javascript
class Hello extends React.Component {
  state = {
    count: 0
  }
  render() {
    const { name = '' } = this.props
    const { count } = this.state
    return (
      <div>
        <h3 className="hello-world" onClick={() => this.setState({ count: count+1 })}>Hello {name} {count}</h3>
      </div>
    )
  }
}
const names = ['john','susan','jean']
ReactDOM.render(
  <div>
    {names.map((name, index) => <Hello name={name} />)}
  </div>,
  document.getElementById('app')
)
```



## Error in log?
**Reusing component in react unique key is needed in props.**

<p style="color:red">"Warning: Each child in an array or iterator should have a unique 'key' prop.<p>



## Add key to props
```javascript
const names = ['john','susan','jean']
<div>
  {names.map((name, index) => <Hello name={name} key={index} />)}
</div>
```



## Life Cycle
![react life cycle](https://developmentarc.gitbooks.io/react-indepth/content/life_cycle/react-lifecycle-flow-chart-states.png)



## Example
```javascript
class Hello extends React.Component {
  state = {
    count: 0
  }
  componentWillMount(){
    this.setState({ count: Math.floor(Math.random()*10) })
  }
  render() {
    const { name = '' } = this.props
    const { count } = this.state
    return (
      <div>
        <h3 className="hello-world" onClick={() => this.setState({ count: count+1 })}>Hello {name} {count}</h3>
      </div>
    )
  }
}
```



## Result 
![React Component Life Cycle WillMount](https://image.ibb.co/cbxwtc/react_component_life_cycle.png)



# Training Code
[Code](https://codepen.io/phuditc/pen/aGBqqR?editors=1010) 



# Let's make todo app.
![React Todo UI](https://preview.ibb.co/bRNzeH/react_todo.png)



# Tools
- [Create React App](https://github.com/facebook/create-react-app) (**Suggest**)
- [Codepen](https://codepen.io)
- [Stackblitz](https://stackblitz.com)



# Maintanance Code
<h3>Git is the best way such as github.</h3>



# Javascript Characteristic
> <h3>Learn Once, Write Anywhere</h3>



# What javascript can do?
- Website
- Mobile App
- Destok App
- Presentations
- Game



# Example
![server nodejs](https://cdn0.froala.com/assets/editor/docs/server/meta-social/nodejs-34c5f8cc37f0756108c490a903d80176.png) <!-- .element height="30%" width="30%" -->
![react js](https://reactjs.org/logo-og.png) <!-- .element height="30%" width="30%" -->
![react native](https://filestore.hasura.io/v1/file/7723c234-4263-4599-9568-9d6788138c5b) <!-- .element height="15%" width="15%" -->
![electron](https://camo.githubusercontent.com/627c774e3070482b180c3abd858ef2145d46303b/68747470733a2f2f656c656374726f6e6a732e6f72672f696d616765732f656c656374726f6e2d6c6f676f2e737667) <!-- .element height="30%" width="30%" -->
![unity](https://unity3d.com/files/images/ogimg.jpg?1) <!-- .element height="30%" width="30%" -->



# Web App Flow
![REST API FLOW](https://cdn.app.compendium.com/uploads/user/e7c690e8-6ff9-102a-ac6d-e4aebca50425/f4a5b21d-66fa-4885-92bf-c4e81c06d916/Image/2344bb28bc75da26b24337547618c954/oneapi2.png)



# Javascript Basic
What did we learn from yesterday?

**Method for ?**
```javascript
  const names = ['john','susan','jean']
  names.map((name,index) => {
    console.log(name)
  })
```



# NPM ?
Node Package Manager

![node lego](https://d2eip9sf3oo6c2.cloudfront.net/series/square_covers/000/000/101/thumb/EGH_JS_NPM_Final.png)



## Let's try
```javascript
console.log(5+6)
```



## Let's try
```javascript
console.log('1'+'3')
```



## Let's try
```javascript
let x = 2
x = 4
console.log(x)
```



## Let's try
```javascript
const y = 1
y = 3
console.log(y)
```



# Comment in Javascript
**Single Line**
```javascript
//console.log(1)
```
**Multi Line**
```javascript
/*
this
code
will
not
execute
*/
```



# Case Sensitive
- Hyphens
<p>first-name, last-name, master-card, inter-city</p>
- Underscore
<p>first_name, last_name, master_card, inter_city</p>
- Camel Case
<p>FirstName, LastName, MasterCard, InterCity</p>



# Danger !
```javascript
console.log(2+3)
```

```javascript
console.log(2+3+'5')
```

```javascript
console.log('5'+2+3)
```

```javascript
console.log(2+3+'7'+5)
```



# Operators
assignment (=), addition (+)

subtraction (-), multiplication (*)

division (/), modulus (%)

increment (++), decrement (--)



# Example
|Operator|Example|Same As|
|:--------|:--------:|--------:|
|=|x = y|x = y|
|+=|x += y|x = x + y|
|-=|x -= y|x = x - y|
|*=|x *= y|x = x * y|
|/=|x /= y|x = x / y|
|%=|x %= y|x = x % y|



# Function
```javascript
function name(argument) {
  return // execute your code
}
```

```javascript
const name = (argument) => {
  return // execute your code
}
```



# Literals string
```javascript
`string text`
```

```javascript
`string text ${1+2} string text`
```



# Real Life Objects, Properties, and Methods
In real life, a person is an object

| Properties | Methods |
|:----------:|:-------:|
|name|speak|
|age|walk|
|weight|sleep|
|eyecolor|eat|



# Access Properties
- objectName.propertyName
- objectName["propertyName"]

**Example**

```javascript
const person = {
  name: 'nat',
  age: 25,
  weight: 49,
  eyecolor: 'black'
}
console.log(person.name) // nat
console.log(persone["age"]) // 25
```



# String
```javascript
const text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"
console.log(text.length) //26
```



# Danger
- == equal value
- === equality in both type and value

```javascript
console.log(1=='1') // true
console.log(1==='1') // false
```



# Condition
- if + else
- if + else if + else

```javascript
let age = 18
if(age > 18){
  console.log('Old enough')
} else {
 console.log('Too young')
}
```



# Switch
```javascript
switch(expression) {
    case n:
        code block
        break;
    case n:
        code block
        break;
    default:
        code block
}
```



# Export vs Export Default
```javascript
const hello = (text) => {
  return `hello ${text}`
}
export hello
```

```javascript
const hello = (text) => {
  return `hello ${text}`
}
export default { 
  hello
}
```



# Callback
```javascript
fs.readFile('input.txt', (err, data) => {
   if (err) return console.error(err)
   console.log(data.toString())
})
```



# Promise
```javascript
promise.then((result) => {
  console.log(result); // "Stuff worked!"
}, (err) => {
  console.log(err); // Error: "It broke"
});
```



# Import
```javascript
const hello = (text) => {
  return `hello ${text}`
}
export hello
```

```javascript
import { hello } from ''
console.log(hello('nat'))
```

```javascript
import { hello as greeting } from ''
console.log(greeting('nat'))
```



# Import
```javascript
const hello = (text) => {
  return `hello ${text}`
}
export default { 
  hello
}
```

```javascript
import greeting from ''
console.log(greeting.hello('nat'))
```



# Express JS
> Fast, Web minimalist web framework



# Babel Installing
```bash
$ npm install babel-cli babel-preset-env babel-preset-stage-2 --save -D
$ npm install babel-polyfill --save
```

**Create .babelrc**
```
{
  "presets": [
    "env",
    "stage-2"
  ],
  "plugins": []
}
```



# Express Installing
```bash
$ npm install express dotenv body-parser helmet http-status morgan express-validation compression --save
```



# HTTP VERB
| VERB | ACTION | USED FOR |
|:----:|:------:|:--------:|
| GET  |        | Retrieve items from resource|
| POST |        | Create new item in resource |
| PUT/PATCH|    | Update existing item in resource |
| DELETE|       | Delete existing item in resource | 



# Routing
```javascript
import express from 'express'
const PORT = process.env.PORT || 8080
const app = express()
app.get('*', res.json({ message: `it's work` }))
app.listen(PORT)
```



# Work Shop
| Name   | Method | URL            |
|--------|:------:|:--------------:|
| LIST   | GET    | /tasks         |
| CREATE | POST   | /tasks         |
| UPDATE | PUT    | /tasks/:taskId |
| REMOVE | DELETE | /tasks/:taskId |



# Mongoose 
```bash
$ npm install mongoose bluebird  --save
```



# Connection
```javascript
import mongoose from 'mongoose'
// const mongoUri = config.mongo.host
mongoose.connect(mongoUri, {
  reconnectTries: Number.MAX_VALUE, // Never stop trying to reconnect
  reconnectInterval: 500, // Reconnect every 500ms
  poolSize: 50, // Maintain up to 10 socket connections
  promiseLibrary: Promise,
  // If not connected, return errors immediately rather than waiting for reconnect
  bufferMaxEntries: 0
})
mongoose.connection.once('open', () => {
  console.log(`mongodb is connected!`)
})
mongoose.connection.on('error', () => {
  throw new Error(`unable to connect to database: ${mongoUri}`)
})
```



# Plugging in your own Promise lib.
```javascript
import Promise from 'bluebird'
mongoose.Promise = Promise
```



# Create Model
Create Folder 
models



# Schema
Create File **task.js**

```javascript
import mongoose, { Schema } from 'mongoose'
const taskSchema = new Schema({
  message: {
    type: String,
    required: true
  },
  complete: {
    type: Boolean,
    required: true,
    default: false,
  }
})
export default mongoose.model(`Task`, taskSchema)
```



# Query
```javascript
import Task from '../models/task'
Task.find({}).then((tasks) => {
  res.json({ tasks })
})
```



# React to Node
```bash
$ npm install axios --save
```



# Make Component
- TodoList
- TodoItems



# .env (NODE)
key=value
# .env (REACT)
REACT_APP_KEY=value