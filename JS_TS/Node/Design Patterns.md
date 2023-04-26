# Creational

## Factory

// TODO: Need to give examples here

The core advantage of the **Factory Pattern**, is the ability to decouple the creation of an object from one particular implementation. Factories can also be used to force encapsulation by leveraging closures.

## Builder

// TODO: Need to give examples here

Builder pattern simplifies the creation of complex objects by providing a fluent interface, which allows us to build the object step by step. This helps readability and the general developer experience when it comes t o creating complex objects.

- The main objective is to beak down complex constructors into multiple more readable + manageable steps.
- Try to create builder methods that can set multiple relation params at once.
- Deduce and implicitly set parameters based on values received. 

## Revealing Constructor

This pattern is something that was made in the JS/Node community to solve a tricky problem. It helps us reveal some private functionality of an object only at the moment of the objects creation. This is useful when we want t o allow an objects internals to be manipulated only during its creation phase. This allows for some interesting scenarios:

- Creating objects that can only be modified at creation
- Creating objects whose custom behaviour can be defined only at creation
- Creating objects that can be initialized only once at creation

```js
const object = new SomeClass(function executor(revleadMembers)) {});
```

The pattern is made of 3 fundamental parts. 

- Constructor that takes a function called the executor
- The executor which is invoked at creation
- The revealed members it receives at creation time

### Immutable Buffer

Immutable objects are only modifiable by creating new objects. They create a strong guarantee that they won't be modified. This makes it easy to track state changes. A common use case for this *change detection*. This technique is used heavily in frontend to detect UI changes.

