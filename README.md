# louvre-osint-investigation
Este proyecto reconstruye el robo de las Joyas de la Corona del Museo del Louvre (octubre de 2025) utilizando únicamente fuentes abiertas OSINT y técnicas de análisis pasivo.
Incluye una investigación completa, un laboratorio virtual que simula la arquitectura digital del museo y un análisis de riesgos físicos/digitales combinados.

## 📄 Presentación completa en PDF

[Abrir presentación OSINT (PDF)](docs/ROBO_EN_EL_LOUVRE_JON_ORMAECHEA_V2.pdf)

# Objetivo del proyecto
- Analizar el robo del Louvre mediante información OSINT verificada.
- Reconstruir la cronología del ataque paso a paso.
- Identificar a los sospechosos y su huella digital.
- Evaluar la infraestructura tecnológica del museo desde un enfoque pasivo.
- Diseñar un laboratorio virtual que simula el entorno corporativo del museo.
- Extraer lecciones aplicables a ciberseguridad, gestión de riesgos y respuesta ante incidentes.

# Contenido del repositorio
· docs/
Documentación completa del caso:
- cronología.md: reconstrucción minuto a minuto del ataque
- sospechosos.md: identificación y análisis OSINT de los detenidos
- analisis-osint.md: análisis físico, digital y contextual del robo
- analisis-web.md: fingerprinting y análisis pasivo del dominio louvre.fr
- lecciones.md: aprendizajes aplicables a ciberseguridad y seguridad física
- esquema-laboratorio.md: descripción del laboratorio virtual utilizado para simular la arquitectura del museo y reproducir un ataque 
- PDF original con la presentación completa del caso

· metodologia/
Cómo se realizó la investigación:
- herramientas-osint.md: herramientas utilizadas y su propósito
- flujo-investigacion.md: proceso paso a paso
- limites-legales.md: marco ético y legal del análisis OSINT

· evidencias/capturas/
Material visual que apoya el análisis:
  - cronología del ataque  
  - puntos de intrusión  
  - rutas de escape  
  - sospechosos  
  - análisis OSINT y web  

# Técnicas OSINT aplicadas
- OSINT de identidades y alias
- Análisis de redes sociales y contenido archivado
- Verificación audiovisual
- Análisis geoespacial
- Análisis de infraestructura web
- Revisión de auditorías de seguridad filtradas
- Correlación temporal y espacial
- Análisis de vehículos y matrículas
- Investigación de herramientas y equipamiento utilizado

# Herramientas y técnicas utilizadas
OSINT
- Sherlock
- Maigret
- TikTok-OSINT
- WhatsMyName
- InstantUsername
- Archive.org / Wayback Machine
- Google Earth / mapas
- Análisis de medios internacionales
- Verificación cruzada de fuentes
ANÁLISIS WEB
- DNSDumpster
- Whois
- WebCheck
- Fingerprinting tecnológico
- SQLmap (solo análisis pasivo/no intrusivo)

# Marco ético y legal
Toda la investigación se realizó:
- Sin técnicas intrusivas
- Sin escaneos activos
- Sin explotación de vulnerabilidades
- Sin acceso a información privada
- Usando exclusivamente fuentes abiertas
- Con un propósito educativo y profesional

# Limitaciones del análisis
- No hay acceso a fuentes privadas.
- Todo se basa en noticias y fuentes abiertas.
- El laboratorio es una simulación, no una reproducción real.

# Laboratorio virtual
El proyecto incluye un laboratorio que simula la arquitectura digital del museo, con dos dominios, máquinas Windows 2000/2003/2022, cámaras vulnerables y estaciones de trabajo.
Este entorno permite reproducir de forma didáctica:
- Pivoting
- Movimiento lateral
- Escalada de privilegios
- Análisis de dominios heredados
- Riesgos de interconexión entre sistemas modernos y legacy

# Lecciones clave para ciberseguridad
- La seguridad física y la digital están completamente interconectadas.
- La obsolescencia tecnológica puede convertir cualquier infraestructura en un objetivo vulnerable.
- La información pública (rutinas, proveedores, fallos previos) puede ser suficiente para planificar un ataque.
- La documentación, la correlación de datos y la verificación son habilidades esenciales para un analista SOC.

# Próximos pasos

Este proyecto está diseñado para seguir creciendo y servir como base para futuros análisis OSINT y ejercicios de laboratorio. Algunas mejoras previstas son:
- Ampliar el laboratorio virtual incorporando más escenarios de movimiento lateral, segmentación de red y simulación de fallos de seguridad.
- Automatizar parte del análisis mediante scripts que faciliten búsquedas iniciales, recopilación de metadatos y extracción de información pública.
Estas mejoras permitirán que el proyecto evolucione hacia un recurso didáctico más completo, útil tanto para estudiantes como para profesionales de ciberseguridad.

# Autor
Jon Ormaechea Caro
Analista de Ciberseguridad orientado a SOC y OSINT
Enfocado en monitorización, análisis de alertas, investigación y documentación técnica.
Contacto
- Github:@jonocaro-coder
- Linkedin:www.linkedin.com/in/jonormaecheacaro
