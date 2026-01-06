# louvre-osint-investigation
Investigación OSINT completa basada exclusivamente en fuentes abiertas para reconstruir el robo de las Joyas de la Corona en el Museo del Louvre.
El proyecto analiza la cronología del ataque, identifica a los sospechosos, evalúa fallos de seguridad física y digital, y revisa la infraestructura web del museo para entender cómo un incidente de este nivel pudo ocurrir.

## 📄 Presentación completa en PDF

[Abrir presentación OSINT (PDF)](docs/ROBO_EN_EL_LOUVRE_JON_ORMAECHEA_V2.pdf)

# Objetivo del proyecto
Este trabajo busca demostrar cómo un analista puede:
- Correlacionar información dispersa procedente de medios, redes sociales y fuentes públicas.
- Reconstruir un incidente real aplicando metodología OSINT.
- Identificar fallos de seguridad física, digital y organizativa.
- Extraer lecciones aplicables a entornos SOC y equipos de respuesta ante incidentes.

# Contenido del repositorio
· docs/
Documentación completa del caso:
- cronología.md — reconstrucción minuto a minuto del ataque
- sospechosos.md — identificación y análisis OSINT de los detenidos
- analisis-osint.md — análisis físico, digital y contextual del robo
- analisis-web.md — fingerprinting y análisis pasivo del dominio louvre.fr
- lecciones.md — aprendizajes aplicables a ciberseguridad y seguridad física
- PDF original con la presentación completa del caso

· metodologia/
Cómo se realizó la investigación:
- herramientas-osint.md — herramientas utilizadas y resultados
- flujo-investigacion.md — proceso paso a paso
- limites-legales.md — marco ético y legal aplicado

· evidencias/
Espacio reservado para:
- Capturas relevantes
- Resultados de herramientas
- Material de apoyo

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

# Lecciones clave para ciberseguridad
- La seguridad física y la digital están completamente interconectadas.
- La obsolescencia tecnológica puede convertir cualquier infraestructura en un objetivo vulnerable.
- La información pública (rutinas, proveedores, fallos previos) puede ser suficiente para planificar un ataque.
- La documentación, la correlación de datos y la verificación son habilidades esenciales para un analista SOC.

# Autor
Jon Ormaechea Caro
Analista de Ciberseguridad orientado a SOC y OSINT
Enfocado en monitorización, análisis de alertas, investigación y documentación técnica.
