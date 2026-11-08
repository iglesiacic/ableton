# Patch DMX

**Sin datos.** No se ha recibido el patch de grandMA2.

Para llenar esta tabla se necesita una de estas fuentes (de más a menos fiable):

1. Exportación del patch desde MA2 (lista de fixtures con universo y dirección).
2. Captura de la pantalla *Setup → Patch*.
3. Dictado del usuario, fixture por fixture.

| ID interno | Fixture ID | Universo | Dirección inicial | Modo | Canales | Rango (fin) | Estado |
|---|---|---|---|---|---|---|---|
| (sin filas) | | | | | | | PENDIENTE |

## Comprobaciones al importar

- Que no haya direcciones solapadas dentro de un universo.
- Que la suma de canales por fixture coincida con el modo.
- Que cada fixture del patch tenga una luminaria física en `fixtures.md`.
- Que cada luminaria de `fixtures.md` aparezca en el patch.
- Que no haya fixture IDs duplicados.
