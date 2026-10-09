# Sąlygos sakinys if, else if, else

Sąlygos sakinys vykdo atitinkamą kodo bloką tik tada, kai sąlyga yra teisinga (`true`).

```js
const score = 75;

if (score >= 90) {
  console.log("Įvertinimas: Puikiai");
} else if (score >= 70) {
  console.log("Įvertinimas: Gerai");
} else if (score >= 50) {
  console.log("Įvertinimas: Patenkinamai");
} else {
  console.log("Egzaminas neišlaikytas");
}
```

### Ternary operatorius (? :)
Trumpas sąlygos užrašymas vienoje eilutėje: `sąlyga ? jei_true : jei_false`
```js
const status = score >= 50 ? "Išlaikyta" : "Neišlaikyta";
```

### Truthy ir Falsy reikšmės
JavaScript sąlygose bet kokia reikšmė paverčiama į `true` arba `false`.

**Falsy reikšmės (tik 6):**
- `false`
- `0`
- `""` (tuščia eilutė)
- `null`
- `undefined`
- `NaN`

Visos kitos reikšmės (įskaitant `[]` ir `{}`) yra **truthy**.

### Optional chaining (?.)
Saugus giliau esančių savybių pasiekimas:
```js
const user = { name: "Tomas" };
console.log(user.address?.city); // undefined (vietoj to, kad mestų klaidą)
```

Nuorodos:
- [W3Schools JS If Else](https://www.w3schools.com/js/js_if_else.asp)
