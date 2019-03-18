# pesquisa-es5-es6
<h3>ES 6 Const</h3>
<pre>
let a = 1
a = 2
</pre>
const b = 1
b = 2 // Uncaught SyntaxError "b" is read-only

<h3>ES 6 Parâmetros de funções</h3>
<pre>
const multiply = (x, y = 1) => x * y

multiply(3, 2) // 6
multiply(3) // 3
</pre>

<h3>ES6 Arrow functions e Destructing<h3>
<pre>
const sum = (a, b) => {
    return a + b;
}

const [a, b] = [1, 2]

console.log(a) // 1
console.log(b) // 2
const colors = ['red', 'green', 'yellow'];
const [red, green, yellow] = colors;
</pre>
<h3>ES6 Classes</h3>
<pre>
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
</pre>
