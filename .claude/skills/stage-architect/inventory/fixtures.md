# Inventario de luminarias

Fuentes:
- **Fotos** (5): existencia, tipo visual y orden → `ESTIMADO`.
- **Captura de consola** (`evidence/2026-11-08-ma2-editsetup-layers.png`, EditSetup → Layers): nombres de layer y fixture IDs → `CONFIRMADO` como lectura de pantalla.
- El **vínculo** entre una luz física y su fixture ID se deduce por nombre y cantidad → `ESTIMADO` hasta que el usuario lo confirme o se vea el patch.

Zonas confirmadas por el usuario: barra frontal con altavoces = TRUSS 1; barra de los 5 PAR sobre la pantalla = TRUSS 2. Los 4 PAR grandes cuelgan de la pantalla grande. Los IDs `SCR-` son provisionales (ver `validation/pending-information.md`).

| ID interno | Plano | Tipo (foto) | Zona | Nombre del usuario | Layer MA2 (captura) | Fixture ID MA2 | Vínculo |
|---|---|---|---|---|---|---|---|
| TR2-PAR01 | P1 | PAR redondo pequeño | TRUSS 2 | Pares Cris | LED 1 | 9 | ESTIMADO |
| TR2-PAR02 | P2 | PAR redondo pequeño | TRUSS 2 | Pares Cris | LED 2 | 10 | ESTIMADO |
| TR2-PAR03 | P3 | PAR redondo pequeño | TRUSS 2 | Pares Cris | LED 3 | 11 | ESTIMADO |
| TR2-PAR04 | P4 | PAR redondo pequeño | TRUSS 2 | Pares Cris | LED 4 | 12 | ESTIMADO |
| TR2-PAR05 | P5 | PAR redondo pequeño | TRUSS 2 | Pares Cris | LED 5 | 13 | ESTIMADO |
| SCR-PAR01 | G1 | PAR grande | Colgado de la pantalla | Techo Cris | TECHO 1 | 1 | ESTIMADO |
| SCR-PAR02 | G2 | PAR grande | Colgado de la pantalla | Techo Cris | TECHO 2 | 2 | ESTIMADO |
| SCR-PAR03 | G3 | PAR grande | Colgado de la pantalla | Techo Cris | TECHO 3 | 3 | ESTIMADO |
| SCR-PAR04 | G4 | PAR grande | Colgado de la pantalla | Techo Cris | "TECHO 3" (nombre repetido) | 4 | ESTIMADO |
| TR1-BAR01 | B1 | Barra de 5 LED | TRUSS 1 | Barras Cris | BAR IZQUIERDA | 5 | ESTIMADO |
| TR1-BAR02 | B2 | Barra de 5 LED | TRUSS 1 | Barras Cris | BAR DERECHA | 6 | ESTIMADO |
| FLOOR-MH01 | M1 | Cabeza móvil | FLOOR | Ambas Spot | SPOT IZQUIERDA | 8 | ESTIMADO |
| FLOOR-MH02 | M2 | Cabeza móvil | FLOOR | Ambas Spot | SPOT DERECHA | 7 | ESTIMADO |
| TR1-SML01 | C1 | Foco pequeño | TRUSS 1 | Batería Cris | WASH BATERIA | 14 | ESTIMADO (solo 1 layer visible) |
| TR1-SML02 | C2 | Foco pequeño | TRUSS 1 | Batería Cris | no visible | PENDIENTE | PENDIENTE |
| TR1-FRS01 | F1 | Fresnel con viseras | TRUSS 1 | Front Cris | FRONT (fila cortada) | 15 (¿cuál de los 4?) | PENDIENTE |
| TR1-FRS02 | F2 | Fresnel con viseras | TRUSS 1 | Front Cris | no visible | PENDIENTE | PENDIENTE |
| TR1-FRS03 | F3 | Fresnel con viseras | TRUSS 1 | Front Cris | no visible | PENDIENTE | PENDIENTE |
| TR1-FRS04 | F4 | Fresnel con viseras | TRUSS 1 | Front Cris | no visible | PENDIENTE | PENDIENTE |

Total físico (fotos): 19 luminarias. Fixture IDs vistos en la captura: 1 al 15. La lista de layers continúa debajo de FRONT y no se vio.

## Puntos que no cuadran todavía

- **Batería:** hay 2 focos pequeños (C1, C2) en las fotos, pero solo un layer `WASH BATERIA` [14] a la vista.
- **Front:** hay 4 fresnel, pero solo se ve `FRONT` [15]. Probablemente hay más layers debajo (no confirmado).
- **TECHO 3 repetido:** dos layers se llaman "TECHO 3", con fixture 3 y fixture 4. Parece que el segundo es "TECHO 4" mal escrito. No lo corrijo hasta que el usuario lo confirme.
- **Izquierda/derecha en consola:** `BAR IZQUIERDA/DERECHA` y `SPOT IZQUIERDA/DERECHA` no dicen desde qué punto de vista. Se asumió congregación. Si es al revés, M1 y M2 (y B1 y B2) se invierten.
- **Orden dentro de cada grupo:** se asume que fixture ID creciente = izquierda a derecha en cada grupo. No verificado.

## No son luminarias

- Altavoces colgados: `TR1-SPK01`, `TR1-SPK02`.
- Luces de sala: cantidad y control `PENDIENTE`. Sin layer visible en la captura.
