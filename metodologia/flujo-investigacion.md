# Flujo de investigación OSINT
Proceso completo seguido para reconstruir el robo al Museo del Louvre utilizando únicamente fuentes abiertas.

1. Definición del objetivo
El propósito inicial fue reconstruir el robo del 19 de octubre de 2025 mediante técnicas OSINT, con tres metas principales:
- Analizar el ataque paso a paso usando información pública.
- Identificar a los sospechosos y verificar su presencia digital.
- Extraer lecciones de ciberseguridad y seguridad física aplicables a infraestructuras críticas.
Este enfoque se mantuvo durante toda la investigación para evitar desviaciones o especulación.

2. Recolección inicial de información (Gathering)
Se recopiló información procedente de:
- Medios internacionales (NYT, BBC, Le Monde, The Guardian, El País, etc.)
- Comunicados oficiales del Ministerio de Cultura y fiscalía de París
- Informes de auditoría previos (ANSSI 2014, INHESJ 2017, Tribunal de Cuentas 2019–2024)
- Material audiovisual verificado (BFMTV, BBC Verify, cámaras del museo)
- Información técnica del dominio louvre.fr
- Registros públicos de DNS, hosting y servidores
- Publicaciones en redes sociales relacionadas con los sospechosos

3. Clasificación de la información
Toda la información recopilada se organizó en cuatro bloques:
- Cronología del ataque
- Identificación de sospechosos
- Análisis OSINT (físico, digital y contextual)
- Análisis web del dominio del museo
Esta clasificación permitió trabajar cada área de forma independiente y evitar mezclar datos no relacionados.

4. Verificación cruzada (Cross-checking)
Cada dato se contrastó con múltiples fuentes para asegurar su fiabilidad:
- Horarios del ataque verificados con BBC Verify, BFMTV y NYT
- Rutas de escape confirmadas con mapas y geolocalización
- Identidades contrastadas con herramientas OSINT de alias
- Auditorías de seguridad comparadas con fallos explotados por los ladrones
- Información técnica del dominio validada con DNSDumpster, Whois y WebCheck
Este proceso permitió reconstruir una cronología precisa y coherente.

5. Análisis técnico y contextual
5.1. Análisis físico del ataque
- Confirmación del balcón utilizado
- Identificación del montacargas Böcker
- Verificación del uso de amoladoras eléctricas
- Análisis de vitrinas, resistencia y métodos de corte
- Validación de la ruta de huida hacia el Sena

5.2. Análisis digital
- Revisión de auditorías ANSSI e INHESJ
- Identificación de sistemas obsoletos (Windows 2000, XP, Server 2003)
- Riesgos derivados de contraseñas débiles (“LOUVRE”)
- Interconexión peligrosa entre redes internas y sistemas de seguridad

5.3. Análisis web
- Fingerprinting tecnológico del dominio
- Identificación de hosting, WAF, certificados y servidores
- Comprobación pasiva con SQLmap (sin explotación)

6. Análisis de actores y presencia digital
Se investigaron los perfiles de los sospechosos mediante:
- Sherlock
- Maigret
- TikTok-OSINT
- WhatsMyName
- InstantUsername
- Archive.org / Wayback Machine
Resultados clave:
- La mayoría de perfiles estaban eliminados o privados
- Solo se accedió a contenido a través de terceros
- Se confirmó la identidad digital histórica de Doudou Cross Bitume mediante vídeos antiguos

7. Síntesis y elaboración del informe
Toda la información verificada se integró en:
- Cronología detallada del ataque
- Identificación de sospechosos
- Análisis OSINT (físico, digital y contextual)
- Análisis web del dominio
- Lecciones aprendidas para ciberseguridad y gestión de riesgos
El resultado final es un informe estructurado, verificable y útil para profesionales de ciberseguridad.

8. Principios aplicados durante la investigación
- No intrusión: ninguna técnica activa o ilegal
- Uso exclusivo de fuentes abiertas
- Respeto a la privacidad
- Verificación cruzada obligatoria
- Documentación clara y reproducible
