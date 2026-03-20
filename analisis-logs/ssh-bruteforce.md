\# Caso 1 - Ataque de fuerza bruta SSH



\## 1. Contexto

El servicio SSH permite el acceso remoto a sistemas Linux mediante autenticación de usuario y contraseña o claves.



Es un servicio crítico y uno de los principales objetivos de ataques automatizados en entornos reales.



\---



\## 2. Escenario simulado

Se ha simulado un servidor Linux con el puerto SSH expuesto.



Un atacante externo intenta acceder al sistema realizando múltiples intentos de autenticación desde la misma IP.



\---



\## 3. Evidencias (logs simulados)



Mar 23 10:15:01 server sshd\[1234]: Failed password for root from 192.168.1.50  

Mar 23 10:15:03 server sshd\[1234]: Failed password for root from 192.168.1.50  

Mar 23 10:15:05 server sshd\[1234]: Failed password for admin from 192.168.1.50  



\---



\## 4. Análisis

Se observa una alta frecuencia de intentos fallidos de autenticación.



Todos los intentos provienen de la misma IP y se realizan en intervalos muy cortos.



Este comportamiento no corresponde a un usuario legítimo, sino a un proceso automatizado.



Se identifica como un ataque de fuerza bruta.



\---



\## 5. Detección

Se debe generar una alerta cuando:



\- Se detecten múltiples intentos fallidos de login

\- Desde una misma IP

\- En un corto periodo de tiempo



Evento clave:

\- "Failed password"



\---



\## 6. Respuesta



Acciones recomendadas:



1\. Validar la alerta

2\. Identificar la IP atacante

3\. Revisar si ha habido accesos exitosos

4\. Bloquear la IP

5\. Revisar configuración SSH

6\. Aplicar medidas de seguridad (MFA, claves SSH)



\---



\## 7. Explicación para estudio

Un ataque de fuerza bruta consiste en probar muchas combinaciones de contraseñas hasta encontrar una válida.



En los logs se identifica por:



\- repetición de intentos fallidos

\- misma IP

\- intervalos cortos



Esto indica automatización.



Es uno de los ataques más comunes contra servicios expuestos.



\---



\## 8. Puntos clave



\- SSH es un servicio crítico y muy atacado

\- La repetición es el principal indicador

\- La detección se basa en frecuencia + origen

\- La respuesta debe ser rápida para evitar compromiso



\---



\## Flujo del ataque



\[Atacante] → \[Servidor SSH] → \[Logs] → \[Detección] → \[Respuesta]

