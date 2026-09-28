# Ejercicio 4 — Detectar errores

El siguiente JSON contenía varios errores de sintaxis que impedían su correcta validación:

## JSON Original (Con errores)
```json
{ 
"nombre": "Laura" 
"edad": 22, 
"activo": verdadero, 
"ciudad": "Valencia", 
}
```

---

## Errores detectados y corrección
1. **Falta de coma (`,`):** No existía una coma de separación entre la línea de `"nombre"` y `"edad"`.
2. **Valor booleano incorrecto (`verdadero`):** Los booleanos en JSON deben escribirse estrictamente en inglés y en minúsculas (`true` o `false`).
3. **Coma huérfana o terminal (`,`):** Había una coma de más después de `"Valencia"`. El último elemento de un objeto JSON **no** debe llevar coma al final.

---

## JSON Válido y Corregido

```json
{ 
  "nombre": "Laura", 
  "edad": 22, 
  "activo": true, 
  "ciudad": "Valencia" 
}
```
