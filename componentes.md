# Hardware

A la hora de elegir el dispositivo que alojará nuestra página web sostenible, consideramos que la opción más económica y respetuosa con el medio ambiente es el uso de una placa Raspberry Pi. Este tipo de dispositivo destaca por su bajo consumo energético, su tamaño compacto y su facilidad de uso, lo que lo convierte en una excelente herramienta para proyectos de computación sostenible.

Existen diversos modelos de Raspberry Pi en el mercado, cada uno con especificaciones distintas que afectan tanto al rendimiento como al impacto ambiental. A continuación, se presenta una comparativa entre varios modelos relevantes y una alternativa interesante: el ODROID-C4.




## Comparativa de Modelos de Raspberry Pi y Alternativa

| Modelo                  | Consumo Energético (reposo/carga) | Rendimiento (CPU/RAM)       | Ventajas                       | Desventajas                    |
|-------------------------|------------------------------------|-----------------------------|--------------------------------|--------------------------------|
| **Raspberry Pi Zero W** | ~0.5W / ~1.2W                     | 1 núcleo / 512MB RAM        | Muy bajo consumo; extremadamente económica.|Rendimiento limitado; no apta para cargas altas.          |
| **Raspberry Pi 3B+**    | ~1.2W / ~4W                       | 4 núcleos / 1GB RAM         | Buen equilibrio entre potencia y eficiencia. | Menos eficiente que modelos más recientes.  |
| **Raspberry Pi 4 (4GB)**| ~3W / ~6W                         | 4 núcleos / hasta 8GB RAM   | Excelente rendimiento y multitarea. | Mayor consumo, menos adecuada para energía solar limitada. |
| **Raspberry Pi 400**    | ~6W / ~10W                        | 4 núcleos / 4GB RAM         | Integrada en un teclado; orientada a educación. | Diseño voluminoso; menos portable.|

### Alternativa: ODROID-C4

| Modelo                  | Consumo Energético                | Rendimiento (CPU/RAM)       | Ventajas                       | Desventajas                    |
|-------------------------|------------------------------------|-----------------------------|--------------------------------|--------------------------------|
| **ODROID-C4**           | ~2W / ~4W                         | 4 núcleos / 4GB RAM         | Similar al Raspberry Pi 4, con mejor eficiencia energética. | Menor comunidad y soporte de software. |

## Conclusiones

Tras analizar las diferentes opciones, hemos obtenido las siguientes conclusiones en relación a las necesidades de este proyecto:

- **Raspberry Pi Zero W**: Es la opción más adecuada si se prevé un bajo volumen de tráfico web, como en el caso de una web estática. Su consumo extremadamente bajo la convierte en la candidata ideal para funcionar con un panel solar pequeño (~5W).

- **Raspberry Pi 3B+**: Representa un equilibrio razonable entre consumo y rendimiento para servidores con un tráfico moderado. Requiere un panel solar algo más potente (~10W).

- **Raspberry Pi 4**: Ideal para proyectos más exigentes que necesiten manejar bases de datos, servidores dinámicos o servicios adicionales. Sin embargo, su mayor consumo demanda una instalación solar más robusta (~20W o más).

- **ODROID-C4**: Ofrece un rendimiento similar al de la Raspberry Pi 4, pero con una mejor eficiencia energética. No obstante, su adopción puede verse limitada por la menor disponibilidad de recursos y soporte técnico en comparación con Raspberry Pi.

Inicialmente, optamos por la **Raspberry Pi Zero** W debido a su mínimo consumo energético y menor huella ambiental, lo cual la convierte en la opción más coherente con los principios de sostenibilidad del proyecto. Es perfecta para alojar una página web optimizada y con contenido ligero.

Sin embargo, por dificultades técnicas en la configuración y despliegue con este modelo —principalmente relacionadas con limitaciones de compatibilidad y rendimiento—, se decidió realizar la implementación práctica con una **Raspberry Pi 4**. Aunque no es la opción más eficiente en cuanto a consumo, su capacidad de procesamiento permite escalar el proyecto en el futuro, integrando nuevos servicios y funcionalidades sin comprometer el rendimiento.

---

⬅️ [Volver al inicio](README.md)  
➡️ [Ir a la sección de Consumo Energético](consumo.md)
