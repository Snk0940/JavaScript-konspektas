# Kintamieji: let, const ir var

Kintamasis – tai pavadinta vieta kompiuterio atmintyje reikšmei saugoti.

### Kintamųjų deklaravimo būdai
- **let**: naudojamas, kai kintamojo reikšmė programos eigoje keisis. Galioja bloko lygiu `{ }`.
- **const**: naudojamas, kai reikšmės keisti neketinama (konstanta). Galioja bloko lygiu `{ }`.
- **var**: senasis būdas (iki ES6). Turi funkcijos lygio arba globalią galiojimo sritį, nepaiso paprastų blokų `{ }`. Naujame kode nerekomenduojama naudoti.

```js
let score = 0;
score = 1;

const greeting = "Labas";
// greeting = "Viso"; // Klaida: Assignment to constant variable
```

Svarbi taisyklė su `const`:
Nors paties priskyrimo pakeisti negalima, jei kintamajame saugomas **masyvas** arba **objektas**, jo vidinius elementus ar savybes keisti galima.

```js
const numbers = [1, 2, 3];
numbers.push(4); // Leidžiama

const user = { name: "Jonas" };
user.name = "Petras"; // Leidžiama
```

### Kintamųjų vardų taisyklės
- Gali būti naudojamos raidės, skaičiai, `$` ir `_`.
- Pavadinimas negali prasidėti skaičiumi.
- Kelių žodžių pavadinimams naudojamas **camelCase** stilius (pvz., `userName`, `totalCartPrice`).
- Didžiosios ir mažosios raidės skiriasi (`myVar` nėra tas pats kaip `myvar`).
- Negalima naudoti rezervuotų JavaScript žodžių (pvz., `let`, `class`, `function`).

Nuorodos:
- [W3Schools JS Variables](https://www.w3schools.com/js/js_variables.asp)
- [W3Schools JS Let](https://www.w3schools.com/js/js_let.asp)
- [W3Schools JS Const](https://www.w3schools.com/js/js_const.asp)
