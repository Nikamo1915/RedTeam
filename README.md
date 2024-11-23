# RedTeam
Práctica Red Team
Práctica de Seguridad: Compromiso de Active Directory mediante Phishing
Descripción
Esta práctica tiene como objetivo demostrar, de manera teórica y educativa, cómo se podría comprometer la seguridad de una empresa objetivo, en este caso KAYAK.COM, mediante un ataque de phishing que lleva a la infección del sistema.

Objetivo
El objetivo final de esta práctica es comprometer el Active Directory de la empresa KAYAK.COM a través de un ataque de phishing bien diseñado y ejecutado.

Entorno de Prueba
Se han utilizado tres máquinas virtuales para la configuración del entorno de prueba:

Servidor con Active Directory (Windows Server)

Configurado como controlador de dominio.

Máquina de Objetivo (Windows)

Unida al dominio configurado.

Máquina de Ejecución de C&C (Debian)


Pasos Seguidos

1. Configuración del Entorno
Instalación de Active Directory en el Servidor Windows:

Instalación de Active Directory Domain Services.

Promoción del servidor a controlador de dominio y configuración del dominio.

Unión de la Máquina de Comando y Control al Dominio:

Configuración y verificación de la conexión al dominio.

2. Recopilación de Información
Herramientas Utilizadas:

whois, nslookup, shodan, nmap

ldapsearch y BloodHound (en un entorno simulado)

3. Diseño y Ejecución del Ataque de Phishing
Diseño del Correo de Phishing:

Creación de un correo convincente con un archivo adjunto malicioso dirigido a un empleado.

Configuración de Havoc en Debian:

Instalación y configuración para la creación del payload.

Envío del Correo de Phishing:

Envío del correo desde la máquina Debian y ejecución del malware en la máquina Windows.

4. Análisis del Acceso Obtenido
Acceso al Active Directory:

Análisis de la conexión y enumeración interna.

Identificación de posibles vectores de escalación de privilegios.

Este repositorio y la información contenida en él tienen fines educativos y de concienciación sobre seguridad. No se deben utilizar para actividades maliciosas. El autor no se responsabiliza del mal uso de esta información.
