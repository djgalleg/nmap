CHRISTIAN_TAPIA
# Nmap Overview

NMAP funciona para realizar escaneo en todas las redes, su propósito principal es encontrar puertos abiertos y vulnerabilidades, además que posee este tipo de escaneos SYN, TCP, UDP, y SCTP para detectar servicios abiertos en un sistema objetivo.
Además, se puede optar por poner un incremento de velocidad a nmap con la opción `-T5`.
Uso de nmap en acción:

```
nmap -sS -T5 -SV $IP
```


### 🔍 ¿Para qué se usa?
- Identificar dispositivos conectados a una red.
- Detectar puertos abiertos y servicios que están corriendo.
- Determinar versiones de software y sistemas operativos.
- Realizar pruebas de seguridad y detección de vulnerabilidades.

### JUSTIFICACIÓN
El escaneo de redes, ya sea en entornos domésticos o a nivel empresarial, siempre revela puertos abiertos, latencia en la red o incluso vulnerabilidades. En este sentido, es fundamental que el profesional en redes sepa comprender y actuar de manera adecuada para analizar dicha red. Una de las herramientas más antiguas y populares es Nmap, cuyo uso se ha extendido ampliamente en retos de CTF, pentesting y análisis de redes.

Por ejemplo, la empresa CompTIA menciona que: Nmap suele considerarse una herramienta de ciberseguridad, aunque no debe subestimarse su utilidad para la resolución de problemas. Los profesionales y administradores de seguridad utilizan Nmap para diversas tareas. (Garn, 2024)

Además de la cita de arriba tomada de la empresa reconocida como COMPTIA, existe otra empresa como Red Hat que nos brinda información de lo siguiente:

Nmap (Network Mapper) es conocido popularmente como la navaja suiza del administrador de sistemas. Dado que las cosas en una red corporativa no funcionan tan bien como se desea, esos tickets de depuración o de "Guardar" pueden acumularse en el registro de trabajo. (Nandishwar, 2019)

## Aspecto | Descripción
--- | ---
**Nombre** | Nmap (Network Mapper)
**Funcionalidad principal** | Nmap es una herramienta de código abierto utilizada para el escaneo y mapeo de redes. Permite a los profesionales de la seguridad informática identificar dispositivos activos en una red, descubrir puertos abiertos y detectar servicios en ejecución, así como posibles vulnerabilidades.
**Características destacadas** | - Detección de hosts activos: Identifica qué dispositivos están conectados a la red.  
- Escaneo de puertos: Determina qué puertos están abiertos en un host específico.  
- Detección de servicios: Identifica servicios y versiones de software que se ejecutan en puertos abiertos.  
- Detección de sistemas operativos: Estima el sistema operativo y su versión en dispositivos remotos.  
- Scripting Engine (NSE): Permite la ejecución de scripts personalizados para realizar tareas específicas, como la detección de vulnerabilidades conocidas.
**Aplicaciones comunes** | - Seguridad informática: Evaluación de la seguridad de redes y sistemas mediante la identificación de posibles puntos débiles.  
- Administración de redes: Inventario de dispositivos y servicios en una red para su gestión eficiente.  
- Auditorías de cumplimiento: Verificación de configuraciones y políticas de seguridad en entornos corporativos.

Fuente: La información proporcionada en este resumen se basa en el enlace de ScienceDirect sobre la herramienta Nmap.

Nmap no solo es una herramienta de escaneo y mapeo de redes ampliamente reconocida, sino que también ofrece la posibilidad de expandir sus funcionalidades a través de la creación y personalización de scripts. La función NSE de la herramienta Nmap es una potente función que permite a los usuarios automatizar diversas tareas relacionadas con la red. La herramienta incluye una amplia biblioteca de scripts preinstalados, que pueden modificarse para satisfacer las necesidades. (Yashvant Mahadev, 2023, p. 1180)

Gracias a su motor de secuencias de comandos (NSE, por sus siglas en inglés), los usuarios pueden desarrollar scripts propios para automatizar tareas específicas, como la detección de vulnerabilidades, la identificación de servicios ocultos o el análisis profundo de la seguridad en la red.

Nmap, abreviatura de "Network Mapper", es una herramienta de código abierto utilizada para la exploración de redes y auditorías de seguridad. Permite a los administradores de red identificar dispositivos activos en una red, descubrir puertos y servicios abiertos, y detectar vulnerabilidades. Nmap puede adaptarse a las condiciones de la red, incluyendo latencia y congestión, durante un escaneo. ("Nmap: the Network Mapper", s.f.)

## Bibliografía
- Garn, D. (2024, Marzo 6). Blog: Comptia. comptia.org Web site: https://www.comptia.org/blog/what-is-nmap
- Liao, S., Zhou, C., Zhao, Y., & Zhang, Z. (2020). A Comprehensive Detection Approach of Nmap: Principles, Rules and Experiments. International Conference on Cyber-Enabled Distributed Computing and Knowledge Discovery. https://doi.org/10.1109/CyberC49757.2020.00020
- Nandishwar, S. (2019, Agosto 19). RedHat Blog. redhat.com Web site: https://www.redhat.com/en/blog/use-cases-nmap
- Yashvant Mahadev, H. (2023). A Review on Nmap and Its Features. International Research Journal of Engineering and Technology, 10(05 | May 2023), 1176-1180.
- Nmap: the Network Mapper - Free Security Scanner. (s.f.). Nmap. https://nmap.org/

