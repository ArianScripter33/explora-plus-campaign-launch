# EXPLORA+ · Evidencia de la exposición v4

EXPLORA+ es la campaña de un proyecto prototípico de Ciencia de Datos para Negocios de la UNRC. Propone consulta gratuita para planear y guardar una ruta por Puuc y Maní. La meta es una PWA de menos de 5 MB y acceso sin conexión al itinerario guardado. Las experiencias se pagan al proveedor. El piloto contempla apoyo institucional y servicios a comercios sujetos a acuerdos.

| Lámina | Respaldo y cálculo |
| --- | --- |
| 02 · Concentración | Corte local de recintos INAH en Yucatán 2022–2025: 12 283 255 visitas. Chichén Itzá 9 393 172 (76,47 %), Uxmal 1 068 559 (8,70 %) y Kabah 157 380 (1,28 %). Cada barra divide por el mismo total. |
| 03 · Audiencia | OTY, visitantes con pernocta de enero a septiembre de 2025: 32,5 % en pareja, 32,1 % en familia, 20,0 % en solitario y 15,4 % con amigos. Los perfiles tácticos sintetizan fricciones y formatos. El equipo comparó Civitatis, Viator, Maps, Airbnb Experiences, Xcaret y ADO/Turibus. |
| 04 · Etapas | Presupuesto propuesto para 38 semanas en el estudio interno §3.3: 15 % prelanzamiento, 45 % lanzamiento, 30 % sostenimiento, 10 % postlanzamiento. |
| 06 · DENUE | 146 384 registros estatales en el CSV local. Suma de establecimientos SCIAN 522110, 522210 y 522320: Mérida 162 + 11 + 49 = 222; Maní 0 + 1 + 1 = 2; Santa Elena 0 + 1 + 0 = 1. |
| 06 · Rest-Mex | Train y test de alexcom: 251 702 filas, 246 153 textos únicos de más de 20 caracteres, 11 524 con menciones a topónimos seleccionados. Coincidencias temáticas: filas y multitudes 570 (4,9 %), pagos y efectivo 212 (1,8 %), baños 483 (4,2 %). Los temas se pueden solapar. |
| 07 · Pronóstico | CSV INAH de Uxmal, 24 pronósticos de un mes adelante en 2024–2025, clima previo y calendario SEP. WAPE: referencia estacional 15,09 %, XGBoost 16,39 %, HistGradientBoosting 17,35 %. El denominador es 549 538 visitas observadas. La campaña usa la referencia estacional. |
| 08 · Clima y ruta | Gumbel ajustada a 996 días con lluvia >0,1 mm del histórico de 1 765 días. Monte Carlo: 100 000 trayectorias, 52 pasos, semilla 42. >45 mm diarios es un umbral de escenario para pausar promoción de cenotes y valorar talleres techados. El grafo compara 104,6 km y 143,1 km. |
| 09 · Cupón | Día valle con 18 % de ocupación: 0,35 × 0,82 = 28,7 %. Fuera de día valle o con aforo lleno: 0 %. |
| 10 · Medición | Visitas verificadas elegibles entre semana en destinos alternativos ÷ total de visitas verificadas elegibles del piloto, comparadas contra semanas equivalentes. |

## Fuentes de consulta

- [INAH · Estadística de Visitantes](https://estadisticas.inah.gob.mx/)
- [INEGI · DENUE](https://www.inegi.org.mx/app/mapa/denue/default.aspx)
- [Gobierno de Yucatán · Observatorio Turístico, comunicado 25-1896](https://www.yucatan.gob.mx/saladeprensa/ver_nota.php?id=10215)
- [Open-Meteo · Archivo histórico](https://open-meteo.com/en/docs/historical-weather-api)
- [Rest-Mex · Dataset de alexcom](https://huggingface.co/datasets/alexcom/analisis-sentimientos-textos-turisitcos-mx-polaridad)
- [Esri World Imagery](https://www.arcgis.com/home/item.html?id=10df2279f9684e4a9f6a7f08febac2a9) y [OpenStreetMap](https://www.openstreetmap.org/copyright)

## Lectura del benchmark anterior

El valor archivado de 9,54 % usa el caché mensual, clima observado del mes objetivo y MAPE promedio por bloque. Los 48 meses compartidos por el caché y el CSV de Uxmal difieren. La comparación v4 usa el CSV, clima disponible antes del mes y un WAPE común. Los recuentos de DENUE y reseñas de esta página identifican el corte y la regla con que se obtuvieron.
