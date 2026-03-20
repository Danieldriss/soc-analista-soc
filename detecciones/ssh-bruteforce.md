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



\## Escenario de detección

Basado en el análisis previo, se define una detección para identificar intentos de acceso no autorizados mediante fuerza bruta.



\## Ejemplo de evento

Evento de autenticación fallida repetido múltiples veces desde la misma IP.



\## Razonamiento

Una alta frecuencia de eventos de tipo "Failed password" es un indicador claro de intento de acceso automatizado.

