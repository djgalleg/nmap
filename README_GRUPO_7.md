# NMAP: Network Mapper

## NMAP Overview
Nmap es una herramienta utilizada para el escaneo de redes, cuyo principal propósito es encontrar puertos abiertos y vulnerabilidades. Posee diferentes tipos de escaneos, como SYN, TCP, UDP y SCTP, que permiten detectar servicios abiertos en un sistema objetivo. Además, se puede incrementar la velocidad de escaneo con la opción `-T5`.

### Uso de Nmap en acción:
```bash
nmap -sS -T5 -SV $IP
```

## 🔍 Utilidad del repositorio NMAP
- Identificar dispositivos conectados a una red.
- Detectar puertos abiertos y servicios en ejecución.
- Determinar versiones de software y sistemas operativos.
- Realizar pruebas de seguridad y detección de vulnerabilidades.

## Justificación del porque se utilizo el repositorio de NMAP
El escaneo de redes, tanto en entornos domésticos como empresariales, permite identificar puertos abiertos, latencia en la red y posibles vulnerabilidades. Es fundamental que los profesionales de redes comprendan y actúen adecuadamente en el análisis de una red. Nmap, una de las herramientas más populares, es ampliamente utilizada en pruebas de penetración (pentesting), retos CTF y auditorías de seguridad.
El repositorio de Nmap no solo ofrece una herramienta de escaneo de puertos, sino que también proporciona un framework avanzado de auditoría de redes y seguridad ofensiva. Su versatilidad lo hace útil tanto para atacantes éticos como para defensores de ciberseguridad.

Por ejemplo, la empresa CompTIA menciona:
> "Nmap suele considerarse una herramienta de ciberseguridad, aunque también es útil para la resolución de problemas de redes." (Garn, 2024)

Asimismo, Red Hat destaca:
> "Nmap es conocido popularmente como la navaja suiza del administrador de sistemas, debido a su capacidad para identificar problemas en redes corporativas." (Nandishwar, 2019)

Nmap es una herramienta fundamental en ciberseguridad, especialmente en pruebas de penetración y análisis de redes. Su capacidad para realizar escaneos de puertos, detectar servicios y analizar sistemas operativos lo convierte en una opción robusta para mapear redes y descubrir vulnerabilidades.

## ¿Por qué usar Nmap?
Nmap es una herramienta que permite mapear rápidamente una red sin necesidad de configuraciones complejas. Puede utilizarse con comandos simples o con scripting avanzado mediante el Nmap Scripting Engine (NSE).

### Principales Características:
- **Reconocimiento de dispositivos**: Detecta rápidamente servidores, routers y dispositivos en la red.
- **Identificación de servicios**: Permite conocer qué servicios están activos y sus versiones.
- **Detección del sistema operativo**: Obtiene información detallada del sistema operativo.
- **Escaneo de seguridad y vulnerabilidades**: Utiliza scripts NSE para auditorías de seguridad.
- **Interfaz gráfica (Zenmap)**: Permite generar mapas visuales de la red.

## Aspectos Claves de Nmap
| **Aspecto**               | **Descripción** |
|---------------------------|-----------------|
| **Nombre**               | Nmap (Network Mapper) |
| **Funcionalidad Principal** | Herramienta de código abierto para el escaneo y mapeo de redes. |
| **Características destacadas** | - Detección de hosts activos.<br>- Escaneo de puertos.<br>- Detección de servicios y versiones.<br>- Estimación del sistema operativo.<br>- Nmap Scripting Engine (NSE) para tareas específicas. |
| **Aplicaciones Comunes** | - Seguridad Informática.<br>- Administración de redes.<br>- Auditorías de cumplimiento. |

### Técnicas avanzadas con Nmap:
- Identificación de sistemas operativos y versiones de software con `-O` y `-sV`.
- Uso en pruebas de penetración para obtener una visión detallada de la superficie de ataque.
- Técnicas de evasión como:
  - Fragmentación de paquetes (`-f`).
  - Modificación de TTL (`--ttl`).
  - Camuflaje de origen (`-S`, `-D`).
- Escaneo distribuido con `nmap -iL` para analizar múltiples objetivos simultáneamente.

## Ejemplo de Escaneo con Nmap
```bash
nmap -A -T4 scanme.nmap.org
```

### Reporte de escaneo:
```bash
Reporte de escaneo de Nmap para scanme.nmap.org (74.207.244.221)
El anfitrión está activo (0.029s latencia).
rDNS: li86-221.members.linode.com
No mostrado: 995 puertos cerrados
PORT     ESTADO    SERVICIO    VERSION
22/tcp   open      ssh         OpenSSH 5.3p1 Debian 3ubuntu7 (protocolo 2.0)
80/tcp   open      http        Apache httpd 2.2.14 ((Ubuntu))
...
```

## Referencias
- Garn, D. (2024). "What is Nmap?" Blog CompTIA. [CompTIA](https://www.comptia.org/blog/what-is-nmap)
- Liao, S., et al. (2020). "A Comprehensive Detection Approach of Nmap". [DOI](https://doi.org/10.1109/CyberC49757.2020.00020)
- Nandishwar, S. (2019). "Use cases of Nmap". RedHat Blog. [RedHat](https://www.redhat.com/en/blog/use-cases-nmap)
- Yashvant Mahadev, H. (2023). "A Review on Nmap and Its Features". International Research Journal of Engineering and Technology, 10(05), 1176-1180.
- Patel, R., & Singh, A. (2023). "Use Nmap like a Pro". ResearchGate. [ResearchGate](https://www.researchgate.net/publication/387953667)
- Kumar, S. (2022). "A Case Study on Nmap". Academia.edu. [Academia.edu](https://www.academia.edu/34856706)
- "Nmap: the Network Mapper - Free Security Scanner". [Nmap.org](https://nmap.org/)

