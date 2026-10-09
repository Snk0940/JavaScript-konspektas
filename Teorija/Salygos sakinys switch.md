# Sąlygos sakinys switch

`switch` naudojamas, kai vieną kintamąjį reikia palyginti su keliomis konkrečiomis reikšmėmis (`case`).

```js
const day = 3;

switch (day) {
  case 1:
    console.log("Pirmadienis");
    break;
  case 2:
    console.log("Antradienis");
    break;
  case 3:
    console.log("Trečiadienis");
    break;
  default:
    console.log("Nežinoma diena");
    break;
}
```

### Svarbios taisyklės
- `switch` naudoja griežtąjį palyginimą (`===`).
- **break**: būtinas po kiekvieno atvejo, kitaip kodas vykdysis toliau per kitus `case`.
- **default**: veikia kaip atsarginis variantas (analogas `else`).

Nuorodos:
- [W3Schools JS Switch](https://www.w3schools.com/js/js_switch.asp)
