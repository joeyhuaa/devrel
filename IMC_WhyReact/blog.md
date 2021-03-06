<div align="center">
  <img src="./img/0.png" />
</div>

# What's with all the craze about React?
### by Joey Hua

## DISCLAIMER:

_This blog was intended for readers who have experience with HTML, CSS, and ideally, JavaScript. If you have no clue what I'm talking about, you will probably find this blog hard to understand._ 

## A Little Introduction

Now is a great time to learn web development! HTML, CSS, and Javascript are the core trio of languages to learn when it comes to mastering front-end skills. If you’re familiar with any of those, you've most likely heard of React.js, the flashy and widely popular new `div` on the `block` (have a sense of humor please!). Over the past five years or so, React has quickly become the go-to JavaScript library for building dynamic web apps. I emphasize "dynamic" because “static” is becoming a thing of the past. With the rapid advancement of today's technology, companies and consumers need websites that are flexible and can make UI and data changes seamlessly. Just think of your favorite destinations on the Internet, such as YouTube, Instagram, or Facebook—you will realize that these are _all_ dynamic web apps (more on this later). 

I wrote this blog to answer the one question undoubtedly bouncing around in your mind—what’s with all the craze about React? This is something I myself didn’t understand when I first began learning React and wish someone had told me. I’m a firm believer in understanding why you’re doing what you’re doing; thus, I believe addressing this topic will definitely make you a better React developer and spur you on in your learning.

<br />

<div align="center">
  <img src="./img/7.jpg" width="600" />
  <p>Programmers love trees. React-ers are no different. Keep reading!</p>
</div>

<br />

## What is React?
What exactly is React? Let’s begin with the fun explanation by starting with the name itself. React is a tool that’s designed to “react” to any changes that the user makes when interacting with a web app as long as they change app state or data. React is like an elegant flower dancing in the wind, constantly changing position but always staying intact. 

<br />

<div align="center">
  <img src="./img/2.jpg" width="600" />
  <p>React is one with nature.</p>
</div>

<br />

As for the more technical (and arguably more boring) explanation, React is a JavaScript library made for one purpose: to make the creation of UIs way more efficient than older methods. It’s essentially an extension of vanilla JavaScript that comes with a small but powerful API that serves as a bridge between the programmer and the **DOM** (DOM stands for **Document Object Model**, the tree structure that HTML uses to arrange elements on the page). Developers no longer have to manually communicate every update to the browser. Instead, developers simply tell React what to change. It'll then use something called the **Virtual DOM** to update the browser (more on this later).

<br />

<div align="center">
  <img src="./img/6.png" width="600" />
</div>

<br />

This is extremely useful for building web apps that need to change and re-render often. React allows us to simply tell it what we want to render or change while it handles all of the “how” grunt work behind the scenes. Without React, we’d have to do all of this heavy-lifting ourselves. With React, we can focus on what we as developers care about most: the UI and logic.

Before the days of React, websites were mostly static and pretty boring. They mainly just displayed information and offered very little user interactivity, if any (think back to the early 2000s). Fast-forward to the early 2010s when social media apps began rapidly rising in popularity, and with that, a new way of building web apps was developed when Facebook created the React library. 

<br />

<div align="center">
  <img src="./img/1.png" width="300" />
</div>

<br />

Compared to the not-so-distant past when websites consisted of several static and separate HTML pages with hard-coded content, React introduced the **single-page application** paradigm—creating one HTML template and dynamically injecting content into it based on the app state. Instagram is a quintessential example of a single-page app built with React. 



<div align="center">
  <img src="./img/3.png" width="400" />
  <p>We have React to thank for Instagram.</p>
</div>

<br />

Long gone are the days of hard-coding content into `div` and `p` tags. In React, HTML is kept relatively bare-bones; any elements will serve as templates that hold data which is dynamically-passed via JavaScript. That being said, don't think HTML isn't important anymore. React won't work without HTML since HTML is still the skeleton of every website. It simply means the **focus** has shifted from writing static content to writing code that renders content based on UI state. 

