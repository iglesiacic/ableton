# Grupos, layers y ejecutores

## Pool de grupos (`CONFIRMADO` como lectura de pantalla)

Fuente: `evidence/2026-11-08-ma2-group-pool.png` (pool "Group", 39 posiciones visibles). Ocupadas: 1–6 y 11–14. El resto está vacío. Nombres tal como se ven en pantalla.

| Group # | Nombre en consola | Plano | Contenido (fixtures) | Estado del contenido |
|---|---|---|---|---|
| 1 | TECHO CRIS | G1–G4 | PENDIENTE (se espera 1–4) | ESTIMADO |
| 2 | BARRAS CRIS | B1–B2 | PENDIENTE (se espera 5–6) | ESTIMADO |
| 3 | AMBAS SPOT | M1–M2 | PENDIENTE (se espera 7–8) | ESTIMADO |
| 4 | PARES CRIS | P1–P5 | PENDIENTE (se espera 9–13) | ESTIMADO |
| 5 | BATERIA CRIS | C1–C2 | PENDIENTE (se espera 14 y ¿otro?) | ESTIMADO |
| 6 | FRONT CRIS | F1–F4 | PENDIENTE (se espera 15 y más) | ESTIMADO |
| 11 | IZQUIERDA SPOT | M1 o M2 | PENDIENTE (¿fixture 8?) | ESTIMADO |
| 12 | DERECHA SPOT | M2 o M1 | PENDIENTE (¿fixture 7?) | ESTIMADO |
| 13 | PARES FONDO | PENDIENTE | PENDIENTE | PENDIENTE |
| 14 | PARES ALFRENTE | PENDIENTE | PENDIENTE | PENDIENTE |

Los grupos 1 al 6 coinciden con los nombres del usuario. Los grupos 11 al 14 no estaban en la lista del usuario.

### Dudas sobre los grupos 13 y 14

`PARES FONDO` y `PARES ALFRENTE` ("al frente") no se pueden asignar solos. Hay dos tipos de PAR en las fotos: los 5 pequeños de la barra del fondo (TRUSS 2) y los 4 grandes de la pantalla. No se sabe si estos grupos los reparten así ni qué fixtures tienen. No asumir.

### Qué hay en el pool que no es grupo

La pantalla también muestra vistas de usuario (TIMECODE, BUTONS, POSITION, GROUP, CLEAR, BARS, LAYAOU, FX, PICKER). No se analizaron.

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

- Qué fixtures contiene cada grupo (la captura solo muestra nombres y números).
- Qué son `PARES FONDO` y `PARES ALFRENTE`.
- En `IZQUIERDA SPOT` y `DERECHA SPOT`, la izquierda y derecha: ¿desde la congregación o desde el escenario?
- Qué significa "Cris" en los nombres.

## Reglas

- No inventar números de grupo.
- Para un show nuevo, proponer el grupo y esperar confirmación antes de usarlo.
