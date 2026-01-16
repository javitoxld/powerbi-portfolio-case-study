# Decisions log + Definition of Done (DoD)

## 1) Definition of Done (DoD) — Portfolio-ready
El proyecto se considera “terminado” cuando:

1. Dataset 100% publicable (o anonimizado) y fuente documentada (link + fecha + licencia/uso).
2. Modelo orientado a BI, preferiblemente **esquema estrella** (hechos + dimensiones) o justificación si no aplica. Microsoft recomienda el enfoque de star schema para rendimiento y usabilidad. 
3. Power Query: tipos correctos, tratamiento de nulos/duplicados y transformaciones mínimas pero justificadas.
4. Medidas DAX clave (KPIs) con nombres consistentes y formato correcto (€, %, unidades) en una tabla/carpeta de medidas.
5. Reporte con narrativa: mínimo 2–3 páginas (Overview / Deep Dive / Insights) con filtros/segmentadores claros.
6. Diseño consistente (alineación, jerarquía visual, tema) y legibilidad (sin “ruido”).
7. Performance básica revisada: sin visuales redundantes, columnas innecesarias minimizadas, agregaciones razonables.
8. Exportables listos: PBIX final + PDF del reporte (y, si aplica, PDF/PPTX del pitch en Gamma).
9. Repo GitHub completo: README, estructura de carpetas, capturas en /images, documentación en /docs, sin datos sensibles.
10. Notion Case Study hub: problema → enfoque → modelo → decisiones → insights → links (GitHub, Gamma, PDF).
11. Pitch (Gamma): 6–10 slides con 3–5 insights accionables y capturas del dashboard.
12. Nota de seguridad (si se contempla “embed”): **Publish to web** es público y sin autenticación; puede exponer datos del modelo. Solo usar con datos totalmente publicables.

## 2) Registro de decisiones (rellenar a medida que avanzas)
Formato: Fecha | Decisión | Motivo | Impacto

- 2026-01-16 | Repo creado con README + MIT License | Portfolio público y reutilizable | Base lista para documentar el caso.
- 2026-01-16 | Estructura de carpetas (/pbix /exports /images /docs) | Orden y replicabilidad | Facilita revisión y exportables.

## 3) Notas de seguridad / publicación (crítico)
- Si se usa **Publish to web**: cualquiera en Internet puede ver el reporte sin autenticarse y podría acceder a datos subyacentes del modelo aunque no se muestren en visuales. No publicar datos confidenciales.
