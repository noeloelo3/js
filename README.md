# parzystosc
```js
const pyt = window.prompt("podaj liczbe")
const liczba = Number(pyt)
if (liczba % 2 == 0)
    window.alert("liczba parzysta")
else
    window.alert("nieparzysta")
```

# przedzial
```js
const pyt = window.prompt("liczba dawaj")
const liczba = Number(pyt)
if (liczba > 5 && liczba < 20)
    window.alert("miesci sie")
else
    window.alert("chuuuja")
```




# kalkulator1
```js
const pyt1 = window.prompt("piersza liczba")
const pyt2 = window.prompt("druga liczba")
const znak = window.prompt("znak")
const liczba1 = Number(pyt1)
const liczba2 = Number(pyt2)
switch (znak) {
    case '*':
        window.alert("wynik to: " + liczba1 * liczba2)
        break
    case '/':
        if (liczba2 == 0)
            window.alert("cozadebil")
        else
            window.alert("wynik to: " + liczba1 / liczba2)
        break
    case '+':
        window.alert("wynik to: " + liczba1 + liczba2)
        break
    case '-':
        window.alert("wynik to: " + liczba1 - liczba2)
        break
}
 ```




# nadpisanie diva
```js
const pier = document.querySelector('#jeden')
const nap = window.prompt("napisz cos ok")
pier.innerHTML = `<span>${nap}</span>`
 ```









# kalkulator divovy
```js
const pier = document.querySelector('#jeden')
const pyt1 = window.prompt("piersza liczba")
const pyt2 = window.prompt("druga liczba")
const znak = window.prompt("znak")
const liczba1 = Number(pyt1)
const liczba2 = Number(pyt2)
switch (znak) {
    case '*':
        pier.innerHTML = ("wynik to: " + liczba1 * liczba2)
        pier.classList.add("mnozenie")
        break
    case '/':
        if (liczba2 == 0)
            pier.innerHTML = ("cozadebil")
        else
            pier.innerHTML = ("wynik to: " + liczba1 / liczba2)
        pier.classList.add("dzielenie")
        break
    case '+':
        pier.innerHTML = ("wynik to: " + liczba1 + liczba2)
        pier.classList.add("dodawanie")
        break
    case '-':
        pier.innerHTML = ("wynik to: " + liczba1 - liczba2)
        pier.classList.add("odejmowanie")
        break
}
```








# zmiana koloru
```js
window.alert("kolorki: red, green, blue, yellow, purple")
const kolor = window.prompt("kolorek")


const zmiana = document.querySelector("body")

switch (kolor) {
    case 'red':
        zmiana.style.backgroundColor = "red"
        break
    case 'green':
        zmiana.style.backgroundColor = "green"
        break
    case 'blue':
        zmiana.style.backgroundColor = "blue"
        break
    case 'yellow':
        zmiana.style.backgroundColor = "yellow"
        break
    case 'purple':
        zmiana.style.backgroundColor = "purple"
        break
    default:
        zmiana.style.backgroundColor = "white"
        break
}
 ```






# licznik
```js
let liczba = 0
const pls = document.querySelector('#plus')
const mns = document.querySelector('#minus')
const lcz = document.querySelector('#liczby')
const rst = document.querySelector('#reset')


function plus() {
    lcz.innerHTML = `${++liczba}`
    if (liczba > 0)
        lcz.style.color = "green"
    else if (liczba == 0)
        lcz.style.color = "black"

}
pls.addEventListener('click', plus)

function minus() {

    lcz.innerHTML = `${--liczba}`
    if (liczba < 0)
        lcz.style.color = "red"
    else if (liczba == 0)
        lcz.style.color = "black"

}
mns.addEventListener('click', minus)

function reset() {
    liczba = 0
    lcz.innerHTML = 0
    lcz.style.color = 'black'

}
rst.addEventListener('click', reset)
 ```







# zgodnosc haselek
```js
const h1 = document.querySelector('#has1')
const h2 = document.querySelector('#has2')
const span = document.querySelector('span')

function jaja() {
    const c = h1.value === h2.value
    if (c) {
        span.innerHTML = "zgadza sie"
        span.style.color = "green"
    }
    else {
        span.innerHTML = "hasla roznia sie"
        span.style.color = "red"
    }
}

h2.addEventListener('input', jaja)
 ```
