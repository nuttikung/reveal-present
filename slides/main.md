# Who am I?
<p>Name : Nat</p>
<p>Education : B.Sc(IT KMITL)</p>
<p>Work : Sharmble Technology</p>

[Sharmble Wb](https://sharmble.com)



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


