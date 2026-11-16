<h1 align="center">📍 Autocorrelación y regresión espacial en R</h1>

<p align="center">
  <b>¿Los homicidios en EE. UU. se agrupan en el espacio? ¿Qué los explica y cómo varía ese efecto entre estados?</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white" alt="R">
  <img src="https://img.shields.io/badge/spdep-Autocorrelación-589632?style=for-the-badge" alt="spdep">
  <img src="https://img.shields.io/badge/spatialreg-SAR_%2F_SEM-F37626?style=for-the-badge" alt="spatialreg">
  <img src="https://img.shields.io/badge/GWmodel-GWR-7B3FA0?style=for-the-badge" alt="GWmodel">
</p>

---

## 📌 Resumen

Análisis completo de econometría espacial sobre la tasa de homicidios (`Murder`) de los 48 estados contiguos de EE. UU., en función del analfabetismo, el ingreso, la proporción de graduados de secundaria y los días de helada. Trabajo práctico del **Diplomado en Análisis Espacial de Datos, Universidad de Chile** (2026).

El script es **totalmente reproducible**: usa datos incluidos en R (`state.x77` y `spData::us_states`), así que no hace falta descargar nada.

## ⚙️ Qué incluye

**1. Autocorrelación espacial**
- Cuatro estructuras de vecindad comparadas: contigüidad reina y torre, k vecinos más próximos (k = 4) y distancia (580 km).
- Matrices de pesos estandarizada por filas y binaria.
- I de Moran (analítico y por 999 permutaciones), C de Geary y diagrama de dispersión de Moran.
- Autocorrelación local: Moran local (LISA), mapa de conglomerados y puntos calientes y fríos de Getis-Ord Gi.
- Prueba de robustez del I de Moran con las cuatro vecindades.

**2. Regresión espacial**
- Modelo MCO de referencia, diagnóstico de residuos y mapa de residuos.
- Tests de multiplicadores de Lagrange para elegir la especificación.
- Modelos de **rezago espacial (SAR)** y **error espacial (SEM)**, con test de razón de verosimilitud.
- Efectos **directos, indirectos y totales** del SAR.
- **Regresión geográficamente ponderada (GWR)** con ancho de banda adaptativo: coeficiente local del analfabetismo y R² local.

## ▶️ Cómo ejecutarlo

1. Abrí `econometria_espacial.R` en RStudio.
2. Ejecutá el **Paso 1** para instalar y cargar los paquetes.
3. Corré el script completo. Las figuras (`Figura_1` a `Figura_9`), las tablas (`Tabla_4` a `Tabla_8`) y un anexo con todas las salidas se guardan en la carpeta de trabajo.

Paquetes: `sf`, `spData`, `spdep`, `spatialreg`, `tmap`, `GWmodel`, `dplyr`.

---

<p align="center">
  <b>Anabella Engelman</b> · Geógrafa · Análisis espacial de datos<br/>
  <a href="https://github.com/geografaengelman-dev">GitHub</a> ·
  <a href="https://www.linkedin.com/in/anabella-engelman-ab1aaa80/">LinkedIn</a> ·
  <a href="mailto:geografaengelman@gmail.com">geografaengelman@gmail.com</a>
</p>

<p align="center"><sub>© 2026 Anabella Engelman. Todos los derechos reservados.</sub></p>
