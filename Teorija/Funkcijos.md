# Funkcijos

Funkcija – kodo blokas, sukurtas atlikti konkrečią užduotį ir vykdomas tik jį iškvietus.

### Funkcijų tipai

1. **Function declaration**:
```js
function add(a, b) {
  return a + b;
}
```
Galioja hoisting (galima kviesti prieš jos aprašymą).

2. **Function expression**:
```js
const add = function(a, b) {
  return a + b;
};
```

3. **Arrow function** (rodyklinė funkcija):
```js
const add = (a, b) => a + b;
```

### Callback ir Higher-Order funkcijos (HOF)
- **Callback**: funkcija, paduodama į kitą funkciją kaip argumentas.
- **Higher-Order Function**: funkcija, priimanti kitą funkciją arba ją grąžinanti (pvz., `map`, `filter`).

### IIFE (Immediately Invoked Function Expression)
Funkcija, pasileidžianti iš karto po aprašymo:
```js
(function() {
  console.log("Vykdoma iškart");
})();
```

### Vidinės (Nested) funkcijos
Vidinė funkcija mato visus išorinės funkcijos kintamuosius (Closure savybė).

Nuorodos:
- [W3Schools JS Functions](https://www.w3schools.com/js/js_functions.asp)
- [W3Schools JS Arrow Function](https://www.w3schools.com/js/js_arrow_function.asp)
