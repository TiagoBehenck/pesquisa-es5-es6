# pesquisa-es5-es6
//ES 6 Const
let a = 1
a = 2

const b = 1
b = 2 // Uncaught SyntaxError "b" is read-only

//ES 6 Parâmetros de funções 
const multiply = (x, y = 1) => x * y

multiply(3, 2) // 6
multiply(3) // 3

//ES6 Arrow functions e Destructing
const sum = (a, b) => {
    return a + b;
}

const [a, b] = [1, 2]

console.log(a) // 1
console.log(b) // 2
const colors = ['red', 'green', 'yellow'];
const [red, green, yellow] = colors;

//ES6 Classes
class Animal {
  constructor(name) {
    this._name = name
  }

  getName() {
    return this._name
  }

  setName(name) {
    this._name = name
  }
}

const animal = new Animal('dog')
animal.getName() // dog
animal.setName('cat')
animal.getName() // cat