You can totally learn React if you have experience with HTML, CSS, and, ideally, JavaScript. Since JavaScript is the language that React uses, they are syntactically and conceptually similar, making React easier to learn with prior JavaScript knowledge. However, even if you have no experience with vanilla JavaScript, you can still learn React if you put in the work. I personally jumped straight into React because I'm impatient, which meant I had to teach myself JavaScript _and_ React simultaneously. I made it out the other side relatively unscathed, but I highly recommend you save yourself a headache and learn vanilla JavaScript first, _then_ React. And if you have zero programming experience, then your first priority should be to learn HTML, CSS, JavaScript, then React, in that order.

As I stated above, JavaScript is the foundation of React. React is a library built on top of the language, which means that it comes with many useful new features. One fundamental feature is **JSX**—the ability to write HTML code inside your React files. Another key feature is **inline-CSS**—the ability to write CSS in React files. In addition to being two of the most fundamental and frequently used features, JSX and inline-CSS are a testament to how tightly integrated HTML, CSS, and JavaScript are in React. Have fun discovering all the other cool features on your own!


## How does React work?

In React, **components** are the building blocks of your app and can be written as either functions or objects. Components dynamically render content via **props** and **state**. 

**Props** are just like parameters you pass to a function—the specific props you design for your component and the data you pass to it in the form of said props will dictate what's being rendered. Prop data is passed **externally** to a component.

**State** is a variable or set of variables that control a component's... state (I actually think it's most intuitive to self-define state). State variables are created and updated **internally** and can be used to render content dynamically based on logic you provide.

The cool part is that components are designed to interact with each other. Components can render other components, props can be passed from one component to another, and state can also be passed as a prop so that it can be updated externally. If this is confusing, don't worry. Practicing how to write React will clear things up. 

React encourages the creation of “reusable, composable, and stateful components.” Let me translate that as such: make components that can generalize into more specific use cases and make sure they have internal properties that can handle the content they display. 

<br />

<div align="center">
  <img src="./img/10.jpg" width="400" />
</div>

<br />

Another key thing to know is that React uses a tree hierarchy to internally structure your components, much like how the DOM is a tree that structures HTML elements. This means that there is a root file (index.js) that extends into a tree of however many parent and child components you want. This goes hand-in-hand with the idea of “generalizing components,” as components should get more general the closer you get to the root.

<br />

<div align="center">
  <img src="./img/8.png" width="600" />
  <p>Gotta get back to our Roots.</p>
</div>

<br />

I will end this section on one final key point to understand about React. Remember when I mentioned the Virtual DOM at the start of this section? Well, it’s essentially a copy of the browser DOM (HTML tree) that React stores in memory. React does this for efficiency’s sake: React makes changes directly to the Virtual DOM, then renders only the differences between the Virtual DOM and the browser DOM. With vanilla JavaScript, the browser DOM would need to re-render itself entirely on each update, which is computationally much more expensive. Don’t worry if this is slightly confusing, things will become more clear as you get more practice coding React. For now, just know that React makes web dev life much easier.

<br />

<div align="center">
  <img src="./img/5.png" width="600" />
  <p>The Virtual DOM compares itself to the browser DOM and smartly re-renders only what has been changed (in red), instead of re-rendering the entire DOM.</p>
</div>

<br />

## When to React and when not to React?
I just spent lots of time describing what React is great at and how it has ushered in a new paradigm into the web dev universe. However, React doesn't need to be used for EVERYTHING web-related. For instance, if all you want is a simple blog site, making a React app would be overkill, at least for 99% of blogs out there. 

You should strongly consider React when you are building something that is **highly interactive**. This is exactly what React was built for. Projects like messenger apps, social media apps, board games, audio workstations, and notetaking and productivity apps are where React will shine brightest.


## How to React!
Now comes the fun part—coding! In this final section, I have included several code examples illustrating fundamental React concepts to get you familiar with the code. At the very end, I have included three great resources where you can learn more about React in-depth. 

I made these examples as easy as I could manage, but there is bound to be some syntax that's confusing if you're new to React. This is unavoidable, as some lines are required for all of the code to function. I have explained the essential portions in comments, but don't worry about the parts you don't understand. Instead, try to get a feel for how React code flows and is structured. In due time, everything will make sense! 

