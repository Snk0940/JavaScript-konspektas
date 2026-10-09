# DOM (I dalis) – Elementų paieška, stiliai ir įvykiai

DOM (*Document Object Model*) – tai HTML dokumento objektinis modelis, leidžiantis JavaScript pasiekti ir keisti puslapio struktūrą, stilių bei turinį.

### Elementų paieška dokumente
- `document.getElementById("id")` : suranda vieną elementą pagal id.
- `document.querySelector("selector")` : suranda pirmą elementą pagal CSS selektorių (pvz., `.klase`, `#id`, `div > p`).
- `document.querySelectorAll("selector")` : suranda visus atitinkančius elementus (grąžina NodeList).
- `document.getElementsByClassName("class")` : suranda pagal klasę (grąžina HTMLCollection).
- `document.getElementsByTagName("tag")` : suranda pagal žymės pavadinimą.

### Turinio keitimas
- `element.textContent = "Naujas tekstas"` : saugiai keičia gryną tekstą.
- `element.innerHTML = "<strong>Formatas</strong>"` : keičia HTML kodą elemento viduje.

### Atributų valdymas
- `element.getAttribute("name")` : gauna atributo reikšmę.
- `element.setAttribute("name", "value")` : nustato arba pakeičia atributą.
- `element.hasAttribute("name")` : tikrina, ar atributas egzistuoja.
- `element.removeAttribute("name")` : pašalina atributą.

### Stiliaus savybių (CSS) keitimas
CSS savybės rašomos per `style` savybę, naudojant **camelCase** (be brūkšnelių):
```js
const box = document.querySelector(".box");
box.style.backgroundColor = "royalblue";
box.style.fontSize = "20px";
box.style.display = "none";
```

### Klasių valdymas (classList)
- `element.classList.add("active")` : prideda klasę.
- `element.classList.remove("active")` : pašalina klasę.
- `element.classList.toggle("active")` : prideda, jei nėra, arba pašalina, jei yra.
- `element.classList.contains("active")` : patikrina, ar turi klasę.

### Įvykių klausymas (EventListeners)
Modernus ir rekomenduojamas būdas reaguoti į vartotojo veiksmus:
```js
const btn = document.querySelector("#myButton");

btn.addEventListener("click", (event) => {
  console.log("Mygtukas paspaustas!");
  console.log("Paspaustas elementas:", event.target);
});
```

Dažniausi įvykiai: `click`, `change`, `input`, `submit`, `mouseover`, `mouseout`, `focus`, `blur`, `DOMContentLoaded`.

Nuorodos:
- [W3Schools JS HTML DOM](https://www.w3schools.com/js/js_htmldom.asp)
- [W3Schools JS DOM Elements](https://www.w3schools.com/js/js_htmldom_elements.asp)
- [W3Schools JS DOM EventListener](https://www.w3schools.com/js/js_htmldom_eventlistener.asp)
