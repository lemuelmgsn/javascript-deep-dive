# Workshop JavaScript Deep Dive

## Program

* Motivation for deep diving in JavaScript 
* Theory based on two demo's: a functional - and an object-oriented one
* Practical applications in a SvelteKit Project

### Motivation for deep diving in JavaScript

* Making it more fun to write JavaScript
* Needed skills to land a job:  [10 Interview Questions Every JavaScript Developer Should Know in 2024]
* How to handle your Imposter Syndrome
* How to handle bro coding culture, how to survive the complexity of the web.

### Theory based on two demo's: a functional - and an object-oriented one

The main concepts derived from the code:
* Fundamentals of JavaScript (Constructor Functions, Context (this), Scope)
* Functions and Closures (Callbacks, Returning Functions, Binding Functions)
* Array Manipulation and Logical Operations (Array Methods, Short-Circuiting, Event Delegation)
* Async Programming in JavaScript (Promises, Async/Await)
* Code Flow and Control Structures (Defensive Programming, Return Early, object destructuring, spread operator)
* Advanced JavaScript Concepts (Chaining Methods, Concurrency Model, Event Loop (Call Stack, Event Queue, and Microtask Queue), Hoisting, Closure)

Bron: You Don't Know JS

Topics we encounter when using the debugger from the **Sources** tab in DevTools:
* Application state
* Scope 
* Context (this)
* Call Stack (Concurrency Model / Single thread)
* Extra: modules (scoped, deferred, async)


### Practical applications in a SvelteKit Project

Opdracht Refactor your JavaScript:
* Object destructuring
* Short circuiting
* One responsibility rule for functions
* Pseudo-Private Custom Properties (Scope CSS)

Decide which conventions you apply to your work


<!-- references -->
[10 Interview Questions Every JavaScript Developer Should Know in 2024]: https://medium.com/javascript-scene/10-interview-questions-every-javascript-developer-should-know-in-2024-c1044bcb0dfb

# Eigen aantekeningen
```
<script type="module" src="static/js/script.js">
```

elk script wat je in laad in script.js is een module.

- modules zijn scoped by default
- modules zijn deferred by default (word ingeladen nadat alles is ingeladen: html css)
- modules zijn async by default en je kan ze awaiten
- modules run script in strict mode


Local scope - in een script waar de global scope niet bij kan
Global scope - in de browser zelf?


## Scope
- function/blocks

## Context
- objecten (this)


### Concurrency model
- wat word er tegelijkertijd in code uitgevoerd
- Javascript is single threaded
- in de eventloop kijken, eventloop maakt het mogelijk om in een single threaded omgeving dingen tegelijk te doen.

Breakpoints: je kan in sources je code lijnen selecteren en op de button klikken om te kijken wat er in je browser gebeurt tot het breakpoint. Dit is een andere manier voor debuggen

je kan in je js code zelf ook "debugger" schrijven, dit maakt automatisch een breakpoint voor in de source debugger.

short circuit 

### object destructuring
- dit zorgt ervoor dat je niet telkens data.title etc moet typen.

```
const {title, sprintnumber, startdate} = data

<h1>{title}</h1>

```

spread operator om nieuwe dingen aan een array toe te voegen




