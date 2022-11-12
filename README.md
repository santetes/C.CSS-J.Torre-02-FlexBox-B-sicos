# C.CSS-J.Torre-02-FlexBox-Basicos
- [Enlace](https://santetes.github.io/C.CSS-J.Torre-02-FlexBox-Basicos/) para ver el resultado del ejercicio

```css
:root {
    --azul: #0071b7;
    --blanco: #FFF;
    --naranja: #ff4f1e;
}
html {
    font-size: 62.5%; /** 1REM = 10pX **/
    box-sizing: border-box;
}
*, *:before, *:after {
    box-sizing: inherit;
}
  

body {
    background-color: var(--azul);
    font-family:  'Lato', sans-serif;
    font-size: 1.6rem;
}

h1, h2 {
    color: var(--blanco);
    text-align: center;
    margin: 5rem 0;
    padding: 1rem;
}
.caja-curso {
    background-color: var(--naranja);
    text-align: center;
    color: var(--blanco);
    padding: 5rem;

}
.caja-curso h1 {
    margin: 0;
}
.caja-curso p {
    font-size: 2.4rem;
}
.caja-curso a {
    font-size: 2.4rem;
    padding: 2rem;
    display: inline-block;
    text-decoration: none;
    color: var(--blanco);
    padding: 0;
}


.contenedor {
    max-width: 120rem;
    margin: 0 auto;
}
.box {
    background-color: var(--naranja);
    color: var(--blanco);
    padding: 5rem;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 4rem;
    border: 1rem solid #bb2b03;
}

.contenedor > div {
    background-color: var(--blanco);
    padding: 5rem;
}

/* 1 */
.d-flex{
    display: flex;
}

/* 2 */
.d-flex-2{
    display: flex;
    flex-direction: column;
}

/* 3 */
.d-flex-3{
    display: flex;
    justify-content: space-around;
}

/* 4 */
.d-flex-4{
    display: flex;
    flex-direction: column;
    height: 1000px;
    justify-content: space-around;
    
}

/* 5 */
.d-flex-5{
    display: flex;
    height: 500px;
    align-items: center;
}

/* 6 */
.d-flex-6{
    display: flex;
    flex-direction: column;
    align-items: center;
}

/* 7 */
.d-flex-7{
    display: flex;
    height: 700px;
    align-items: flex-end;
    justify-content: space-around;
}

/* 8 */
.d-flex-8{
    display: flex;
}

.d-flex-8 .box{
    flex-basis: 33.3%;
}

/* .d-flex-8 .box:nth-child(1){
    flex-basis: 33.3%;
} */


/* 9 */
/* Se realiza con nuevas características CSS (gap) */
/* .d-flex-9{
    display: flex;
    gap: 2rem;
}

.d-flex-9 .box{
    flex-basis: 33.3%;
} */

/* Sin gap */
.d-flex-9{
    display: flex;
    justify-content: space-between
}

.d-flex-9 .box{
    flex-basis: calc(33.3% - 1rem);
}

/* 10 */
.d-flex-10{
    display: flex;
    flex-wrap: wrap;
}

.d-flex-10 .box{
    flex-basis: 33.3%
}

/* 11 */

.d-flex-11{
    display: flex;
}

.d-flex-11 .box:nth-child(1){
    flex-grow: 2;
}

.d-flex-11 .box:nth-child(2),
.d-flex-11 .box:nth-child(3){
    flex-grow: 1;
}

/* 12 */

.d-flex-12{
    display: flex;
}

.d-flex-12 .box{
    flex-grow: 1;
    flex-basis: 300px;
   
}

.d-flex-12 .box:nth-child(3){
    flex-shrink: 2;
}

/* 13 */

.d-flex-13{
    display: flex;
}

.d-flex-13 .box{
    flex-basis: 33.3%;
    flex-grow: 1;
    flex-shrink: 1;
 
    /* Esto es lo mismo que: */
    flex: 1 1 33.3%
}
```
