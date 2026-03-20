\# Detección - SSH Brute Force



\## Objetivo

Detectar intentos de fuerza bruta en servicios SSH.



\## Fuente de datos

\- Logs de autenticación Linux

\- Servicio SSH



\## Lógica de detección

Generar alerta cuando:

\- Se detecten más de 10 intentos fallidos

\- Desde la misma IP

\- En un corto periodo de tiempo



\## Condiciones

\- Evento: Failed password

\- Repetición de origen

\- Alta frecuencia



\## Posibles falsos positivos

\- Usuario introduciendo mal la contraseña

\- Scripts automatizados legítimos



\## Severidad

Media-Alta



\## Acción recomendada

Escalar a análisis manual

