# tambola-generator
A library for generating tambola tickets and the draw sequence

## Installation
We use **npm** for dependency management, run

```shell
npm install --save https://github.com/rishiwadhwani/tambola-generator/tarball/master
```

## Usage
In your NodeJS application, require the module:
```shell
var tambola = require('tambola-generator');
```

To get tickets, use the getTickets(count) method:
```shell
tambola.getTickets(100) //This generates 100 tambola tickets
```

To get the draw sequence, use the getDrawSequence() method:
```shell
tambola.getDrawSequence() //Returns numbers 1-90 scrambled
```

## JSON
```shell
// Tickets array
[
  [
    [0,18,23,30,40,0,0,0,80],
    [5,0,0,0,42,52,0,75,87],
    [0,0,20,0,49,58,65,0,90]
  ],
  [
    [0,10,21,34,0,52,0,0,83],
    [0,11,0,36,41,0,0,72,85],
    [9,0,26,37,43,0,67,0,0]
  ]
]
```
```shell
// Draw Sequence
[72,65,47,89,42,4,61,84,36,22,37,18,9,27,
12,71,46,15,30,55,17,3,56,25,68,80,43,26,
50,39,53,38,60,31,28,11,8,62,49,79,51,35,
14,67,45,41,40,5,44,34,73,32,86,69,70,48,
21,33,83,13,54,77,78,90,29,6,52,59,58,66,
76,1,10,24,19,64,85,7,74,2,16,63,88,23,57
,87,81,82,20,75]
```
