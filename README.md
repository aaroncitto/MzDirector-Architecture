MzDirector: Portal de Reporting Corporativo Interactivo
Aviso de Confidencialidad: Debido a políticas de privacidad y protección de datos corporativos, este documento opera exclusivamente como una Auditoría de Arquitectura Técnica. No se exponen archivos binarios .pbix, conjuntos de datos reales ni código fuente propietario asociado a la lógica de negocio.

Resumen Ejecutivo
Diseño y desarrollo de un portal de cuadros de mando corporativo de alto rendimiento. El proyecto superó las limitaciones visuales estándar de las herramientas de Business Intelligence mediante la inyección de código front-end (HTML/SVG) para crear una experiencia de navegación interactiva, respaldada por un modelado de datos robusto.

Stack Tecnológico
Motor Analítico & BI: Power BI, Lenguaje M (Power Query), DAX.

Desarrollo UI/UX: HTML, SVG, CSS (Glassmorphism).

1. El Problema de Negocio
Los sistemas de reporting corporativo tradicionales presentaban una experiencia de usuario (UX) rígida, con navegación lineal y estética plana. Se requería centralizar múltiples flujos de datos en un entorno único que funcionara visual y operativamente como una aplicación web nativa, no como un informe estático.

2. Solución Arquitectónica
A. Ingeniería Front-End (UI Avanzada)
Para romper las limitaciones nativas del lienzo, se desarrolló una interfaz híbrida:

Contenedores Glassmorphic: Implementación de tarjetas visuales mediante código HTML y SVG renderizado dinámicamente. Se ajustaron niveles de opacidad precisos (backdrop-blur) para evitar transparencias absolutas o blancos planos, garantizando la legibilidad sobre fondos oscuros.

Navegación Interactiva: Integración de menús de vídeo incrustados para guiar el flujo del usuario entre los distintos cuadros de mando, simulando la experiencia de un portal web.

B. Modelado de Datos y Rendimiento
La capa visual se sustentó en una base de datos analítica optimizada para la escalabilidad:

Lenguaje M (ETL): Diseño de flujos de transformación de datos complejos para limpiar, unificar y estructurar orígenes dispares antes de su carga en el modelo en memoria.

Cálculo Computacional (DAX): Desarrollo de medidas iterativas e inteligencia de tiempo avanzadas. El modelo relacional fue optimizado para reducir la latencia de las consultas, permitiendo que la interfaz interactiva respondiera en tiempo real frente a millones de registros.

3. Impacto y Conclusión
MzDirector demuestra la viabilidad de fusionar el Desarrollo Front-End con el Business Intelligence. El resultado fue una herramienta de toma de decisiones corporativa que no solo asegura la integridad y el rendimiento del dato, sino que eleva la adopción del usuario mediante un diseño de interfaz de vanguardia.
