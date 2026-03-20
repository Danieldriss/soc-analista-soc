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



\## Escenario simulado

Se ha simulado un servidor Linux con servicio SSH expuesto a red, donde un atacante intenta acceder mediante múltiples intentos de autenticación.



\## Evidencias (logs simulados)

Mar 23 10:15:01 server sshd\[1234]: Failed password for root from 192.168.1.50

Mar 23 10:15:03 server sshd\[1234]: Failed password for root from 192.168.1.50

Mar 23 10:15:05 server sshd\[1234]: Failed password for admin from 192.168.1.50



\## Interpretación personal

Los intentos repetidos desde la misma IP en intervalos muy cortos indican un comportamiento automatizado típico de ataques de fuerza bruta.



\## Decisión

Se considera necesario generar una alerta cuando se detecten múltiples intentos fallidos desde una misma IP en un corto periodo de tiempo.



\## Flujo del ataque



\[Atacante] → \[Servidor SSH] → \[Logs] → \[Detección] → \[Respuesta]

