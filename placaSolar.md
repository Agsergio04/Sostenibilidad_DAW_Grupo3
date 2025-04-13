# Placa Solar

Para alimentar una **Raspberry Pi 4**, que consume **1.5A a 5V** (lo que equivale a **7.5 W** por hora si está funcionando de manera continua), se necesita una **placa solar** capaz de generar suficiente energía para cubrir ese consumo.

Si utilizamos una **placa solar de 20 W** y asumimos un promedio de **5 horas de sol pico al día**, la producción diaria de la placa sería:

$$
Producción \ diaria = 20 \ W \times 5 \ h = 100 \ Wh
$$

Dado que la **Raspberry Pi 4** consume aproximadamente **7.5 W al día**, una **placa solar de 20 W** sería más que suficiente para cubrir el consumo diario de la Raspberry Pi, siempre y cuando se utilice un sistema de almacenamiento adecuado (como una batería).

## Montaje del Sistema Solar

### Componentes necesarios

- **Placa solar** (20 W)
- **Controlador de carga** (para gestionar la carga de la batería)
- **Batería** (para almacenamiento de energía)
- **Cables y conectores** (para las conexiones eléctricas)

### Conexión

1. Conecta la **placa solar** al **controlador de carga**.
2. Conecta el **controlador de carga** a la **batería** para almacenar la energía generada.
3. Conecta la **batería** a la **Raspberry Pi** (usualmente mediante un **regulador de 5V** para asegurar que la Raspberry reciba la cantidad adecuada de voltaje).

---

### Navegación

⬅️ **[Volver al inicio](README.md)**  
⬅️ **[Ir a Consumo Energético](consumo.md)**  
➡️ **[Ir a Montaje del Servidor](servidor.md)**  