=======
NMAP
AMY_GARAY
1) UTILIDAD DEL REPOSITORIO
DARIO_GALLEGOS
Nmap es una herramienta crucial en el campo de la ciberseguridad, especialmente en el contexto de las pruebas de penetración y el análisis de redes. Su capacidad para realizar escaneos de puertos, detectar servicios y obtener detalles sobre sistemas operativos hace de Nmap una opción robusta para mapear redes y descubrir vulnerabilidades. Con opciones avanzadas como el Nmap Scripting Engine (NSE), los profesionales pueden ejecutar scripts automatizados para detectar fallos de seguridad específicos. Además, su capacidad de escaneo pasivo y activo ofrece flexibilidad para adaptarse a diferentes escenarios y políticas de seguridad. La eficiencia y precisión de Nmap lo convierten en una herramienta indispensable para auditar la infraestructura de red en busca de puntos débiles que puedan ser explotados por atacantes.

3) JUSTIFICACIÓN
Nmap es una herramienta excelente debido a su capacidad de realizar escaneos profundos y detallados de redes, lo que permite una evaluación precisa de la seguridad de los sistemas. Su flexibilidad para realizar análisis tanto activos como pasivos asegura que los profesionales puedan operar de manera discreta o invasiva según el contexto de la prueba de penetración. Además, su integración con el Nmap Scripting Engine (NSE) amplifica la utilidad de la herramienta, permitiendo a los usuarios ejecutar scripts personalizados para detectar vulnerabilidades específicas de manera automatizada. Esto hace que Nmap no solo sea fácil de usar, sino también extremadamente potente y adaptable a diversos entornos de red, lo que lo convierte en un estándar de facto en la seguridad informática.

   Identifica sistemas operativos y versiones de software a través de fingerprinting con -O y -sV
   Se usa en pruebas de penetración para obtener una visión detallada de la superficie de ataque de una red.
   Técnicas de evasión como fragmentación de paquetes (-f), modificación de TTL (--ttl) o camuflaje de origen (-S, -D) para analizar reglas de firewall.
   Se puede ejecutar en modo agente distribuido mediante nmap -iL para escanear múltiples objetivos simultáneamente
3) JUSTIFICACIÓN
   El repositorio de Nmap no solo ofrece una herramienta de escaneo de puertos, sino que proporciona un framework avanzado de auditoría de redes y seguridad ofensiva, esencial en cualquier kit de pentesting o administración de redes. Su versatilidad lo hace útil tanto para atacantes éticos como para defensores de ciberseguridad
4) REFERENCIAS
   Patel, R., & Singh, A. (2023). Use Nmap like a Pro: A Beginner's Guide for Aspiring Security Professionals. ResearchGate. https://www.researchgate.net/publication/387953667

Kumar, S. (2022). A Case Study on Nmap - Network Mapper. Academia.edu. https://www.academia.edu/34856706

Gómez, J., & López, M. (2021). Análisis de las vulnerabilidades del sistema de información utilizando herramientas de ciberseguridad. Universidad Politécnica Salesiana. https://dspace.ups.edu.ec/bitstream/123456789/25183/4/UPS-CT010619.pdf

Chen, L., & Brown, T. (2023). A Comparative Analysis of Port Scanning Tool Efficacy. arXiv. https://arxiv.org/abs/2303.11282

1) NMAP funciona para raelizar escaneo en todas las redes, su proposito principal es encontrar puertos abiertos y vulnerabilidades ademas que posee este tipo de escaneos SYN, TCP, UDP, y SCTP para detectar servicios abiertos en un sistema objetivo.

Ademas se puede optar por poner velocidad a nmap con la opcion -T5
2) 🔍 ¿Para qué se usa?
-Identificar dispositivos conectados a una red.
-Detectar puertos abiertos y servicios que están corriendo.
-Determinar versiones de software y sistemas operativos.
-Realizar pruebas de seguridad y detección de vulnerabilidades.
-Identifica sistemas operativos y versiones de software a través de fingerprinting con -O y -sV
-Se usa en pruebas de penetración para obtener una visión detallada de la superficie de ataque de una red.
-Técnicas de evasión como fragmentación de paquetes (-f), modificación de TTL (--ttl) o camuflaje de origen (-S, -D) para analizar reglas de firewall.
-Se puede ejecutar en modo agente distribuido mediante nmap -iL para escanear múltiples objetivos simultáneamente
4) JUSTIFICACIÓN
Nmap, abreviatura de "Network Mapper", es una herramienta de código abierto utilizada para la exploración de redes y auditorías de seguridad. Permite a los administradores de red identificar dispositivos activos en una red, descubrir puertos y servicios abiertos, y detectar vulnerabilidades. Nmap puede adaptarse a las condiciones de la red, incluyendo latencia y congestión, durante un escaneo.("Nmap: the Network Mapper", s.f.)
El repositorio de Nmap no solo ofrece una herramienta de escaneo de puertos, sino que proporciona un framework avanzado de auditoría de redes y seguridad ofensiva, esencial en cualquier kit de pentesting o administración de redes. Su versatilidad lo hace útil tanto para atacantes éticos como para defensores de ciberseguridad.

