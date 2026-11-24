# Escáner de Archivos y Credenciales Expuestas

[![Escaneo Archivos Expuestos](https://img.shields.io/badge/TAVARDT-Superficie%20de%20Ataque-5b3cf5.svg)](https://tools.tavardt.com/es/escaneo-archivos-expuestos/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Escáner de superficie de ataque para detección automatizada de archivos de entorno, copias de seguridad, repositorios git y credenciales expuestas.

Desarrollado y mantenido por la division de ciberseguridad ofensiva de **TAVARDT**.

***

## Alcance de Deteccion de Superficie

* **Variables de Entorno y Secretos**: Inspeccion de archivos `.env`, `.env.local` y `.env.production`.
* **Metadatos de Versionado**: Verificacion de rutas de repositorios en `/.git/HEAD` y `/.git/config`.
* **Respaldos de Bases de Datos**: Deteccion de volcados SQL como `backup.sql`, `dump.sql` y `database.sql`.
* **Configuraciones de Servidor**: Comprobacion de `docker-compose.yml` y exposicion de datos en `phpinfo.php`.
* **Alineacion Normativa**: Estructurado de acuerdo con el Guias de Seguridad CCN-STIC del CCN-CERT y Esquema Nacional de Seguridad (ENS).

***

## Instalacion y Ejecucion

Requiere unicamente Python 3.8 o superior sin dependencias externas.

```bash
git clone https://github.com/TAVARDT-Espana/exposed-files-scanner-es.git
cd exposed-files-scanner-es
python scanner.py empresa.es
```

Para generar la salida en formato JSON:

```bash
python scanner.py empresa.es -json
```

***

## Diagnostico Completo en la Web

Para escaneos corporativos continuos con interfaz grafica, acceda a la herramienta oficial:

* **Escaneo de Archivos Expuestos**
* **[Portal Corporativo TAVARDT](https://ag.tavardt.com/es/)**

***

## Consultoria en Seguridad Ofensiva

Para pruebas de penetracion y gestion de superficie de ataque en Espana, consulte a los especialistas de **TAVARDT**.

***

© 2026 TAVARDT. Todos los derechos reservados.
