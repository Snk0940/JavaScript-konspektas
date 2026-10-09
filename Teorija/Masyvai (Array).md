# Masyvai (Array)

Masyvas – tai kintamasis, kuriame saugomas tvarkingas sąrašas reikšmių (elementų). Elementai pasiekiami pagal indeksus, pradedant nuo `0`.

### Masyvo kūrimas
```js
const fruits = ["Obuolys", "Bananas", "Kriaušė"];
console.log(fruits[0]); // "Obuolys"
console.log(fruits.length); // 3
```

Masyvai atmintyje saugomi per nuorodą (reference). Nukopijavus kintamąjį, abu kintamieji rodo į tą patį masyvą.

### Spread (...) operatorius ir kopijavimas
Norint padaryti tikrą masyvo kopiją:
```js
const original = [1, 2, 3];
const copy = [...original];
const combined = [...original, 4, 5];
```

### Pagrindiniai masyvų metodai

#### Elementų pridėjimas ir šalinimas
- `push(elem)`: prideda elementą į masyvo galą.
- `pop()`: pašalina paskutinį elementą ir jį grąžina.
- `unshift(elem)`: prideda elementą į masyvo pradžią.
- `shift()`: pašalina pirmą elementą ir jį grąžina.

#### slice() ir splice()
- `slice(start, end)`: nukopijuoja dalį masyvo į naują masyvą (originalo nekeičia).
- `splice(start, deleteCount, ...items)`: redaguoja originalų masyvą – gali ištrinti, pakeisti arba įterpti elementus.

#### Iteravimo ir transformavimo metodai
- **forEach(callback)**: atlieka veiksmą su kiekvienu elementu, nieko negrąžina:
```js
fruits.forEach((fruit, index) => {
  console.log(`${index}: ${fruit}`);
});
```

- **map(callback)**: sukuria naują masyvą transformuodamas kiekvieną elementą:
```js
const numbers = [1, 2, 3];
const doubled = numbers.map(n => n * 2); // [2, 4, 6]
```

- **filter(callback)**: sukuria naują masyvą tik su tais elementais, kurie tenkina sąlygą:
```js
const evens = numbers.filter(n => n % 2 === 0); // [2]
```

- **find(callback)**: grąžina pirmą elementą, atitinkantį sąlygą (arba undefined):
```js
const found = numbers.find(n => n > 1); // 2
```

- **sort(callback)**: rikiuoja masyvą vietoje.
```js
// Skaičių rikiavimas didėjimo tvarka:
numbers.sort((a, b) => a - b);
// Mažėjimo tvarka:
numbers.sort((a, b) => b - a);
```

- **reduce(callback, initialValue)**: sutraukia visą masyvą į vieną reikšmę (pvz., sumą):
```js
const sum = numbers.reduce((acc, curr) => acc + curr, 0);
```

Nuorodos:
- [W3Schools JS Arrays](https://www.w3schools.com/js/js_arrays.asp)
- [W3Schools JS Array Methods](https://www.w3schools.com/js/js_array_methods.asp)
- [W3Schools JS Array Iteration](https://www.w3schools.com/js/js_array_iteration.asp)
