# Ciklai (Loops)

Ciklai naudojami pasikartojančiam kodo blokui vykdyti tam tikrą skaičių kartų.

### Ciklų rūšys

1. **for ciklas**:
Naudojamas, kai iš anksto žinoma, kiek kartų ciklas turi suktis.
```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

2. **while ciklas**:
Vykdomas tol, kol sąlyga yra teisinga (`true`). Naudojamas, kai iteracijų skaičius iš anksto nežinomas.
```js
let count = 0;
while (count < 3) {
  console.log(count);
  count++;
}
```

3. **do...while ciklas**:
Kodo blokas įvykdomas bent vieną kartą, ir tik tada tikrinama sąlyga.
```js
let num = 0;
do {
  console.log(num);
  num++;
} while (num < 0); // Atspausdins 0 ir sustos
```

4. **for...of ciklas**:
Skirtas iteruoti per masyvus ir kitas iteruojamas struktūras (paima elementų reikšmes):
```js
const colors = ["raudona", "žalia", "mėlyna"];
for (const color of colors) {
  console.log(color);
}
```

5. **for...in ciklas**:
Skirtas iteruoti per objekto savybių pavadinimus (raktus):
```js
const car = { brand: "Audi", year: 2020 };
for (const key in car) {
  console.log(`${key}: ${car[key]}`);
}
```

### Ciklo valdymo komandos
- **break**: pilnai nutraukia ciklo vykdymą.
- **continue**: praleidžia esamą iteraciją ir pereina prie sekančios.

Nuorodos:
- [W3Schools JS For Loop](https://www.w3schools.com/js/js_loop_for.asp)
- [W3Schools JS While Loop](https://www.w3schools.com/js/js_loop_while.asp)
- [W3Schools JS For In / For Of](https://www.w3schools.com/js/js_loop_forin.asp)
