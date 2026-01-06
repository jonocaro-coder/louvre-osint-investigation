# Esquema de Laboratorio Virtual
Simulación controlada del entorno técnico del Museo del Louvre
Este laboratorio reproduce, en un entorno virtual y aislado, la arquitectura digital del museo tal como se describe en el informe.
Su objetivo es permitir la simulación didáctica de un ataque lateral partiendo desde un dispositivo vulnerable.

1. Topología del entorno
La red está compuesta por 7 máquinas virtuales, distribuidas en dos dominios:

1.1 Dominio moderno: museo.local
· DC MUSEO 2022
- Windows Server 2022
- IP: 192.168.100.10
- Controlador de dominio principal

· GUARDPOST
- Windows 11
- IP: 192.168.100.20
- Puesto de vigilancia

· CURADOR
- Windows 11
- IP: 192.168.100.50
- Estación del curador de arte

1.2 Dominio legado: legacy.local
· DC MUSEO 2003
- Windows Server 2003 R2
- IP: 192.168.100.11
- Controlador de dominio intermedio

· ART VAULT
- Windows 2000 Professional
- IP: 192.168.100.30
- Almacén de información sensible

· CAM 01
- Dispositivo embebido (simulado)
- IP: 192.168.100.60
- Cámara vulnerable con firmware inseguro

1.3 Atacante
- Kali Linux
- IP: 192.168.100.99
- Máquina de simulación ofensiva

2. Objetivo de la simulación
Reproducir el recorrido de ataque descrito en el informe:
- Explotación inicial desde CAM 01
- Pivoting hacia ART VAULT
- Escalada de privilegios en DC MUSEO 2003
- Movimiento lateral hacia GUARDPOST
- Acceso final a CURADOR y simulación de exfiltración

3. Consideraciones éticas
- Este laboratorio es educativo y no ofensivo
- No se simulan payloads reales ni explotación destructiva
- Las vulnerabilidades están simuladas para fines didácticos
- No se conecta a redes externas ni sistemas reales
