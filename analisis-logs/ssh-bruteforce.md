\# Análisis de logs - Ataque SSH Brute Force



\## Objetivo

Identificar actividad sospechosa en logs de autenticación SSH.



\## Escenario

Se observa un volumen elevado de intentos fallidos de login en un servidor.



\## Observaciones

\- Múltiples intentos fallidos de autenticación

\- Repetición desde una misma IP

\- Intervalos de tiempo muy cortos entre intentos



\## Indicadores detectados

\- Evento: "Failed password"

\- Alta frecuencia de eventos

\- Origen repetido



\## Análisis

El patrón observado corresponde a un ataque de fuerza bruta contra el servicio SSH.



\## Impacto potencial

\- Acceso no autorizado si se compromete una cuenta

\- Movimiento lateral

\- Escalada de privilegios



\## Conclusión

Se trata de un intento de intrusión mediante fuerza bruta.



\## Lecciones aprendidas

\- Los logs de autenticación son clave

\- La repetición es un indicador crítico

