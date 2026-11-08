---
name: stage-architect
description: Fuente de verdad de la arquitectura física y técnica del escenario de la iglesia (grandMA2 / MA2 onPC). Úsala para saber qué luminarias existen, dónde están, su fixture ID, atributos, universo/dirección DMX y grupos. Consúltala antes de diseñar o programar cualquier show. No inventa datos: separa lo confirmado, lo estimado y lo pendiente.
---

# stage-architect

Base de conocimiento del escenario. **No crea shows.** Solo describe la instalación para que otras Skills programen sin inventar posiciones, fixtures ni capacidades.

## Regla de oro

Cada dato lleva una etiqueta de estado. Nunca mezcles estados ni subas uno sin evidencia.

| Estado | Significado |
|---|---|
| `CONFIRMADO` | Lo dijo el usuario o viene del patch/showfile real. |
| `ESTIMADO` | Deducido de fotos. Puede estar mal. |
| `PENDIENTE` | No se sabe. Se deja vacío y se pregunta. |

Una foto no confirma modelo, dirección DMX, modo ni atributos.

## Zonas

`TRUSS 1`, `TRUSS 2` y `FLOOR`. El mapeo entre las barras vistas en las fotos y estas zonas está `PENDIENTE` (ver `validation/pending-information.md`).

## Mapa de archivos

| Necesitas saber… | Lee |
|---|---|
| Visión general y zonas | `architecture/stage-overview.md` |
| Sistema de coordenadas y posiciones | `architecture/stage-layout.md` |
| Qué hay en cada zona | `architecture/truss-1.md`, `truss-2.md`, `floor-fixtures.md` |
| Lista de luminarias con ID | `inventory/fixtures.md` |
| Modelo, canales y atributos | `inventory/fixture-specifications.md` |
| Universo y dirección DMX | `inventory/dmx-patch.md` |
| Vistas del escenario | `diagrams/front-view.md`, `top-view.md`, `side-view.md` |
| Grupos y fixture IDs de consola | `grandma2/groups.md`, `fixture-ids.md`, `console-configuration.md` |
| Qué está verificado y qué falta | `validation/verified-data.md`, `pending-information.md` |
| Nombres que usa el usuario | `grandma2/groups.md` |

## Identificadores

`<ZONA>-<TIPO><NN>`, por ejemplo `TR1-MH01`, `TR2-PAR01`, `FLOOR-MH01`. Son referencias internas. Se conservan aparte el fixture ID y el nombre real de grandMA2.

## Cómo responder a otros agentes

Ante una consulta (qué luces hay, dónde, qué controlan, cuáles trabajan juntas, qué cobertura dan, qué limitaciones hay):

1. Responde solo con datos `CONFIRMADO` o `ESTIMADO`, indicando cuál.
2. Si falta un dato, di que está `PENDIENTE`. No lo rellenes.
3. Si la tarea depende de un dato pendiente, pide que se pregunte al usuario.

## Reglas de seguridad

- No modificar el showfile ni ejecutar comandos destructivos en la consola durante el levantamiento.
- No cambiar un estado a `CONFIRMADO` sin evidencia anotada en `validation/verified-data.md`.
- Actualizar los diagramas cuando cambie la arquitectura.

## Fases

1. Recopilación de fotografías (en curso).
2. Identificación y clasificación de luminarias (borrador).
3. Mapa espacial.
4. Importación del patch de grandMA2.
5. Validación con el usuario.
6. Documentación definitiva.
7. Pruebas de consulta.

No avanzar de fase si faltan datos fundamentales. Estado actual y datos faltantes: `validation/pending-information.md`.