Using the [[#Revealing Constructor]] pattern we are able to achieve this:

```ts
const MODIFIERS_NAMES = ['swap', 'write', 'fill'];

export class ImmutableBuffer {
	constructor(size, executor) {
		const buffer = Buffer.alloc(size);
		const modifiers = {};
		
		for (const prop in buffer) {
			if (typeof buffer[prop] !== 'function') {
				continue;
			}
			
			if (MODIFIER_NAMES.some(m => prop.startsWith(m))) {
				modifiers[prop] = buffer[prop].bind(buffer);
			} else {
				this[prop] = buffer[prop].bind(buffer);
			}
		}
		
		executor(modifiers);
	}
}
```

## Inversion of Control

https://github.com/inversify/InversifyJS

Inversion of Control (IoC) is a design principle used in software engineering to achieve a more flexible and modular architecture. It is mainly applied to manage dependencies. In traditional services are responsible for managing their dependencies.

IoC reverses this responsibility by moving the task of creating and managing dependencies from the components themselves to an external entity, typically called a container or a framework.

There are several techniques to implement IoC, such as:

1.  Dependency Injection (DI): This is the most common IoC technique. In DI, dependencies are provided to components (usually through constructors, setters, or interfaces) rather than being created by the components themselves. This makes it easier to swap out dependency implementations, and promotes the use of interfaces, leading to a more modular design.
   
2.  Service Locator: This pattern involves using a central registry, called a service locator, which components can use to request their dependencies. Instead of creating dependencies themselves, components look up the dependencies in the service locator.

3.  Event-driven programming: In this approach, components communicate through events rather than direct method calls. Components can subscribe to and emit events, reducing the coupling between them. This can be seen as a form of IoC, as the flow of control is inverted - instead of a component explicitly calling a method on another component, it emits an event that is then handled by any subscribed components.

# Structural

Structural design patterns are focused on providing ways to realize the relationships between entities. This will focus on:

- Proxy: Allows us to control access to another object
- Decorator: A pattern to augment the behaviour of an existing object dynamically.
- Adapter: A pattern that allows us to access the functionality of an object using a different interface.

## Adapter

// TODO: Need to give examples here

Adapter pattern allows us to access functionality of an object using a different interface. Similar to how in real life if you have a USB-C to USB-A you would need some form of adapter to bridge this. 

In software the adapter pattern is used to take the interface of an object and make it compatible with another that is expected. 

## Proxy

A **proxy** is an object that controls access to another object, called the **subject**. It intercepts all or some of the operations that are meant to be executed on the subject, augmenting or complementing their behaviour. Proxy is useful for things such as:

- Data validation
- Security
- Caching
- Lazy initialization
- Logging
- Remote Objects

```ts
class MyClass {
	someMethod() {
		return "result";
	}
}

class MyClassProxy(myClass) {
	constructor() {
		this.#myClass = myClass;
	}

	someMethod() {
		console.log("This is a proxy method");
		return this.#myClass.someMethod();
	}
}
```

In JavaScript there are 3 ways to achieve the proxy pattern:

- **Object Composition:** This is as per the example above. Where we mi-mick the original class and essentially create a wrapper around the subject to do what we need.
- **Object Augmentation:** This is what is commonly referred to as monkey patching. This will actually mutate the original subject. However as a result we do not have to implement every method of the result as we will be dealing with it once returned.
- **Proxy Object:** Only available in ES5, this is a great middle ground where we only have to implement the methods we want to. On top of that it returns the same instance type of the subject. This makes it a very powerful tool.

## Change Observer with Proxy

The Change Observer Pattern is a design pattern in which the subject notifies one or more observers of any state changes. 

```ts
function createObservable(target, observer) {
	const observable = new Proxy(target, {
		set(obj, prop, value) {
			if (value !== obj[prop]) {
				const prev = obj[prop];
				obj[prop] = value;
				observer({prop, prev, curr: value});
			}
			
			return true;
		}
	});

	return observable;
}
```

## Decorator Pattern

// TODO: Need to give examples here

The decorator pattern is a structural design pattern that consists in dynamically augmenting the behaviour of an existing object. It is different from classical inheritance, because the behaviour is not add to all the objects of the same class, but only to the instances that are explicitly decorated.

The proxy and decorator, although different in concept, share the same implementation strategies: 

- Composition
- Augmentation
- Proxy Object

# Behavioural Patterns

This focuses on understanding how we can combine objects and how to define the way they communicate so that the behaviour of the resulting structure becomes extensible, modular, reusable, and adaptable.

## Strategy

// TODO: Need to give examples here

Strategy pattern enables an object, called the context, to support variations in its logic by extracting the variable part into separate, interchangeable objects called strategies.

This pattern can be considered close to the adapter pattern. However the difference between the two is that the adapter pattern does not add any behaviour to the adaptee; it just makes it available under another interface. With a strategy pattern the context and the strategy implement tow different parts of an algorithm and therefore both implement some kind of logic and both are essential to build the final algorithm.

Good use case in the wild is the PassportJS Library.

## State Pattern

// TODO: Need to give examples here

The State pattern is a specialization of the strategy pattern where the strategy changes depending on the state of the context.

This means that, unlike the strategy pattern, the state pattern can changing over it's life time. Thus allowing it's behaviour to change. 

## Template

// TODO: Need to give examples here

This pattern has a lot in common with the strategy pattern. It defines an abstract class that implements the skeleton of a component where some of its steps are left undefined. The main difference between the 2 lies in their structure and implementation. Both allow us to change the variable parts of a component while reusing the common parts. However while strategy allows us to do it dynamically at runtime., with Template, the component is determined the moment the concrete class is defined.

The best example we have already used for this template pattern is the Streams we were working with. Where we took the template methods and put in our own behaviour.

## Iterator

The iterator is a fundamental pattern and its so important and commonly used that it is usually built into the programming language itself. Iterables are objects that implement an `@@iterator` method.

The iterator pattern defines a common interface or protocol for iterating the elements of a container, such as an array or tree data structure.

### Iterator:

An iterable is an object that can be looped through using a specific protocol, which requires the object to implement a method called ``Symbol.iterator``

```js
const myArray = [1, 2, 3];

for (const element of myArray) {
  console.log(element); // Output: 1, 2, 3
}
```

### Iterable:
An iterator is an object that is responsible for keeping track of the current position in the iterable and providing a way to access the next element in the sequence.

```JS
const myArray = [1, 2, 3];
const iterator = myArray[Symbol.iterator]();

let nextElement = iterator.next();
while (!nextElement.done) {
  console.log(nextElement.value); // Output: 1, 2, 3
  nextElement = iterator.next();
}
```

Obviously arrays, maps etc are iterables. However you can create your own iterators that keep track of its own iterable. This could be in shape of a class or function that returns some iterable.

In doing so this may contain some custom iteration logic to iterate over some data. Some common data structures in JavaScript that accept iterables:

- `Map`
- `WeakMap`
- `Set`
- `WeakSet`
- `Promise.all/Promise.race`
- `Array.from`

On the Node side the most notable would be `stream.Readable.from` which creates a readable stream out of an iterable object.

## Async Iterators

Iterators we have seen so far return a value synchronously. However how would this work in async land? Some examples may be dealing with a bunch of HTTP requests or results of a SQL query.

Async iterables are objects that implement an `@@asyncIterator` method. Or in other words a method accessible through the `Symbol.asyncIterator` key.  

Async Iterables can be looped over using the `for await...of` syntax. Which can only be used inside an async function. This is essentially just syntactic sugar for the following:

```js
const asyncIterator = iterable[Symbol.asyncIterator]();
let iterationResult = await asyncIterator.next();
while (!iterationResult.done) {
	console.log(iterationResult.value);
	iterationResult = await asyncIterator.next();
}
```

## Generator

Generators also known as `semicoroutines`. They are a generalization of standard functions, in which there can be different entry points. In a standard function we can only have one entry point, which corresponds to the invocation of the function itself. However in a generator function it can be suspended, using the yield statement, and then resumed at a later time. 

Among other things generators and well suited to implement iterators. In fact the generator object returned by a generator function is both an iterator and iterable

```js
function * myGenerator() {
	// body
}
```

Invoking a generator will not execute the body immediately. It will rather return a generator object. Calling next will start or resume the execution of the generator until the yield instruction or the generator returns. 

`yield` followed by a value is equivalent also to returning `{done: false, value: x}` from the iterator, while returning a value x is equivalent to returning `{done: true, value: x}`.

In a generator the `next` method optionally accepts arguments:

```js
function * twoWayGenerator() {
	const what = yield null;
	yield `Hello ${what}`;
}
```

By calling the above as:

```js
const twoWay = twoWayGenerator();
twoWay.next();
console.log(twoWay.next('world'));
```

We will now populate the value of `const what` as the next generation populate this.

Generators can be a great replacement for customer iterators, since they are iterable. This make's them somewhat more intuitive.

## Middleware

Middleware can be defined as a layer that acts as glue between services. The software the in the middle.

```js
class MiddlewareManager {
  constructor() {
    this.middlewares = [];
  }

  use(middleware) {
    this.middlewares.push(middleware);
  }

  run(data) {
    let result = data;
    for (const middleware of this.middlewares) {
      result = middleware(result);
    }
    return result;
  }
}

const middlewareManager = new MiddlewareManager();
middlewareManager.use((data) => {
  console.log(`Received data: ${data}`);
  return data.toUpperCase();
});
middlewareManager.use((data) => {
  return `Modified data: ${data}`;
});

const result = middlewareManager.run('hello world');
console.log(result);
```

This is a trivial example. However the idea here is about creating a manager that has a use function. This then allows you to load up different middleware that will then get executed in order when run. 

This means we will see it pass in `hello world`, transform that to uppercase and return the final result as `HELLO WORLD`. 

## Command Pattern

// TODO: Need to give examples here

The command pattern can be described as follows:

- **Command** is the object encapsulating the information necessary to invoke a method or function
- **Client** is the component that creates the command and provides it to the invoker
- **Invoker** is the component responsible for executing the command on the target.
- **Target** (**receiver**) is the subject of the invocation. It can be a lone function or a method of an object.

