# Explore asynchronicity and the event loop in Javascript

<img src="./img/timeline-example.png" width="600" height="350" />

## Learning objectives

 * Describe "the flow of control of a program" as "the order in which the parts of the code are executed".
 * Understand how asynchronous behaviour is different from synchronous.
 * Follow the flow of control to help you understand how callbacks work.

## Instructions

For each piece of code below:

1. Read the code.
2. Write down your prediction of what would happen if you run it (what will appear on the console, and in what order).
3. Run the code by pasting it in the console of your browser.
4. Compare the actual result with your predictions.


## Code

---

```js
setTimeout(() => {
	console.log('hello')
}, 1000)
```
---

```js
const callback = () => {
	console.log('hello')
}

setTimeout(callback, 1000)
```

---

```js
console.log('A')

const callback = () => {
	console.log('B')
}

console.log('C')

setTimeout(callback, 1000)

console.log('D')
```

---

```js
console.log('A')

const callback = () => {
	console.log('B')
}

console.log('C')

setTimeout(callback, 0)

console.log('D')
```

---

```js
let a = 10

const callback = () => {
	a = 20
}

setTimeout(callback, 1000)

console.log(a)
```

---

```js
let a = 10

const callback = () => {
	a = 20
}
setTimeout(callback, 0)

console.log(a)
```

---

```js
let a = 10

const callback = () => {
	a = 20
	console.log(a)
}
setTimeout(callback, 0)
```

---

```js
const callback = () => {
	return "hello"
}
setTimeout(callback, 2000)
```

## Reflection

* What is a callback?
* Can you explain why these are antipatterns:
  * having a callback that returns a value
  * having a callback that changes global state