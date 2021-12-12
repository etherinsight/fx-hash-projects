```js
function setup() {
  const size=1000
  createCanvas(size, size);	
   
	background(2);
  const cars = ["BMW", "Volvo", "Saab", "Ford", "Fiat", "Audi"];

  


for (let i = 0; i < cars.length*10; i++) {
  
  

   const size=1000
  ellipse(Math.floor(Math.random() * size+100), Math.floor(Math.random() * size+10), Math.floor(Math.random() * size), Math.floor(Math.random() * size)); // ellipse(x, y, width, height)
  
  polygon(100,100,60);

}

function polygon(x, y, radius, npoints) {
  let angle = TWO_PI / npoints;
  beginShape();
  for (let a = 0; a < TWO_PI; a += angle) {
    let sx = x + cos(a) * radius;
    let sy = y + sin(a) * radius;
    vertex(sx, sy);
  }
  endShape(CLOSE);
}


}

```
