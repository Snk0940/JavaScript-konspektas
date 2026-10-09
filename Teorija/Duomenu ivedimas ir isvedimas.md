# Duomenų įvedimas ir išvedimas

Naršyklės suteikia bazinius metodus dialogams ir informacijos išvedimui.

### 1. alert()
Parodo informacinį pranešimo langelį su mygtuku OK:
```js
alert("Veiksmas atliktas sėkmingai!");
```

### 2. prompt()
Parodo teksto įvesties langelį.
- Vartotojui įvedus tekstą ir paspaudus OK, grąžinamas įvestas tekstas (`string` tipas).
- Paspaudus Cancel arba Esc, grąžinama reikšmė `null`.

```js
const userName = prompt("Koks tavo vardas?", "Svečias");
console.log(userName);

// Įvestos reikšmės konvertavimas į skaičių:
const age = Number(prompt("Kiek tau metų?"));
```

### 3. confirm()
Parodo klausimą su mygtukais OK ir Cancel.
- Paspaudus OK, grąžina `true`.
- Paspaudus Cancel, grąžina `false`.

```js
const confirmed = confirm("Ar tikrai norite ištrinti failą?");
if (confirmed) {
  console.log("Ištrinta");
}
```

### 4. console metodai (kūrėjų konsolė)
- `console.log()`: standartinis informacijos išvedimas.
- `console.error()`: klaidos pranešimas.
- `console.warn()`: įspėjimas.
- `console.table()`: atvaizduoja masyvus ar objektus tvarkingu formatu.

Nuorodos:
- [W3Schools JS Popup Boxes](https://www.w3schools.com/js/js_popup_boxes.asp)
