# js-random-array
Randomize and return an array in javascript

# use
  let new = array.slice()>br?
  randomize(new)
  
`var randomize = function (array) {`<br>

`// Fisher-Yates (aka Knuth) Shuffle`<br>
`  var currentIndex = array.length,  randomIndex;`<br>

`  // While there remain elements to shuffle...`<br>
`  while (0 !== currentIndex) {`<br>

`    // Pick a remaining element...`<br>
`    randomIndex = Math.floor(Math.random() * currentIndex);`<br>
`    currentIndex--;`<br>

`    // And swap it with the current element.`<br>
`    [array[currentIndex], array[randomIndex]] = [`<br>
`    array[randomIndex], array[currentIndex]];`<br>

`  }`<br>
`  return array;`<br>
`}`<br>