For each example, I have embedded links to CodeSandBox so that you can play around with the code yourself and see it being rendered in the browser (highly encouraged!). Keep in mind that I designed these examples to demonstrate the basics. You can do **many more** fancy and creative things with React!

1. <a href="https://codesandbox.io/s/react-hooks-usestate-j5iu3?file=/src/index.js">React class component</a>

> Components are the building blocks of React apps. Here's an example of a simple React **class component** that renders a sentence inside of a `div`. Click the title (next to "1.") to play with the code on CodeSandBox!  

```js
import React from "react"; 
import ReactDOM from "react-dom";

// Class components are essentially JavaScript objects
class NewComponent extends React.Component {
  
  // This is where content is rendered in the form of HTML or other React components
  render() {
    return (
      <div>Hello, I'm a new React Component!</div>
    )
  };
};

// render to the DOM
ReactDOM.render(
  <NewComponent />,
  document.getElementById("root")
);
```

<br />

2. <a href="https://codesandbox.io/s/react-hooks-usestate-54p5z?file=/src/index.js">React functional component (more popular)</a>

> As I mentioned earlier, components can also be written as functions in React. 

> Generally speaking, class components require more boilerplate than **functional components** to perform the same tasks. However, class components have access to an array of <a href='https://blog.bitsrc.io/react-16-lifecycle-methods-how-and-when-to-use-them-f4ad31fb2282'>lifecycle methods</a> that allow for precise control over rendering, updating, etc.

> Here's the same component as the one in Example 1, but in functional form instead. 

```js
import React from 'react';
import ReactDOM from 'react-dom';

// Functional components are becoming more popular than class components, since they are more flexible and can perform the same duties with less code.
function AnotherComponent() {

  // You don"t need a render() {} block like in class components, just a return() function
  return (
    <div>Hello, I'm a new React Component!</div>
  );
};

ReactDOM.render(
  <AnotherComponent />,
  document.getElementById("root")
)
```

<br />

3. <a href="https://codesandbox.io/s/react-hooks-usestate-r0uk0?file=/src/index.js">React JSX</a>

> Here's a simple example of **JSX**. I'm assigning a `div` to the variable _element_ and embedding the variable _anime_ inside my content. JSX is super useful since it allows you to interweave JavaScript and HTML code together! 

```js
import React from 'react';
import ReactDOM from 'react-dom';

let anime = "Hunter x Hunter";

// A very simple example of JSX - assigning an HTML element to a variable
let element = <div>My favorite anime is {anime}.</div>;

ReactDOM.render(
  element,
  document.getElementById("root")
);
```

<br />

4. <a href="https://codesandbox.io/s/react-hooks-usestate-bfkb3?file=/src/index.js">React inline CSS </a>

> In React, there are two ways to <a href='https://www.w3schools.com/react/react_css.asp'>apply styling to components</a>. The first is **inline CSS**, which is the focus of this example. The other way is to import external style sheets.

> This example builds off of the code in Example 3. The only addition is that I applied styling to the `div` element in the form of a JavaScript object. 

```js
import React from 'react';
import ReactDOM from 'react-dom';

let anime = "Hunter x Hunter"
let element = 
  <div 
    // Inline-CSS is written as a JavaScript object
    style={{
      border:"solid purple 2px", 
      padding:"5em",
      textAlign: "center" // JSX uses camelCase syntax instead of hyphenating multi-word attributes like in vanilla CSS
    }}
  >
    My favorite anime is {anime}.
  </div>

ReactDOM.render(
  element,
  document.getElementById("root")
);
```

<br />

5. <a href="https://codesandbox.io/s/react-hooks-usestate-1ewyf?file=/src/index.js">React component with props</a>

> **Props** are essentially parameters you pass to your components in order to control functionality. 

> In this example, I use a functional component to render a list of anime titles as a `ul`. There are two props—_styles_ allows me to pass whatever CSS I want, and _animes_ allows me to control the content I want rendered inside of the `ul`.

> The prop names and locations are defined within my component, but the actual content of those props is defined externally. Scroll to the bottom of this example to see how it's done!

