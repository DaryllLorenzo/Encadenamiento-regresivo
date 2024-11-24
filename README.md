# Encadenamiento-regresivo
Este proyecto está diseñado utilizando el lenguaje C, y hace uso de manejo de memoria, estructuras y punteros para implementar el sistema basado en reglas del encadenamiento regresivo.


# Reglas de ejercicio de Ejemplo

## Reglas

- **R1:** A ^ B => C
- **R2:** D ^ E ^ F => G
- **R3:** H ^ I => J
- **R4:** C ^ G => K
- **R5:** G ^ J => L
- **R6:** K ^ L => M

## Meta a alcanzar

**M**

Utilizando un universo cerrado, si no lo conozco asumo que es falso.

## Hechos

Hechos iniciales: `{A, B, D, E, F, L}`

### Proceso para alcanzar M

<img alt="diapo3" src="/imgs/diapo3ER.png"><br>
<img alt="diapo2" src="/imgs/diapo2ER.png"><br>
<img alt="resultado" src="/imgs/EJ1ER.png"><br>

---

## Ejemplo donde no se llega a la meta M

Hechos iniciales: `{D, E, F, L}`

### Resultado

Para llegar a este resultado seria necesario comentar las lineas de 
    //hechos[4] = h5;
    //hechos[5] = h6;
    y ademas por lo tanto reducir el size de hechos a 4

<img alt="resultado" src="/imgs/EJ2ER.png"><br>

---

## Cómo probar con otras reglas

Si desea probar con otras reglas, es necesario modificar el código y adaptarlo a las necesidades, principalmente la función **`node_signo_nodos_forman_regla`**.

---
