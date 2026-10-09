# Loginiai operatoriai

Loginiai operatoriai sujungia arba apverčia logines sąlygas.

### Operatoriai
- `&&` (AND – IR): grąžina `true`, tik jei ABI sąlygos yra teisingos.
- `||` (OR – ARBA): grąžina `true`, jei bent VIENA sąlyga yra teisinga.
- `!` (NOT – NE): apverčia reikšmę (iš `true` padaro `false` ir atvirkščiai).

```js
const age = 20;
const hasId = true;

if (age >= 18 && hasId) {
  console.log("Įeiti galima");
}

const isWeekend = true;
const isHoliday = false;

if (isWeekend || isHoliday) {
  console.log("Poilsio diena");
}

console.log(!hasId); // false
```

### Trumpasis sujungimas (Short-circuit evaluation)
- `&&` sustoja ties pirma `false` (arba falsy) reikšme.
- `||` sustoja ties pirma `true` (arba truthy) reikšme.

Nuorodos:
- [W3Schools JS Logical Operators](https://www.w3schools.com/js/js_comparisons.asp)