```js
import React from "react";
import ReactDOM from "react-dom";

// If you want your component to be able to hold props, simply pass "props" as a parameter.
// Alternatively, you could omit "props" and individually put prop names within an object, and pass the object as a parameter to your component
function FunctionalComponentWithProps(props) {
  return (
    <div>
      <h1>You should watch the following animes:</h1>

      <div style={props.styles}>
        <ul>
          {props.animes.map(anime => (
            <li>{anime}</li>
          ))}
        </ul>
      </div>
    </div>
  );
}

// Here is the "style" prop I will pass to my component
let myStyles = {
  color: "orangered",
  marginTop: "10px"
};

// Here is the "animes" prop I will pass to my component
let myAnimes = ["Hunter x Hunter", "Neon Genesis Evangelion", "One Piece"];

ReactDOM.render(
  <FunctionalComponentWithProps
    styles={myStyles} // passing styles as prop
    animes={myAnimes} // passing animes as prop
  />,
  document.getElementById("root")
);
```

<br />

6. <a href="https://codesandbox.io/s/react-hooks-usestate-lr8nj?file=/src/index.js">React component with state</a>

> Last, but definitely not least, here's an example of **state**. If you're familiar with object-oriented programming, think of state as class attributes, except you can update it throughout a component's lifecycle and pass it between different components (<a href='https://reactjs.org/docs/lifting-state-up.html'>lifting state</a>). 

> In this example, I have two state variables—_animes_ holds the anime titles that are waiting to be recommended, and _recs_ holds the anime titles that have been recommended. These two state variables are updated whenever a button is pressed. Take your time to mess around with the code in this example, since there are quite a few fundamental concepts to digest.

> Until the introduction of <a href='https://reactjs.org/docs/hooks-intro.html'>hooks</a>, functional components were stateless—they COULD NOT use state, unlike class components. With hooks, we can use state and control lifecycle events in functional components, although it's a bit different from how it's done in class components.

> State is one of the most important concepts to grasp in React, so I definitely encourage you to get a ton of practice with it! 

```js
import React, { useState } from 'react';
import ReactDOM from 'react-dom';

// This is our initial state, will also make resetting state easier
let initialState = {
  animes: [
    "Hunter x Hunter",
    "One Piece",
    "Neon Genesis Evangelion"
  ]
}

function FuncComponentWithState() {

  // This is where we initialize our state variables for our component
  let [animes, setAnimes] = useState([...initialState.animes]);
  let [recs, setRecs] = useState([]);
  
  let handleClick = () => {
    if (animes.length !== 0) {

      // Updating state happens here
      setAnimes(animes.slice(0, animes.length-1))
      setRecs(recs.concat(animes[animes.length-1]))
    }

    else {
      alert("We have no more anime recommendations for you today! Please return after you have finished watching the ones we have already given you. Good luck!")
    }
  };

  // This variable will hold all anime recommendations
  // map() is an extremely useful Array function you will be using very frequently
  let recommended = recs.map(rec => <p style={{margin:".5em"}}>{rec}</p>)

	// Actual content to be rendered is inside return()
	return (
		<div style={{display:"block", padding:"1.5em"}}>

      <button 
        style={{padding:".5em", margin:"1em"}}
        onClick={handleClick}
      > 
        Click to get new anime recommendation!
      </button>

      <div>{recommended}</div>

      <button
        style={
          animes.length === 0 
            ? 
          {} : {'visibility':'hidden'}
        }
        onClick={() => {
          setAnimes(initialState.animes);
          setRecs([])
        }}
      >Reset</button>
    </div>
	);
};

ReactDOM.render(
	<FuncComponentWithState />,
  document.getElementById("root")
);
```

<br />

Hopefully, you now have a better understanding of what React is and why it's used. I highly encourage you to make your own React apps; no other method of learning comes close in terms of enjoyment and improvement potential. Below are some great resources to get you started on your React journey. Thank you for reading!

<a href="https://reactjs.org/tutorial/tutorial.html">React Tic-Tac-Toe Beginner Tutorial</a>

<a href="https://reactjs.org/docs/state-and-lifecycle.html">State and Lifecycle</a>

<a href="https://scrimba.com/p/p7P5Hd/Index">Scrimba: A Great Interactive Resource for learning how to write React code</a>









