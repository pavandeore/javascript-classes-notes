# javascript-classes-notes

1] Getting Started

```
class Rectangle{
  constructor(_width, _height, _color){
    console.log('rectangle created')
    
    this.width = _width;
    this.height = _height;
    this.color = _color;
  }
  
  getArea(){
    return this.width * this.height
  }
  
  printDescription(){
    return('i am rectangle with '+ this.width)
  }
  
}

let rect1 = new Rectangle(6,5,'blue')
let rect2 = new Rectangle(100, 4, 'abg')

console.log(rect1.getArea())
console.log(rect2.getArea())
console.log(rect2.printDescription())

```

2] Getters and Setters

```

// Getters and Setters 
// used to define methods on class and then use it is a property 
// essentially they look like methods but they are peoperty of those class

class Square{
  constructor(_width){
    this.width = _width;
    this.height = _width;
  }
  
  get area(){
    return this.width * this.height
  }
  set area(area){
    this.width = Math.sqrt(area);
  }
  
}

let sq1 = new Square(3)

sq1.area = 30

console.log(sq1.area)


```

3] Static Methods

```
// static methods
// it is a method called on class but is not a part of obj 
// basically call methods without creating objs mostly used for performance and utlity 


class Square{
  constructor(_width){
    this.width = _width
  }
  
  static equal(a,b){
    return a===b
  }
  
}

let squ1 = new Square(8)
let squ2 = new Square(10)


console.log(Square.equal(3,3))
```




