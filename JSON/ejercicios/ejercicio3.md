# Ejercicio 3 — Número vs. texto

## Contexto
Tenemos el siguiente objeto JSON:
```json
{
  "producto": "Ordenador",
  "precio": "1200",
  "stock": 15
}
```

---

## Solución al Cuestionario

1. **¿Qué tipo de dato tiene precio?**
   * **Respuesta:** Tiene tipo de dato **String** (cadena de texto). Se identifica porque el valor está envuelto entre comillas (`"1200"`).

2. **¿Qué tipo de dato tiene stock?**
   * **Respuesta:** Tiene tipo de dato **Number** (específicamente un número entero o *integer*). Se identifica porque el valor numérico no lleva comillas (`15`).

3. **¿Son del mismo tipo?**
   * **Respuesta:** **No**. Aunque `"1200"` representa un valor numérico visualmente, para el sistema es una secuencia de caracteres de texto (String). Por lo tanto, no se pueden realizar operaciones matemáticas directas con él sin antes convertirlo, a diferencia de `stock` que ya es un número nativo.

---

## JSON Modificado
Para que `precio` sea un número en lugar de un texto, se deben eliminar las comillas que lo envuelven:

```json
{
  "producto": "Ordenador",
  "precio": 1200,
  "stock": 15
}
```

---

## Objetivo del Ejercicio
El propósito de esta actividad es aprender a **distinguir entre un String que contiene dígitos numéricos y un tipo de dato Number (Integer)**. En el desarrollo de software y el intercambio de datos (como JSON), las comillas definen la naturaleza del dato y cómo el ordenador lo procesará.
