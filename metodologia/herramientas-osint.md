# Herramientas OSINT utilizadas
Listado detallado de las herramientas empleadas durante la investigación OSINT del robo al Museo del Louvre, junto con su propósito y los resultados obtenidos.

1. Herramientas para búsqueda de identidades y perfiles digitales
Sherlock
- Uso: búsqueda de un nombre de usuario en múltiples plataformas.
- Aplicación en el caso: se utilizó para localizar perfiles asociados a doudou.cross.bitu.
- Resultado: no se encontraron perfiles activos; solo referencias archivadas en sitios como Archive.org y BlitzTactics.

Maigret
- Uso: búsqueda masiva de perfiles asociados a un alias.
- Aplicación: análisis del alias doudou.cross.bitu.
- Resultado: error técnico en la ejecución, sin resultados concluyentes.

TikTok-OSINT
- Uso: extracción de metadatos y análisis de cuentas de TikTok.
- Aplicación: investigación del usuario doudou.cross.bitu.
- Resultado: no se encontraron perfiles activos; la cuenta parece eliminada o privada.

WhatsMyName
- Uso: comprobación de alias en más de 600 plataformas.
- Resultado: 0 coincidencias, lo que refuerza la hipótesis de perfiles eliminados tras las detenciones.

InstantUsername / SocialSearcher
- Uso: búsqueda rápida de alias y menciones en redes sociales.
- Resultado: coincidencias indirectas a través de terceros (vídeos antiguos, menciones en prensa y redes).

Archive.org / Wayback Machine
- Uso: recuperación de contenido eliminado o no disponible.
- Resultado: no existían capturas archivadas de los perfiles investigados.

2. Herramientas para análisis técnico y web
DNSDumpster
- Uso: enumeración de DNS, servidores, infraestructura y ubicaciones.
- Aplicación: análisis del dominio louvre.fr.
- Resultado:
- Infraestructura alojada en Claranet
- Servidores NS: ns0.fr.claradns.net, ns1.fr.claradns.net, ns2.fr.claradns.net
- Presencia de WAF y capa de caché Varnish

Whois / RDAP
- Uso: obtención de información de registro del dominio.
- Resultado:
- IP principal: 195.157.4.140
- ASN: AS8426 (Claranet)
- Hosting externalizado y protegido

WebCheck
- Uso: fingerprinting tecnológico.
- Resultado:
- nginx como servidor backend
- Certificado HTTPS válido 
- Redirección automática a HTTPS

SQLmap (modo pasivo)
- Uso: comprobación de comportamiento básico del sitio (sin explotación).
- Resultado:
- Redirección 301 a https://www.louvre.fr/
- No se realizaron pruebas intrusivas

3. Herramientas para análisis geoespacial y verificación visual
Google Earth / Mapas
- Uso: verificación de rutas, balcones, ángulos de cámaras y accesos.
- Aplicación:
- Confirmación del balcón usado por los ladrones
- Verificación de la ruta de escape hacia el Sena
- Identificación de la ubicación del montacarga

BBC Verify / BFMTV / CNN
- Uso: análisis de vídeo y verificación de imágenes.
- Resultado:
- Confirmación del ángulo de grabación
- Validación del tiempo real del ataque (3 min 57 s)

4. Herramientas para análisis de vehículos y matrículas
Gideon
- Uso: búsqueda de matrículas internacionales.
- Resultado: sin datos concluyentes para EV-698-HA.

Siv-auto.fr
- Uso: consulta del sistema francés SIV.
- Resultado: error de servidor; sin información disponible.

LicensePlatesMania
- Uso: identificación de códigos regionales.
- Resultado:
- Código 75 → París
- Símbolo rojo → Île-de-France

5. Herramientas para análisis de contenido multimedia
YouTube / Vimeo / TikTok
- Uso: análisis de vídeos antiguos del sospechoso Doudou Cross Bitume.
- Resultado:
- Identificación de acrobacias en moto
- Confirmación de su presencia digital histórica
- Relación con el entorno urbano de Seine-Saint-Denis

6. Herramientas para análisis documental y auditorías
Informes ANSSI (2014) y INHESJ (2017)
- Uso: análisis de fallos de seguridad previos.
- Hallazgos clave:
- Uso de Windows 2000/XP
- Contraseñas débiles (“LOUVRE”)
- Interconexión peligrosa entre redes internas y sistemas de seguridad

Tribunal de Cuentas (2019–2024)
- Uso: evaluación de retrasos en modernización.
- Resultado:
- Proyectos de videovigilancia pospuestos
- Falta de coordinación técnica
- Riesgo estructural elevado

