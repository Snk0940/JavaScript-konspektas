# Datos (Date)

Objektas `Date` naudojamas darbui su data ir laiku.

### Datos kūrimas
```js
// Dabartinė data ir laikas:
const now = new Date();

// Iš nurodyto teksto:
const d1 = new Date("2026-10-09");

// Iš parametrų (metai, mėnuo nuo 0 iki 11, diena, valanda, min):
const d2 = new Date(2026, 9, 9, 14, 30); // 9 yra Spalis!
```

### Timestamp
Timestamp – milisekundžių skaičius nuo 1970 m. sausio 1 d. 00:00:00 UTC.
- `Date.now()` : dabartinis timestamp.
- `date.getTime()` : konkrečios datos timestamp.

### Metodai informacijai gauti
- `getFullYear()` : 4 skaitmenų metai.
- `getMonth()` : mėnuo (0-11: 0 = Sausis, 11 = Gruodis).
- `getDate()` : mėnesio diena (1-31).
- `getDay()` : savaitės diena (0-6: 0 = Sekmadienis).
- `getHours()`, `getMinutes()`, `getSeconds()`.

### Metodai datai keisti
- `setFullYear(year)`
- `setMonth(month)`
- `setDate(day)`

### Datų palyginimas
Datos gali būti tiesiogiai lyginamos su operatoriais `>`, `<`, `>=`, `<=`:
```js
const d1 = new Date("2026-01-01");
const d2 = new Date("2026-05-01");
console.log(d2 > d1); // true
```

Nuorodos:
- [W3Schools JS Dates](https://www.w3schools.com/js/js_dates.asp)
- [W3Schools JS Date Methods](https://www.w3schools.com/js/js_date_methods.asp)
