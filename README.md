# Calidad de Datos en el ETL: Las 6 Dimensiones

Documentación académica replicable sobre las 6 dimensiones de calidad de datos (framework DAMA) aplicadas al proceso ETL. Incluye fórmulas de medición, umbrales por criticidad, criterios de aceptación y descarte, e implementación práctica.

---

## 📄 Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `index.html` | Artefacto interactivo con las 6 dimensiones, métricas, umbrales y hallazgos |
| `Calidad_de_Datos_en_el_ETL_Las_6_Dimensiones.pdf` | Presentación de apoyo en formato PPTX exportada a PDF |

---

## 🧭 Estructura del artefacto

El archivo `index.html` está organizado en 4 secciones navegables:

- **Dimensiones** — Definición, fórmula y ejemplo ilustrativo de cada una de las 6 dimensiones
- **Umbrales** — Tabla de umbrales aceptables por dimensión y nivel de criticidad
- **Hallazgos** — Resultados ilustrativos de una evaluación con impacto operativo y acciones recomendadas
- **Herramientas** — Plataformas comerciales y open source para automatizar la medición

---

## 📐 Las 6 Dimensiones (Framework DAMA)

| # | Dimensión | Descripción |
|---|---|---|
| 1 | **Exactitud** | Los datos reflejan la realidad sin errores |
| 2 | **Integridad** | No hay campos requeridos vacíos o nulos |
| 3 | **Coherencia** | Los datos son consistentes entre tablas y fuentes |
| 4 | **Puntualidad** | Los datos están disponibles cuando se necesitan |
| 5 | **Unicidad** | No existen registros duplicados |
| 6 | **Validez** | Los datos cumplen formatos y reglas definidas |

---

## 🔢 Fórmulas base

```
Integridad (%)  = (Valores no nulos / Total requeridos) × 100
Exactitud (%)   = (Registros correctos / Total muestreados) × 100
Unicidad (%)    = (Registros únicos / Total registros) × 100
Validez (%)     = (Registros con formato correcto / Total) × 100
Coherencia (%)  = (Registros consistentes entre tablas / Total) × 100
Puntualidad (%) = (Registros a tiempo / Total requeridos) × 100
```

---

## ✅ Criterios ETL

**Aceptación** — El dato cumple reglas de negocio, tiene formato correcto, es consistente, único y completo.

**Descarte** — El dato es irrelevante, inconsistente, incompleto o duplicado de forma no válida para el análisis.

**Umbrales orientativos**

| Tipo de campo | % faltantes | Acción |
|---|---|---|
| ID / clave primaria | > 0% | ❌ Descartar o revisar fuente |
| Campos críticos | ≤ 5% | ✅ Imputar |
| Campos críticos | 5 – 20% | ⚠️ Evaluar impacto |
| Campos críticos | > 20% | ❌ Descartar |
| Campos no críticos | ≤ 20% | 👍 Dejar nulo o imputar |
| Campos no críticos | > 50% | ❌ Eliminar columna |

---

## 🛠️ Herramientas referenciadas

- **Talend Data Quality** — Perfilado ML, deduplicación, scoring de confianza
- **Informatica DQ** — Limpieza por reglas automáticas, monitoreo continuo
- **Ataccama ONE** — Detección de anomalías con IA
- **OpenRefine** — Open source, ideal para prototipos
- **Apache Griffin** — Open source, optimizado para big data

---

## 📚 Referencias

- DAMA International. *Data Management Body of Knowledge (DMBOK)*
- IBM Data Quality Documentation
- Alation Data Quality Framework
- QuestionPro Data Quality Guide

---

## 🚀 Visualizar el artefacto

El artefacto está publicado en GitHub Pages:

> 🔗 `https://NataCastanoH.github.io/CalidadDatos`

---

*Documentación académica replicable · Framework DAMA · ETL · Business Intelligence*
