### List of things I learnt during the course of this project
1. **Difference between onClick in HTML vs JSX -** Events are written in lowercase, e.g. onclick, while in JSX events are written in camelCase, e.g. onClick. You can directly assign JavaScript code to the event attribute, e.g. 
```
    <button onclick="alert('Hello')">Click me</button>
```
But in JSX, It is a best practice to define event handler functions separately and pass them as references to the event attributes, e.g.
```
    <button onClick={handleClick}>Click me</button>
```
you can also use inline arrow functions directly in JSX if the logic is simple:
```
    <button onClick={() => alert('Hello')}>Click me</button>
```

2. **Difference between onClick{alert(previous)} and onClick{( )=> alert(next)}**- These differences arise from how JavaScript functions are executed and how event handlers are assigned in React.
```
    onClick={alert(previous)}
```
- Executes immediately when the component renders.
- No event handling occurs because the function is already executed.
- onClick={alert(previous)}: Assigns the result of alert(previous) (which is undefined) to onClick.

```
    onClick={() => alert(next)}
```
- Executes when the button is clicked.
- Proper event handling occurs when the button is clicked.
- This syntax assigns an anonymous function to onClick. 
- onClick={() => alert(next)}: Assigns a function to onClick that will call alert(next) when the event occurs.

3. **color highlight -** is an extenstion in VScode used for highlighting colors

4.
5.
6.

