# Placa Solar

Para alimentar una Raspberry Pi 4 con un consumo de 1.5 A/h, necesitarás una placa solar que pueda generar suficiente energía. Si consideramos una placa solar de 100 W, y suponiendo que recibes un promedio de 5 horas de sol pico al día, la producción diaria de la placa sería:

$$Producción \ diaria = 100 \ W \times 5 \ h = 500 \ Wh$$

Dado que la Raspberry Pi consume 432 Wh al día (1.5 A a 12 V), una sola placa de 100 W sería suficiente para cubrir el consumo diario, siempre y cuando se utilice un sistema de almacenamiento adecuado (batería).

## Montaje del Sistema Solar

### Componentes necesarios

- Placa solar (100 W)
- Controlador de carga
- Batería 
- Inversor (si la Raspberry Pi requiere corriente alterna)
- Cables y conectores

### Conexión

1. Conecta la placa solar al controlador de carga.
2. Conecta el controlador de carga a la batería.
3. Si es necesario, conecta el inversor a la batería y luego a la Raspberry Pi.



Inicio -> **[Volver al inicio ](README.md)**  
Anterior -> **[Consumo Energético](consumo.md)**  
Siguiente -> **[Placa Solar ](placaSolar.md)** 

