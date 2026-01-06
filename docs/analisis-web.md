# Análisis Web del dominio louvre.fr
Análisis técnico del dominio oficial del Museo del Louvre utilizando únicamente técnicas OSINT pasivas y fuentes abiertas.

1. Información general del dominio
El dominio louvre.fr presenta una infraestructura externalizada y gestionada por un proveedor especializado.

1.1. IP principal
195.157.4.140

1.2. Proveedor
Claranet, empresa europea de servicios gestionados.

1.3. ASN
AS8426 (Claranet)

1.4. Ubicación del servidor
Ashford (TW15), Inglaterra
Conclusión:
El museo delega su infraestructura web en un proveedor externo, lo que mejora disponibilidad y resiliencia, pero también implica dependencia operativa.

2. Servidores DNS autoritativos
El dominio utiliza servidores DNS de Claranet:
- ns0.fr.claradns.net
- ns1.fr.claradns.net
- ns2.fr.claradns.net
Observación:
La redundancia DNS está correctamente distribuida entre múltiples servidores.

3. Tecnologías detectadas (Fingerprinting pasivo)

3.1. Seguridad web
- Certificado HTTPS válido emitido por Let’s Encrypt.
- Redirección automática de HTTP a HTTPS.
- Configuración estándar y actualizada.

3.2. Servidor web
- nginx como servidor backend.
- Varnish / WADP como capa de caché y proxy inverso.

3.3. Protección
- Presencia de WAF gestionado por Claranet.
- Arquitectura orientada a disponibilidad y mitigación de ataques comunes.
Conclusión:
La superficie de ataque web es reducida y bien protegida mediante servicios gestionados.

4. Resultados de DNSDumpster
El análisis pasivo con DNSDumpster reveló:
- Infraestructura distribuida entre Claranet y OVHcloud.
- Servicios expuestos mínimos.
- Banners genéricos (openresty), sin información sensible.
- No se detectaron subdominios vulnerables ni configuraciones inseguras.
Interpretación:
La arquitectura está diseñada para ocultar detalles internos y minimizar exposición.

5. Análisis con WebCheck
WebCheck confirmó:
- Coincidencia de los servidores DNS autoritativos.
- CNAMEs asociados a Claranet.
- Fingerprinting consistente con nginx y Varnish.
- No se detectaron cabeceras inseguras relevantes.

6. SQLmap (modo pasivo, sin explotación)
Se realizó una comprobación pasiva para observar el comportamiento del sitio ante solicitudes básicas:
- El dominio responde con un 301 redirect hacia https://www.louvre.fr/.
- No se realizaron pruebas intrusivas ni payloads.
- No se detectaron comportamientos anómalos.

7. Conclusiones del análisis web
El dominio louvre.fr funciona sobre una infraestructura gestionada por Claranet, lo que implica que gran parte de la seguridad y el mantenimiento recaen en un proveedor especializado. La web pública está bien protegida: usa HTTPS correctamente, cuenta con un WAF activo y combina nginx con Varnish para mejorar rendimiento y filtrar tráfico no deseado. Además, la información expuesta hacia el exterior es mínima, lo que reduce la superficie de ataque.
Sin embargo, este buen estado de la web contrasta con la situación interna del museo descrita en las auditorías filtradas. Mientras la parte pública muestra una configuración moderna y estable, los sistemas internos arrastraban problemas serios: equipos obsoletos, contraseñas débiles y una red mal segmentada que conectaba áreas administrativas con sistemas de seguridad. Esto deja claro que el punto débil no estaba en la web externa, sino en la infraestructura interna del museo, que llevaba años sin actualizarse.
