\# Playbook - Respuesta a SSH Brute Force



\## Escenario

Se detectan múltiples intentos fallidos de login SSH desde una misma IP.



\## Triage

1\. Validar la alerta

2\. Identificar IP origen

3\. Revisar número de intentos

4\. Confirmar si hay accesos exitosos



\## Investigación

1\. Buscar actividad posterior

2\. Verificar si hay más sistemas afectados

3\. Analizar comportamiento de la IP



\## Contención

1\. Bloquear IP

2\. Revisar configuración SSH

3\. Aplicar medidas adicionales (MFA, claves)



\## Erradicación

1\. Revisar cuentas afectadas

2\. Cambiar credenciales si es necesario



\## Recuperación

1\. Restaurar acceso seguro

2\. Monitorizar actividad



\## Lecciones aprendidas

\- Necesidad de monitorización continua

\- Importancia de hardening



\## Contexto del incidente

La detección se activa tras identificar múltiples intentos fallidos de autenticación SSH desde una misma IP.



\## Decisión operativa

Se prioriza el bloqueo de la IP y la revisión de accesos para evitar compromiso del sistema.

