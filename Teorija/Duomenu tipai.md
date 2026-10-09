# Duomenų tipai ir jų keitimas

JavaScript yra dinamiškai tipizuojama kalba – kintamajam nereikia iš anksto nurodyti tipo, tipas nustatomas automatiškai pagal priskirtą reikšmę.

### Primityvūs duomenų tipai
- **Number**: skaičiai (sveikieji ir dešimtainiai), taip pat specialios reikšmės `Infinity`, `-Infinity`, `NaN` (Not a Number).
- **String**: teksto eilutės, rašomos viengubose `' '`, dvigubose `" "` arba atvirkštinėse `` ` ` `` kabutėse.
- **Boolean**: loginė reikšmė, turinti tik dvi būsenas: `true` arba `false`.
- **Undefined**: kintamasis yra deklaruotas, bet jam dar nepriskirta jokia reikšmė.
- **Null**: speciali reikšmė, reiškianti „nieko“, „tuščia“ arba „reikšmė nežinoma“.
- **Symbol**: unikalus nekintamas identifikatorius.
- **BigInt**: dideliems sveikiesiems skaičiams, viršijantiems Number limitą.

### Tipų tikrinimas: typeof
```js
typeof 42;          // "number"
typeof "tekstas";   // "string"
typeof true;        // "boolean"
typeof undefined;   // "undefined"
typeof null;        // "object" (istorinė JS klaida)
typeof {};          // "object"
typeof [];          // "object"
```

### Duomenų tipų keitimas (Type Conversion)

#### 1. Automatinis keitimas (Implicit)
- Su `+` operatoriumi, jei bent viena pusė tekstas, skaičius paverčiamas tekstu: `"5" + 2` tampa `"52"`.
- Su matematiniais operatoriais `-`, `*`, `/` tekstas automatiškai paverčiamas skaičiumi: `"5" - 2` tampa `3`.

#### 2. Rankinis keitimas (Explicit)
- **Į skaičių**:
  - `Number("123")` -> `123`
  - `Number("123px")` -> `NaN`
  - `parseInt("123px")` -> `123` (išskiria sveikąjį skaičių nuo pradžios)
  - `parseFloat("3.14m")` -> `3.14` (išskiria dešimtainį skaičių)
- **Į tekstą**:
  - `String(123)` -> `"123"`
  - `(123).toString()` -> `"123"`
- **Į loginę reikšmę (Boolean)**:
  - `Boolean(1)` -> `true`
  - `Boolean(0)` -> `false`

Nuorodos:
- [W3Schools JS Data Types](https://www.w3schools.com/js/js_datatypes.asp)
- [W3Schools JS Type Conversion](https://www.w3schools.com/js/js_type_conversion.asp)
