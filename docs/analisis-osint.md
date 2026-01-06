# Análisis OSINT
Análisis detallado del robo al Museo del Louvre desde la perspectiva OSINT, integrando información física, digital, técnica y contextual obtenida exclusivamente de fuentes abiertas.

1. Análisis del vector de acceso físico
Los ladrones explotaron una combinación de vulnerabilidades estructurales y rutinas operativas previsibles.

1.1. Balcón vulnerable identificado en auditorías previas
- Auditorías de 2018 ya habían señalado el balcón utilizado como punto crítico de acceso.
- Se mencionaba incluso la posibilidad de usar un montacargas para alcanzarlo.
- Esta información fue confirmada posteriormente por Le Monde

1.2. Ventanas sin refuerzo
- Las ventanas de la Galería de Apolo no estaban reforzadas.
- Las amoladoras eléctricas utilizadas por los ladrones cortaron el vidrio en segundos.
- El museo confirmó que los cristales y paneles de madera no resistieron.

1.3. Herramientas empleadas
Los ladrones utilizaron herramientas idénticas a las recomendadas en el manual contra incendios del Louvre para abrir vitrinas en emergencias:
- Amoladoras eléctricas
- Herramientas de corte especializadas
- Equipamiento portátil de alta potencia
Estas herramientas están diseñadas para abrir vitrinas resistentes a 140 golpes de martillo o hacha, lo que explica la rapidez del ataque.

2. Análisis del montacargas Böcker
El montacargas utilizado fue un elemento clave del ataque.

2.1. Identificación del modelo
- La empresa Böcker reconoció públicamente el modelo tras ver las imágenes en prensa.
- Confirmó que la máquina había sido robada durante una demostración solicitada por los propios ladrones.

2.2. Coincidencia con equipos usados en el Louvre
- El modelo era idéntico a los utilizados en restauraciones periódicas del museo.
- Esto sugiere conocimiento previo de los procedimientos internos.

2.3. Manipulación del equipo
- Los ladrones retiraron el logo del cliente.
- Cambiaron la matrícula para dificultar la trazabilidad

3. Análisis de la matrícula EV‑698‑HA
La matrícula del montacargas fue analizada mediante herramientas OSINT.

3.1. Limitaciones legales
La legislación francesa impide obtener datos personales del propietario mediante el SIV.

3.2. Herramientas utilizadas
- Gideon: sin resultados.
- Siv-auto.fr: error de servidor.
- LicensePlatesMania:
- Código 75 → París
- Símbolo rojo → Île-de-France

3.3. Conclusión
Solo fue posible obtener información geográfica, no datos personales

4. Análisis de fallos de seguridad digital
Las auditorías previas revelan un entorno tecnológico obsoleto y vulnerable.

4.1. Auditoría ANSSI (2014)
- Uso de Windows 2000 en la red de oficinas.
- Servidor de videovigilancia con contraseña “LOUVRE”.
- Usuario “THALES” con acceso a la aplicación de videovigilancia.

4.2. Auditoría INHESJ (2017)
- Estaciones con Windows 2000/XP.
- Servidores con Windows Server 2003.
- Falta de segmentación adecuada entre redes internas y sistemas de seguridad.

4.3. Tribunal de Cuentas (2019–2024)
- Retrasos significativos en la modernización.
- Proyectos de videovigilancia pospuestos repetidamente.
- Falta de coordinación entre departamentos técnicos.

4.4. Riesgo crítico identificado
La interconexión entre redes administrativas y sistemas de seguridad permitía, en caso de intrusión:
- Manipulación física mediante acceso informático
- Escalada lateral
- Riesgo sistémico para la videovigilancia

5. Análisis del ecosistema de videoprotección (PVPP)
El Louvre forma parte del Plan de Videoprotección para París (PVPP).
Hallazgos clave
- El museo es socio de videoprotección con la Prefectura de Policía.
- Sus flujos de vídeo pueden ser redirigidos mediante convenios específicos.
- Aunque no hay pruebas de explotación, la combinación de:
- interconexión estructural
- sistemas obsoletos
- retrasos en modernización
lo convierten en un eslabón débil potencial dentro del ecosistema de videovigilancia parisino.

6. Análisis de la fuga
Los ladrones huyeron en dos Yamaha TMAX, confirmadas por múltiples fuentes.
Puntos clave
- ADN encontrado en uno de los scooters.
- Cámaras captaron la salida hacia el sur, dirección autopista A6.
- Un guardia evitó que incendiaran el camión.
- Las imágenes no permiten identificar matrículas ni modelos con precisión, pero todas las crónicas coinciden en el uso de TMAX.

7. Contacto con CGI Group y la dark web
Una empresa israelí de inteligencia privada, CGI Group, afirmó:
- Haber sido contactada por los ladrones mediante un mensaje cifrado.
- Se les ofreció negociar la venta de las joyas en la dark web.
- Mantuvieron conversaciones codificadas durante 24 horas.
- El Louvre no respondió a la intermediación.
La empresa también afirmó que:
- La IA les permite rastrear amenazas en línea.
- Habían detectado conversaciones previas sobre planes para robar el Louvre.

8. Conclusión del análisis OSINT
El robo fue posible gracias a una combinación de:
- Vulnerabilidades físicas (balcón, ventanas, vitrinas)
- Fallas organizativas (rutinas previsibles, falta de refuerzo)
- Obsolescencia tecnológica (sistemas antiguos, contraseñas débiles)
- Interconexión peligrosa entre redes internas y sistemas de seguridad
- Conocimiento previo de procedimientos y equipamiento del museo
- Ejecución rápida y precisa (3 min 57 s dentro de la galería)
El caso demuestra cómo la seguridad física y la ciberseguridad están profundamente conectadas, y cómo un atacante puede explotar información pública, fallos estructurales y tecnología obsoleta para ejecutar un ataque de alto impacto.
