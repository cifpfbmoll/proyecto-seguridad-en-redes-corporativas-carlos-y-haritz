

[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/A04QAW6X)
Sprint 3
Aumentar la seguridad del servidor Apache.
Configurar el servidor para minimizar vulnerabilidades
Implementar medidas de protección contra ataques

1. Instalación de Apache
Actualización de paquetes del sistema
Instalación de Apache
Verificación del estado del servicio

3. Configuraciones Globales
Configuración de usuarios y grupos: Editamos los archivos apache2.conf y envvars para establecer los usuarios y grupos que ejecutan el servidor
Ocultación de versiones: Modificamos el archivo security.conf para ocultar la versión de Apache, cambiando ServerSignature a Off y añadiendo ServerTokens ProductOnly
Exposición mínima de módulos: Desactivamos módulos no utilizados

5. VirtualHost
Creación de un VirtualHost con nombre y apellido, configurando las directivas de opciones para establecer el comportamiento del servidor

7. Autenticación y Acceso
Implementación de restricciones de acceso al contenido mediante las directivas Auth y Require para autenticar el acceso a un directorio específico

9. Archivos .htaccess
Los archivos .htaccess son utilizados para controlar el comportamiento del servidor y gestionar solicitudes a recursos específicos sin modificar la configuración global

11. Configuración HTTPS
Habilitación de SSL en Apache y creación de certificados para asegurar el VirtualHost, obligando a que todas las conexiones sean a través de HTTPS

13. Módulo mod_security
mod_security es un módulo de Apache que actúa como un firewall de aplicaciones web, monitoreando y filtrando solicitudes HTTP en tiempo real para bloquear tráfico malicioso

15. Pruebas de Seguridad
Ataque DoS: Descarga de Kali Linux y realización de un ataque DoS mediante Metasploit (Slowloris) para comprobar la vulnerabilidad del servidor
Reglas OWASP: Clonación e instalación de las reglas recomendadas de OWASP y habilitación de mod_security para detectar SQL Injection

17. Re-evaluación del Ataque DoS
Realizamos nuevamente el ataque DoS y comprobamos que el servidor sigue accesible gracias a las configuraciones implementadas
