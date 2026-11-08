# Grupos, layers y ejecutores

## Nombres del usuario (`CONFIRMADO`)

El usuario confirmó que **estos nombres son grupos de grandMA2**.

| Grupo (nombre del usuario) | Plano | Cantidad (fotos) | Luminarias |
|---|---|---|---|
| Pares Cris | P1–P5 | 5 | TR2-PAR01..05 |
| Techo Cris | G1–G4 | 4 | SCR-PAR01..04 |
| Front Cris | F1–F4 | 4 | TR1-FRS01..04 |
| Barras Cris | B1–B2 | 2 | TR1-BAR01..02 |
| Ambas Spot | M1–M2 | 2 | FLOOR-MH01..02 |
| Batería Cris | C1–C2 | 2 | TR1-SML01..02 |

Qué fixtures tiene cada grupo dentro de la consola, y su número de grupo, **no se han visto** (`PENDIENTE`).

## Lo que muestra la captura (`CONFIRMADO` como lectura de pantalla)

### Layers (vista EditSetup → Layers)

TECHO 1, TECHO 2, TECHO 3 (dos veces), BAR IZQUIERDA, BAR DERECHA, SPOT IZQUIERDA, SPOT DERECHA, LED 1 a LED 5, WASH BATERIA, FRONT y más debajo. Cada layer contiene un solo fixture. Detalle en `fixture-ids.md`.

Los nombres de layer **no son idénticos** a los de los grupos. La correspondencia más probable, por nombre y cantidad:

| Grupo del usuario | Layers relacionados | Estado |
|---|---|---|
| Techo Cris | TECHO 1–4 | ESTIMADO |
| Pares Cris | LED 1–5 | ESTIMADO |
| Barras Cris | BAR IZQUIERDA, BAR DERECHA | ESTIMADO |
| Ambas Spot | SPOT IZQUIERDA, SPOT DERECHA | ESTIMADO |
| Batería Cris | WASH BATERIA | ESTIMADO (falta un fixture) |
| Front Cris | FRONT | ESTIMADO (falta ver los demás) |

### Ejecutores (página de faders 1, posiciones 1–6)

| Posición | Nombre | Contenido |
|---|---|---|
| 1 | LT84 TECHO | 1 cue |
| 2 | LT85 BARRAS | 1 cue |
| 3 | LT86 PARES | 1 cue |
| 4 | LT87 BATERIA | 1 cue |
| 5 | LT88 FRONT | 1 cue |
| 6 | LT89 SPOTS | 1 cue |

Los seis tienen un cue y aparecen con el mismo formato. Para qué sirven exactamente (por ejemplo, un nivel por grupo) no se leyó en la captura. No asumir. Aparte hay un ejecutor `LT AZUL` (posición 1.21) con 1 cue, que se ve activo.

## Pendiente

- Captura del pool de **Groups** con sus números y los fixtures de cada grupo.
- Confirmar si "Pares Cris", "Techo Cris", etc. son el nombre exacto del grupo o una forma de llamarlo.
- Qué significa "Cris" en los nombres.

## Reglas

- No inventar números de grupo.
- Para un show nuevo, proponer el grupo y esperar confirmación antes de usarlo.
