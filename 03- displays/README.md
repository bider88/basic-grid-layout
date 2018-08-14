### Definiedo las columnas
- Para usar grid layout hay que poner el ```display: grid``` en el contenedor padre.
- Podemos tener subgrids dentro un grid agregando el siguiente código de ejemplo:
```
.item:nth-of-type(4) {
    background: blueviolet;
    overflow: auto;
    /* display: subgrid; */
    /* display: inline-grid; */
    display: grid;
    grid-template: 50px 50px 50px / 200px 200px 200px;
}
.item .item {
    background: yellowgreen;
}
```
Con **nth-of-type({numb})** especifícamos el número de item que deseamos modificar con estilos y colocar los demás elementos dentro de él.