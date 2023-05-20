# javascript-classes-notes

1] 

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
