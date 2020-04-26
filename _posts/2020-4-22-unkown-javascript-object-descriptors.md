---
layout: post
title: Unknow JavaScript - Object Descriptors
subtitle: Object class in JavaScript has one method which I think is a little unknown to most of the JavaScript Developers out there.
avatar: /img/hello_world.jpeg
published: true
categories:
    - JavaScript
tag:
     JavaScript
---


### Object.defineProperties(object, property)
Used to define new properties or properties to the existing object or to modify existing properties.

> You can only call this method on **Object** constructor

Example 1.
```javascript
  const obj = {};
  Object.defineProperties(obj, {
      proparty: {
          value: "Suhas",
          enumerable: false,
          writable: false,
          configurable: false
      }
  });
```
<!-- 
<img src="/img/post/js-descriptor/object-define-properties.png" alt="define properties example"> -->

Example 2.

```javascript
  const obj = {};
  Object.defineProperty(obj, "property2", {
      value: "More",
      enumerable: false,
      writable: false,
      configurable: false
      
  })
```
<!-- <img src="/img/post/js-descriptor/define-property-example.png" alt="define property example">  -->


using writable property we can restrict properties from being updated.


<img src="/img/post/js-descriptor/writable-example.png" alt="define property example"> 


For further reading refer [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object)

Follow me on [Twitter](https://twitter.com/suhas0101)


