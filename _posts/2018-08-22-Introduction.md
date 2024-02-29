---
layout: post
author: ted
---
Kiwifruit (often abbreviated as kiwi), or Chinese gooseberry is the
edible berry of several species of woody vines in the genus Actinidia.

The most common cultivar group of kiwifruit is oval, about the size of
a large hen's egg (5–8 cm (2.0–3.1 in) in length and 4.5–5.5 cm
(1.8–2.2 in) in diameter). It has a fibrous, dull greenish-brown skin
and bright green or golden flesh with rows of tiny, black, edible
seeds. The fruit has a soft texture, with a sweet and unique flavor.

```js
function setup() {
  // Set simulation framerate to 10 to avoid flickering
  frameRate(10);
  var canvas = createCanvas(720, 400);
  canvas.parent('gameoflife');
  w = 20;
  // Calculate columns and rows
  columns = floor(width / w);
  rows = floor(height / w);
  // Wacky way to make a 2D array is JS
  board = new Array(columns);
  for (let i = 0; i < columns; i++) {
    board[i] = new Array(rows);
  }
  // Going to use multiple 2D arrays and swap them
  next = new Array(columns);
  for (i = 0; i < columns; i++) {
    next[i] = new Array(rows);
  }
  init();
}
```

<div id="gameoflife"><script src="/assets/js/gameoflife.js"></script></div>
