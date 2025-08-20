# Curso-NGINX
Video de youtube: https://www.youtube.com/watch?v=UFSaK7Pv-aA&t=51s

### **Temario NGINX desde cero**

#### **Módulo 1: Introducción a NGINX**✅
1. **¿Qué es NGINX?**✅
   - Historia y propósito de NGINX.✅
   - Diferencias entre NGINX y otros servidores web (Apache, IIS).✅
   - Casos de uso: servidor web, proxy inverso, balanceador de carga, caché.✅
2. **Arquitectura de NGINX**✅
   - Modelo basado en eventos (event-driven).✅
   - Procesos maestros y trabajadores (master and worker processes).✅
   - Comparación con el modelo de hilos de Apache.✅
3. **Instalación de NGINX**✅
   - Instalación en sistemas operativos:✅
     - Linux (Ubuntu, CentOS, Debian).✅
     https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware+Workstation+Pro&freeDownloads=true
     - Windows.✅
     - macOS.✅
   - Instalación desde repositorios, compilación desde el código fuente.✅
   - Verificación de la instalación (`nginx -v`).✅

#### **Módulo 2: Configuración básica**✅
1. **Estructura de los archivos de configuración**✅
   - Archivo principal: `nginx.conf`.✅
   - Directorios: `/etc/nginx/`, `sites-available`, `sites-enabled`.✅
   - Sintaxis básica: directivas, bloques (`http`, `server`, `location`).✅

2. **Comandos básicos de NGINX**
   - Iniciar, detener y reiniciar NGINX (`systemctl`, `nginx -s`).✅
   - Validar la configuración (`nginx -t`).✅
   - Recargar configuración sin tiempo de inactividad.✅

3. **Configuración de un servidor web básico**✅
   - Servir archivos estáticos (HTML, CSS, JS).✅
   - Configurar el puerto y la dirección IP (`listen`).✅
   - Definir la raíz de los documentos (`root`).✅
   
4. **Logs en NGINX**✅
   - Configuración de logs de acceso (`access_log`) y errores (`error_log`).✅
   - Formatos de log personalizados.✅
   - Análisis básico de logs.✅

#### **Módulo 3: Configuración avanzada de servidores**
1. **Manejo de rutas y ubicaciones**✅
   - Bloques `location`: exactos, prefijos, expresiones regulares.✅
   - Prioridad de las reglas de coincidencia.✅
   - Reescrituras y redirecciones (`rewrite`, `return`). ✅

2. **Configuración de dominios virtuales**✅
   - Servidores virtuales basados en nombre (`server_name`).✅
   - Manejo de múltiples dominios en una sola instancia de NGINX.✅

3. **Manejo de errores**✅
   - Páginas de error personalizadas (`error_page`).✅
   - Redirecciones para errores 404, 500, etc.✅

4. **Compresión y optimización**✅
   - Habilitar compresión Gzip (`gzip`). ✅
   - Configuración de caché de navegador (`expires`).✅

#### **Módulo 4: NGINX como proxy inverso**✅
1. **¿Qué es un proxy inverso?**✅
   - Diferencias entre proxy directo y proxy inverso.✅
   - Casos de uso comunes.✅

2. **Configuración de un proxy inverso**✅
   - Directiva `proxy_pass`.✅
   - Configuración de cabeceras (`proxy_set_header`).✅
   - Manejo de conexiones persistentes.✅

3. **Proxy para aplicaciones dinámicas**
   - Configuración para servidores de aplicaciones (Node.js, PHP-FPM, Python, Ruby).✅
   - Configuración de FastCGI para PHP.✅
   - Integración con servidores como Gunicorn o uWSGI.✅

#### **Módulo 5: Balanceo de carga**
1. **Conceptos de balanceo de carga**✅
   - Beneficios y casos de uso.✅
   - Algoritmos de balanceo: round-robin, least connections, IP hash.✅

2. **Configuración de balanceo de carga**✅
   - Bloque `upstream`.✅
   - Configuración de servidores backend.✅
   - Monitoreo de salud de los servidores (`health checks`).✅

3. **Sesiones persistentes**✅
   - Configuración de sticky sessions (`ip_hash`, módulos de terceros).✅
