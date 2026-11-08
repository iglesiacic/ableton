# Patch DMX

**Datos parciales.** Solo una fila tiene patch real, leída de la captura. Falta el patch completo.

Formato de la columna Patch en MA2: `universo.dirección` (por ejemplo, `1.013` = universo 1, dirección 13).

| ID interno | Fixture ID | Fixture Type (MA2) | Nombre del fixture | Universo | Dirección | Modo / canales | Estado |
|---|---|---|---|---|---|---|---|
| SCR-PAR03 (¿?) | 3 (ChaID 3) | 6 Colorado 1 Tri | C1T7TA1S 1 | 1 | 13 | PENDIENTE | CONFIRMADO en pantalla. Vínculo con SCR-PAR03 ESTIMADO |
| (resto de fixtures 1–2, 4–15+) | | | | | | | PENDIENTE |

Notas de la fila 3:
- `React to Master`: On.
- `Pan DMX Invert` y `Tilt DMX Invert`: vacíos.
- El fixture type aparece como "Colorado 1 Tri" con número 6 en el pool de tipos. El fabricante y el modo DMX no se leen en la captura. No asumir.

No se puede deducir la dirección de los demás fixtures a partir de esta. Los saltos entre direcciones dependen del tamaño de cada modo.

## Cómo completar

1. Captura de *Setup → Patch & Fixture Schedule* con todos los fixtures.
2. Captura de *Fixture Types* (para modos y canales).
3. O una exportación del showfile en modo lectura.

## Comprobaciones al importar

- Direcciones solapadas dentro de un universo.
- Suma de canales por fixture frente al modo.
- Cada fixture del patch tiene luminaria física en `fixtures.md`, y al revés.
- Sin fixture IDs duplicados.
