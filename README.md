# java-3


const person = { name: "홍길동", age: 25 };


const car = { brand: "Toyota", model: "Corolla" };
console.log(car.brand);


const personAlice = {
  name: "Alice",
  sayHello: function() {
    console.log("Hello, I am " + this.name + ".");
  }
};
personAlice.sayHello();


const personBob = { name: "Bob" };
personBob.greet = function() {
  console.log(`Hi, I'm ${this.name}`);
};
personBob.greet();


function Person(name, age) {
  this.name = name;
  this.age = age;
}
const john = new Person("John", 30);


const people = [
  { name: "John", age: 17 },
  { name: "Jane", age: 20 },
  { name: "Paul", age: 15 },
  { name: "Mark", age: 25 }
];
const adults = people.filter(person => person.age >= 18);
console.log(adults);


const fruits = ["Apple", "Banana", "Orange"];


console.log(fruits[1]);

const numbers = [1, 2, 3, 4];
numbers.push(5);
console.log(numbers);


const colors = ["Red", "Green", "Blue"];
colors.pop();
console.log(colors);

const days = ["Monday", "Tuesday", "Wednesday"];
days.shift();
console.log(days);


const names = ["Bob", "Charlie"];
names.unshift("Alice");
console.log(names);


const numbers2 = [1, 2, 3];
numbers2.forEach(num => console.log(num));


const doubled = numbers.map(num => num * 2);
console.log(doubled);


const ages = [12, 18, 20, 14, 25];
const adultsAges = ages.filter(age => age >= 18);
console.log(adultsAges);


const prices = [10, 20, 30, 40];
const total = prices.reduce((sum, price) => sum + price, 0);
console.log(total);


console.log(fruits.includes("Banana"));


const unsortedNumbers = [5, 2, 8, 1, 3];
unsortedNumbers.sort((a, b) => a - b);
console.log(unsortedNumbers);


const letters = ["a", "b", "c", "d"];
letters.reverse();
console.log(letters);


const animals = ["Cat", "Dog", "Elephant", "Lion"];
const slicedAnimals = animals.slice(0, 2);
console.log(slicedAnimals);


fruits.splice(1, 0, "Strawberry");
console.log(fruits);

const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];
const combinedArr = arr1.concat(arr2);
console.log(combinedArr);

const products = [
  { name: "Shirt", price: 50 },
  { name: "Shoes", price: 120 },
  { name: "Hat", price: 80 }
];
const expensiveProduct = products.find(product => product.price >= 100);
console.log(expensiveProduct);

const allEven = numbers.every(num => num % 2 === 0);
console.log(allEven);

const isAnyoneOver21 = ages.some(age => age >= 21);
console.log(isAnyoneOver21);

const hasDuplicates = numbers.some((num, index) => numbers.indexOf(num) !== index);
console.log(hasDuplicates);

const people2 = [
  { name: "John", age: 30 },
  { name: "Jane", age: 25 },
  { name: "Mark", age: 35 }
];
people2.sort((a, b) => a.age - b.age);
console.log(people2);

const index = ages.findIndex(age => age >= 21);
console.log(index);

const words = ["Hello", "World", "JavaScript"];
const sentence = words.join(", ");
console.log(sentence);

const nestedArray = [[1, 2], [3, 4], [5, [6, 7]]];
const flatArray = nestedArray.flat(2);
console.log(flatArray);
 
