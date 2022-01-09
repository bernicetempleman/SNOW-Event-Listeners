# SNOW-Event-Listeners

An event listener is a procedure or function in a computer program that waits for an event to occur; that event may be a user clicking or moving the mouse, pressing a key on the keyboard, or an internal timer or interrupt. 
The listener is in effect a loop that is programmed to react to an input or signal.
Event Listener are implemented by two methods
The addEventListener() method
The removeEventListener() method

## The addEventListener() method


```
Add an event listener that fires when a user clicks a button
Syntax
   element.addEventListener(event, function, useCapture);
Example (Event Listener applied to function)
element.addEventListener("click", myFunction);
function myFunction() { 
alert ("Hello World!");
}

```

## The removeEventListener() method
```
The removeEventListener() method removes event handlers that have been attached with the addEventListener() method.
Example

     element.removeEventListener("mousemove", myFunction);
```
## Bubbling / capturing
- Event propagation is a way of defining the element order when an event occurs
- In bubbling the inner most element's event is handled first and then the outer: the <p> element's click event is handled first, then the <div> element's click event.
- In capturing the outer most element's event is handled first and then the inner: the <div> element's click event will be handled first, then the <p> element's click event.
 - With the addEventListener() method you can specify the propagation type by using the "useCapture" parameter:
- addEventListener(event, function, useCapture);
- The default value is false, which will use the bubbling propagation, when the value is set to true, the event uses the capturing propagation.


## Event Object
- When an event occur in HTML, the event belongs to a certain event object, like a mouse click event belongs to the MouseEvent object.
- Some of the properties and methods of the event objects are
![image](https://user-images.githubusercontent.com/12488769/148699808-f09dac14-0061-47b1-a1d0-195bafffe310.png)
  ![image](https://user-images.githubusercontent.com/12488769/148699814-8e08f61d-5b93-48be-a7e0-debb065f08a1.png)
![image](https://user-images.githubusercontent.com/12488769/148699823-25b2d7cc-9fc8-432d-8fdd-cd2f1a2dd009.png)



