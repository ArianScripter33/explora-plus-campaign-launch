# EXPLORA+ · Campaign Launch

Proyecto prototípico de Ciencia de Datos para Negocios en la UNRC. La campaña propone redistribuir visitas hacia Ruta Puuc–Maní en días con capacidad.

## Fuentes de consulta

| Fuente | Uso |
| --- | --- |
| [INAH · Estadística de Visitantes](https://estadisticas.inah.gob.mx/) | Visitas por recinto y mes; serie de Uxmal |
| [INEGI · DENUE](https://www.inegi.org.mx/app/mapa/denue/default.aspx) | Inventario territorial y clasificación SCIAN |
| [Open-Meteo · Archivo histórico](https://open-meteo.com/en/docs/historical-weather-api) | Temperatura y precipitación diaria |
| [Rest-Mex · IberBench](https://huggingface.co/datasets/iberbench/iberbench_all) | Antecedente del análisis de reseñas turísticas |
| [Esri World Imagery](https://www.arcgis.com/home/item.html?id=10df2279f9684e4a9f6a7f08febac2a9) y [OpenStreetMap](https://www.openstreetmap.org/copyright) | Referencia cartográfica |

## Cómo leer la evidencia

- Los porcentajes de Chichén Itzá, Uxmal y Kabah usan como denominador 12 283 255 visitas registradas en el corte local de recintos INAH de Yucatán, 2022–2025.
- El WAPE de Uxmal divide la suma de errores absolutos por la suma de visitas observadas en 24 cortes de un mes adelante durante 2024–2025.
- Dijkstra compara caminos en un grafo piloto. Las distancias que expone el equipo provienen de esas aristas.
- Monte Carlo usa una tasa Poisson hipotética de 0,05 por ventana. El cupón se activa en día valle según capacidad disponible.
- La redistribución de visitas y el impacto comercial se medirían en el piloto.
