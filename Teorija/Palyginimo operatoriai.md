# Palyginimo operatoriai

Palyginimo operatoriai naudojami reikšmėms palyginti ir grąžina loginę reikšmę: `true` arba `false`.

### Operatoriai
- `===` : griežtas lygu (tikrina ir reikšmę, ir duomenų tipą).
- `!==` : griežtas nelygu (tikrina ir reikšmę, ir tipą).
- `==` : negriežtas lygu (prieš lygindamas automatiškai konvertuoja tipus; nerekomenduojama).
- `!=` : negriežtas nelygu.
- `>` : daugiau.
- `<` : mažiau.
- `>=` : daugiau arba lygu.
- `<=` : mažiau arba lygu.

```js
5 === 5;    // true
5 === "5";  // false (skirtingi tipai: number ir string)
5 == "5";   // true (atlieka automatinį konvertavimą)
10 > 5;     // true
```

Taisyklė: profesionaliame kode visada rekomenduojama naudoti `===` ir `!==`, kad išvengtumėte paslėptų klaidų dėl tipų konvertavimo.

Nuorodos:
- [W3Schools JS Comparisons](https://www.w3schools.com/js/js_comparisons.asp)