6) Referencia:

Nmap: the Network Mapper - Free Security Scanner. (s.f.). Nmap. https://nmap.org/


master


# Nmap - Network Mapper

Nmap es “Network Mapper”una herramienta de código abierto para la red exploración y auditoría de la seguridad. Fue diseñado para rápidamente escanean grandes redes, aunque funciona bien contra single anfitriones. Nmap utiliza paquetes IP crudos de maneras novedosas para determinar qué Los anfitriones están disponibles en la red, qué servicios (aplicación nombre y versión) que ofrecen esos hosts, qué sistemas operativos (y versiones del sistema operativo) están en ejecución, qué tipo de paquetes filtros/cortales están en uso, y docenas de otros características. Mientras que Nmap se utiliza comúnmente para auditorías de seguridad, muchos sistemas y administradores de redes lo encuentran útil para la rutina tareas como inventario de la red, gestión de la actualización del servicio horarios, y monitorear el tiempo de actividad o servicio


**`nmap -A -T4 scanme.nmap.org`**Reporte de escaneo de mapa de Nmap para scanme.nmap.org (74.207.244.221)
El anfitrión se levanta (0.029s latencia).
rDNS récord para 74.207.244.221: li86-221.members.linode.com
No mostrado: 995 puertos cerrados
PORT ESTADO SERVICIO VERSION
22/tcp open ssh OpenSSH 5.3p1 Debian 3ubuntu7 (protocolo 2.0)
* ssh-hostkey: 1024 8d:60:f1:7c:ca:b7:3d:0a:d6:67:54:9d:69:d9:b9:dd (DSA)
No2048 79:f8:09:ac:d4:e2:32:42:10:49:d3:bd:20:82:85:ec (RSA)
80/tcp abierto http Apache httpd 2.2.14 ((Ubuntu))
- Título: Adelante y escanearme.
646/tcp filtrado ldp
1720/tcp filtrado H.323/Q.931
9929/tcp open nping-echo eco de Nping
Tipo de dispositivo: propósito general
Corrida: Linux 2.6. X
OS CPE: cpe:/o:linux:linux-kernel:2.6.39
Detalles del sistema operativo: Linux 2.6.39
Distancia de la red: 11 lúpulo
Información del servicio: OS: Linux; CPE: cpe:/o:linux:kernel

TRACEROUTE (utilización del puerto 53/tcp)
HOP RTT ADDRESS
[Cortar los primeros 10 lúpulo para la brevedad]
11 17.65 ms li86-221.members.linode.com (74.207.244.221)

Maestación hecha: 1 dirección IP (1 host up) escaneada en 14.40 segundos


 Luis_Pacheco
# Referencias  20

- https://nmap.org/book/man.html#man-ex-repscan
- https://www.freecodecamp.org/news/what-is-nmap-and-how-to-use-it-a-tutorial-for-the-greatest-scanning-tool-of-all-time/

# Por qué usar Nmap?

Nmap es una herramienta que permite trazar rápidamente una red sin necesidad de comandos sofisticados ni configuraciones complejas. Puede utilizarse tanto con comandos simples, como para comprobar si un host está activo, como con scripting avanzado a través de su Motor de Scripting Nmap.

### Características principales de Nmap:

-   **Reconocimiento de dispositivos:** Detecta rápidamente todos los dispositivos conectados a la red, incluyendo servidores, routers, interruptores, dispositivos móviles, entre otros.
-   **Identificación de servicios:** Permite conocer qué servicios se ejecutan en un sistema, como servidores web, servidores DNS y otras aplicaciones comunes. También puede detectar versiones de aplicaciones con una precisión razonable, facilitando la identificación de vulnerabilidades.
-   **Detección del sistema operativo:** Obtiene información detallada sobre el sistema operativo de los dispositivos, incluyendo versiones específicas, lo que resulta útil en pruebas de penetración.
-   **Escaneo de seguridad y vulnerabilidades:** Puede ejecutar scripts del Motor de Scripting Nmap para realizar auditorías de seguridad y ataques controlados a los sistemas analizados.
-   **Interfaz gráfica (Zenmap):** Incluye una interfaz gráfica llamada Zenmap, que permite desarrollar mapas visuales de la red para mejorar la usabilidad y el análisis de reportes.

# Referencias

https://nmap.org/book/man.html#man-ex-repscan
https://www.freecodecamp.org/news/what-is-nmap-and-how-to-use-it-a-tutorial-for-the-greatest-scanning-tool-of-all-time/
 master
 master
 master
