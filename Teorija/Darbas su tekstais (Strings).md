# Darbas su tekstais (Strings)

Tekstas (String) – primityvus duomenų tipas, skirtas simbolių eilutėms saugoti.

### Savybė length ir simbolių pasiekimas
```js
const text = "JavaScript";
console.log(text.length); // 10
console.log(text[0]);     // "J"
console.log(text.charAt(0)); // "J"
```

### Pagrindiniai String metodai
- `toUpperCase()` : paverčia visas raides didžiosiomis.
- `toLowerCase()` : paverčia mažosiomis.
- `trim()` : pašalina tarpus iš teksto pradžios ir pabaigos.
- `includes(sub)` : tikrina, ar tekstas turi nurodytą frazę (grąžina true/false).
- `startsWith(sub)` / `endsWith(sub)` : tikrina pradžią arba pabaigą.
- `indexOf(sub)` : grąžina pirmo sutapimo indeksą (arba -1, jei nerasta).
- `slice(start, end)` : iškerpa ir grąžina teksto dalį.
- `replace(old, new)` : pakeičia pirmą sutapusią frazę kita.
- `replaceAll(old, new)` : pakeičia visus sutapimus.
- `split(separator)` : padalina tekstą į masyvą pagal skirtuką:
```js
const csv = "Jonas,Petras,Antanas";
const names = csv.split(","); // ["Jonas", "Petras", "Antanas"]
```

### Template Literals (Šabloninės eilutės)
Naudojamos atvirkštinės kabutės `` ` ` ``. Leidžia įterpti kintamuosius per `${kintamasis}` ir rašyti tekstą per kelias eilutes be `\n`.

```js
const name = "Lukas";
const greeting = `Sveikas, ${name}!`;
```

Nuorodos:
- [W3Schools JS Strings](https://www.w3schools.com/js/js_strings.asp)
- [W3Schools JS String Methods](https://www.w3schools.com/js/js_string_methods.asp)
- [W3Schools JS Template Literals](https://www.w3schools.com/js/js_string_templates.asp)
