# Vista frontal

Desde la congregación mirando al escenario. Esquema `ESTIMADO`, sin escala. La altura relativa viene de las fotos. Izquierda a derecha según la congregación.

```mermaid
flowchart TB
  subgraph B["Barra B (¿TRUSS 2?) · sobre la pantalla"]
    direction LR
    P1["TR2-PAR01"] --- P2["TR2-PAR02"] --- P3["TR2-PAR03"] --- P4["TR2-PAR04"] --- P5["TR2-PAR05"]
  end
  subgraph A["Barra A (¿TRUSS 1?) · frontal"]
    direction LR
    SL["SPK01"] --- C1["TR1-SML01"] --- B1["TR1-BAR01"] --- F1["TR1-FRS01"] --- F2["TR1-FRS02"] --- F3["TR1-FRS03"] --- F4["TR1-FRS04"] --- B2["TR1-BAR02"] --- C2["TR1-SML02"] --- SR["SPK02"]
  end
  subgraph S["Pantalla y fondo"]
    direction LR
    M1["FLOOR-MH01"] --- G1["SCR-PAR01"] --- G2["SCR-PAR02"] --- G3["SCR-PAR03"] --- G4["SCR-PAR04"] --- M2["FLOOR-MH02"]
  end
  B --> A --> S
```

El orden de arriba hacia abajo indica altura relativa aproximada. No hay medidas.

Vista interactiva del esquema: https://claude.ai/artifact/TGTsVGhx3vJSkwVbcWaLhH (usa los códigos P, G, F, B, M, C; ver equivalencias en `inventory/fixtures.md`).
