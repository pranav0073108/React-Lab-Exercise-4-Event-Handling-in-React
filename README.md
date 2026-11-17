# React-Lab-Exercise-4-Event-Handling-in-React

## Name : PRANAV K
## Register number : 2305001026

# Aim
To understand and implement event handling in React using events such as onClick, onChange, and onSubmit.
# Program 
## App.jsx
## onclick event function
```python
App() {
function handleClick() {
alert("Button was clicked!"); 
  }   return ( 
    <div> 
      <h1>React Event Handling</h1> 
      <button onClick={handleClick}> 
        Click Me 
      </button> 
    </div> 
  ); 
} export default App;

```
## onclick with state
```python
import { useState } from "react";
function App() { 
  const [count, setCount] = useState(0); 
  function handleClick() { 
    setCount(count + 1); 
  } 
  return ( 
    <div> 
      <h1>Click Counter</h1> 
      <h2>Button clicked: {count} times</h2> 
      <button onClick={handleClick}> 
        Click Me 
      </button> 
    </div> 
  ); 
} 
export default App; 

```
## on change event
```python
import { useState } from "react"; 
function App() { 
  const [name, setName] = useState(""); 
  function handleChange(event) { 
    setName(event.target.value); 
  } 
  return ( 
    <div> 
      <h1>Student Name</h1> 
      <input 
      type="text" 
        placeholder="Enter your name" 
        onChange={handleChange} 
      /> 
      <h2>Hello, {name}</h2> 
    </div> 
  ); 
} 
export default App; 

```
# Output:
 ## on click event

 <img width="890" height="318" alt="image" src="https://github.com/user-attachments/assets/c562f135-2ad7-4abe-b3a2-e7b07cd80331" />

 ## on click with state

 <img width="867" height="330" alt="image" src="https://github.com/user-attachments/assets/a8656ab7-fafc-4f79-89f1-66c055b6e252" />

 # Result:
 Thus, React event handling was successfully implemented using the onClick and onChange events. The application responded to button clicks, maintained a click counter using useState, and displayed the student's name dynamically based on user input.
 

 


