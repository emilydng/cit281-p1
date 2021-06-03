## Project 1


```markdown
Goals and Outcomes

  -  Gain experience accessing your operating system's command line interface (CLI)
  -  Gain experience working with CLI commands
  -  Gain experience working with Visual Studio Code (VSCode)
  -  Gain experience writing and executing non-web server Node.js JavaScript code

```

p1-date.js

```rouge

  `/*
    CIT 281 Project 1
    Name: Emily Deng
*/
var weekDays = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
var d = new Date();
var num = d.getDay();
var name = weekDays[num];
console.log(name);`

```

p1-random.js
 
```rouge

  `/*
    CIT 281 Project 1
    Name: Emily Deng
*/

// Returns a random number between min (inclusive) and max (exclusive)
function getRandomInteger(min, max) {
    return Math.floor(Math.random() * (max - min) + min);
}

//Output to the console a string of random length between 5 - 25 characters (range inclusive) in length, that consists of all random lowercase letters from the English alphabet.
function random(length){
    var result = '';
    var characters = 'abcdefghijklmnopqrstuvwxyz';
    var charactersLength = characters.length;
    for (var i = 0; i < length; i++){
        var index = getRandomInteger(0,charactersLength);
        result = result + characters[index];
    }
    return result;
}
console.log(random(getRandomInteger(5,26)));`


```
