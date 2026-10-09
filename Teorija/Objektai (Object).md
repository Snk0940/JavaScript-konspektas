# Objektai (Object)

Objektas – tai duomenų struktūra, sauganti susijusią informaciją `key: value` (raktas: reikšmė) poromis.

### Kūrimo būdai
1. **Object literal** (dažniausias ir rekomenduojamas):
```js
const person = {
  firstName: "Jonas",
  age: 25,
  isEmployed: true,
  greet() {
    console.log(`Labas, aš esu ${this.firstName}`);
  }
};
```
2. **Su `new Object()`**:
3. **Konstruktoriaus funkcija** (senesnis būdas):
```js
function Person(name, age) {
  this.name = name;
  this.age = age;
}
const p1 = new Person("Aistė", 20);
```
4. **Klasės (`class`)** (modernus ES6 būdas):
```js
class Student {
  constructor(name, grade) {
    this.name = name;
    this.grade = grade;
  }
}
const s1 = new Student("Lukas", 10);
```

### Savybių pasiekimas ir keitimas
- Per tašką: `person.firstName`
- Per laužtinius skliaustus: `person["firstName"]` (būtina, jei rakto pavadinimas saugomas kintamajame arba turi tarpų).

### Raktinis žodis `this`
Metodo viduje `this` nurodo į objektą, kuris iškvietė tą metodą.

### Naudingi objektų metodai
- `Object.keys(obj)`: grąžina visų savybių pavadinimų (raktų) masyvą.
- `Object.values(obj)`: grąžina visų reikšmių masyvą.
- `Object.entries(obj)`: grąžina `[raktas, reikšmė]` porų masyvą.
- `Object.assign(target, source)`: nukopijuoja savybes iš vieno objekto į kitą.

### Spread operatorius (...) ir Destruktūrizavimas
```js
// Sujungimas / kopijavimas:
const base = { a: 1, b: 2 };
const extended = { ...base, c: 3 };

// Destruktūrizavimas (išpakavimas į kintamuosius):
const { firstName, age } = person;
console.log(firstName, age); // "Jonas", 25
```

Nuorodos:
- [W3Schools JS Objects](https://www.w3schools.com/js/js_objects.asp)
- [W3Schools JS Object Methods](https://www.w3schools.com/js/js_object_methods.asp)
- [W3Schools JS Classes](https://www.w3schools.com/js/js_classes.asp)
