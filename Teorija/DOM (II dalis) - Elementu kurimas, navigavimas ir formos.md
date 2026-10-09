# DOM (II dalis) – Elementų kūrimas, navigavimas ir formos

### Naujų elementų kūrimas ir įkėlimas į puslapį
1. `document.createElement("tagName")` : sukuria naują elementą atmintyje.
2. `element.append(...nodes)` / `element.appendChild(node)` : prideda elementą į tėvinio elemento pabaigą.
3. `element.prepend(...nodes)` : prideda į pradžią.
4. `element.before(...nodes)` / `element.after(...nodes)` : įterpia prieš arba už elemento.

Pavyzdys:
```js
const list = document.querySelector("#todo-list");
const newItem = document.createElement("li");
newItem.textContent = "Išmokti DOM elementų kūrimą";
newItem.classList.add("item");
list.appendChild(newItem);
```

### Elementų šalinimas
- `element.remove()` : pašalina patį elementą iš puslapio.
- `parent.removeChild(child)` : senesnis būdas pašalinti vaikinį elementą.

### Navigavimas DOM medžiu (Traversing)
- `element.parentElement` : tėvinis elementas.
- `element.children` : visi tiesioginiai vaikiniai elementai (HTMLCollection).
- `element.firstElementChild` / `element.lastElementChild` : pirmas ir paskutinis vaikas.
- `element.nextElementSibling` : sekantis brolinis elementas.
- `element.previousElementSibling` : ankstesnis brolinis elementas.

### Darbas su formomis ir įvestimis
Paimti įvesties reikšmę iš laukelio:
```js
const input = document.querySelector("#username");
console.log(input.value);
```

Formos pateikimo (submit) valdymas ir puslapio perkrovimo sustabdymas:
```js
const form = document.querySelector("#loginForm");

form.addEventListener("submit", (event) => {
  event.preventDefault(); // Sustabdo puslapio persikrovimą
  const data = new FormData(form);
  console.log("Forma pateikta!");
});
```

Nuorodos:
- [W3Schools JS DOM Nodes](https://www.w3schools.com/js/js_htmldom_nodes.asp)
- [W3Schools JS Form Validation](https://www.w3schools.com/js/js_validation.asp)
