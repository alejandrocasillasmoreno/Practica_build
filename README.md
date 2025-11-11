✅ Tarea Específica
Extiende la implementación existente del Patrón Builder para incluir el componente Monitor, siguiendo la misma estructura y principios de diseño que el resto del sistema.

🔧 Requisitos Técnicos
1. Enum Inmutable para Conexiones
Crea un objeto congelado (Object.freeze()) que defina los tipos de conexión permitidos

Debe incluir al menos: HDMI, DISPLAY_PORT y VGA

El objeto debe ser inmutable para prevenir modificaciones

2. Clase Monitor con Validaciones
La clase Monitor debe:

Recibir tres parámetros: pulgadas, color, conexion

Implementar validaciones en el constructor:

pulgadas: entre 15 y 50 pulgadas

color: no puede estar vacío

conexion: debe ser uno de los valores del enum

3. Integración en el Patrón Existente
Clase Ordenador: Añadir propiedad monitor y actualizar toString()

Clase OrdenadorBuilder:

Inicializar propiedad monitor en el constructor

Crear método withMonitor() que retorne this

Añadir validaciones opcionales en build()

4. Demostración Funcional
Actualizar ambos ejemplos (ordenador básico y gaming) para incluir monitores

Verificar que la salida en consola muestre correctamente la información del monitor

