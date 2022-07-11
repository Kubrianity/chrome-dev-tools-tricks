# JavaScript 30 #9: chrome-dev-tools-tricks
This is the ninth practice of JavaScript30 Challenge. </br></br>
This practice shows some features of developer tools and console methods. </br></br>
## Usage & Features
- Interpolation
```
console.log("Hello, I am a %s!", "world")
```
- Styling
```
 console.log("%c I am some great text", "font-size:25px; color:red");
```
- Warning
```
console.warn("OH NOOO!!!")
```
- Error
```
console.error("Oops, error!")
```
- Info
```
 console.info("Octopuses have three hearts")
```
- Testing
```
console.assert(1 === 2, 'That is wrong'); //only fired when assertion is wrong 
```
- Clearing
```
console.clear()
```
- Viewing DOM elements
```
const p = document.querySelector("p")
console.log(p); //view the element
console.dir(p); //show methods and properties
```
- Grouping together
```
 const dogs = [{ name: 'Snickers', age: 2 }, { name: 'hugo', age: 8 }]
     dogs.forEach(dog => {
      console.group(`${dog.name}`);
      console.log(`This is ${dog.name}`);
      console.log(`${dog.name} is ${dog.age} years old`);
      console.log(`${dog.name} is ${dog.age * 7} dog years old`);
      console.groupEnd(`${dog.name}`);
    })
```
- Counting
```
console.count('Hermione')
console.count('Ron')
console.count('Harry')
```
- Timing
```
console.time('fetching data');
    fetch('https://api.github.com/users/Kubrianity')
      .then(data => data.json())
      .then(data => {
        console.timeEnd('fetching data');
        console.log(data);
      })
```
- Table
```
console.table(dogs)
```


