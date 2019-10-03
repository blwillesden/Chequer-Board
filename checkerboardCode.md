// Chequer-Board
//Checkerboard Project


let boardSize = 400
let sqCount = 8
let color1 = "#FF0000"
let color2 = "#000000"

function setup() {
  createCanvas(boardSize, boardSize);

}

function draw() {
  background(220);
  let size = boardSize / sqCount

  for (let r = 0; r <= 15; r++) {
    for (let c = 0; c <= 15; c++) {
      if (r % 2 === 0) {
        if (c % 2 === 0) {
          fill(color2);
        } else {
          fill(color1);
        }
      } else {
        if (c % 2 === 1) {
          fill(color2)
        } else {
          fill(color1)
        }
      }
      rect(c * size, r * size, size, size)
    }
  }

}
