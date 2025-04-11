
### Comparativa de Modelos de Raspberry Pi y Alternativa

| Modelo                  | Consumo Energético (reposo/carga) | Rendimiento (CPU/RAM)       | Ventajas                       | Desventajas                    |
|-------------------------|------------------------------------|-----------------------------|--------------------------------|--------------------------------|
| **Raspberry Pi Zero W** | ~0.5W / ~1.2W                     | 1 núcleo / 512MB RAM        | Muy bajo consumo; económico.   | Rendimiento limitado.          |
| **Raspberry Pi 3B+**    | ~1.2W / ~4W                       | 4 núcleos / 1GB RAM         | Buen balance entre consumo y potencia. | Menor eficiencia que el Pi 4.  |
| **Raspberry Pi 4 (4GB)**| ~3W / ~6W                         | 4 núcleos / hasta 8GB RAM   | Excelente rendimiento; multitarea. | Alto consumo para proyectos solares pequeños. |
| **Raspberry Pi 400**    | ~6W / ~10W                        | 4 núcleos / 4GB RAM         | Integración con teclado; ideal para aprendizaje. | Diseño menos compacto.         |

### Alternativa: ODROID-C4

| Modelo                  | Consumo Energético                | Rendimiento (CPU/RAM)       | Ventajas                       | Desventajas                    |
|-------------------------|------------------------------------|-----------------------------|--------------------------------|--------------------------------|
| **ODROID-C4**           | ~2W / ~4W                         | 4 núcleos / 4GB RAM         | Similar al Raspberry Pi 4 pero más eficiente energéticamente. | Menor soporte de comunidad y software. |

### Conclusiones

Tras analizar las diferentes opciones, hemos obtenido las siguientes conclusiones en relación a las necesidades de este proyecto:

- **Raspberry Pi Zero W**: Es la opción ideal si el tráfico web será bajo (servidor estático) y el presupuesto es reducido. Su bajo consumo la hace perfecta para un sistema alimentado con un panel solar pequeño (~5W).

- **Raspberry Pi 3B+**: Una buena opción para proyectos con requerimientos moderados, como un servidor dinámico con tráfico ocasional. Sin embargo, su consumo energético demanda un panel solar más potente, de aproximadamente 10W.

- **Raspberry Pi 4**: Es la mejor elección si se necesita alto rendimiento (por ejemplo, para bases de datos o aplicaciones más pesadas). No obstante, su mayor consumo energético implica una configuración solar más robusta, con un panel de ~20W o superior.

- **ODROID-C4**: Representa una alternativa eficiente si se busca un rendimiento similar al Raspberry Pi 4, pero con un consumo energético algo menor. A pesar de esto, su menor soporte de comunidad y software podría dificultar su implementación en comparación con las opciones de Raspberry Pi.


**[Volver al inicio ](README.md)** | **[Consumo Energético ](consumo.md)**
