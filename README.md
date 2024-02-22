# Arquitecturas Css
Curso de Arquitecturas Css.

Necesitamos que css sea.
1. Limpio.
2. Escalable.
3. Mantenible.

Podemos tomar en cuenta los principios de la programación orientada a objetos.
 * Solid.
 * Dry.
 * Immutability.

Arquitectura se refuere como se divide el codigo en archivos y carpetas, Y como trabajamos con nuestros selectores __*Nombramiento de Clases*__.

## Solid.
### S.
 Single Responsability Principle: Una clase debe tener solo una razon para cambiar.

```css
.button {
     border-radius: 2px;
}
.button--secondary {
    background-color: red;
    color: blue;
}
```

```html
<button class='button button--secondary'></button>
```
es esta caso caso cada clase son independentes y complen su funcion sin mezclarse.

---

### O.
Open-Closed principle:Las entidades de software deben estar abiertas para extención, pero cerradas para módificación.


```css
.button {
     border-radius: 2px;
}
.button--secondary {
    @extend .buttom--sm;
    background-color: red;
    color: blue;
}
```
se deben agregar es propiedades paro no deben heredar.

---
### L.
Liskov substitution



