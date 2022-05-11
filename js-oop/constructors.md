# Constructors

A constructor is just a function that by convention starts with a capital letter, that creates objects.

The new keyword is used on constructors to create new objects from it.

## Example

```js
function MakeCar(carMake, carModel, carColor){
    this.make = carMake,
    this.model = carModel,
    this.color = carColor
    this.honk = function(){
    alert("BEEP BEEP")
    }
}

let hondaCivic = new MakeCar("Honda", "Civic", "black);
```

Every Object can look up its prototype chain and inherit properties from the prototypes all the way up to the global object prototype.

## Class syntax

```js
class MakeCar {
  constructor(carMake, carModel, carColor) {
    this.make = carMake, this.model = carModel, this.carColor = carColor,
  }
  lock() {
    alert("locked the doors");
  }
}

let hondaCivic = new MakeCar("honda", "civic", "silver", 4);
```
