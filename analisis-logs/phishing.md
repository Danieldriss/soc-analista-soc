\# Caso 2 - Ataque de phishing



\## 1. Contexto

El phishing es una técnica de ingeniería social utilizada para engañar a los usuarios y robar credenciales o información sensible.



Es uno de los ataques más comunes en entornos corporativos.



\---



\## 2. Escenario simulado

Un usuario recibe un correo electrónico aparentemente legítimo solicitando que acceda a un enlace para verificar su cuenta.



El usuario hace clic en el enlace e introduce sus credenciales en una página falsa.



\---



\## 3. Evidencias (simuladas)



Correo recibido:

\- Remitente: soporte@empresa-segura.com

\- Asunto: "Verificación urgente de cuenta"

\- Enlace: http://empresa-verificacion-login.com



Actividad detectada:

\- Login desde ubicación inusual

\- Acceso desde IP desconocida



\---



\## 4. Análisis

El correo presenta características típicas de phishing:



\- Urgencia en el mensaje

\- Dominio sospechoso

\- Enlace externo



El acceso posterior desde una IP desconocida sugiere que las credenciales han sido comprometidas.



\---



\## 5. Detección

Se debe generar alerta cuando:



\- Se detecten accesos desde ubicaciones inusuales

\- Cambios en el comportamiento de login

\- Uso de credenciales tras un evento sospechoso



Indicadores clave:

\- Dominio sospechoso

\- Login anómalo



\---



\## 6. Respuesta



Acciones recomendadas:



1\. Bloquear la cuenta afectada

2\. Forzar cambio de contraseña

3\. Revisar actividad reciente

4\. Notificar al usuario

5\. Analizar el correo recibido

6\. Bloquear el dominio malicioso



\---



\## 7. Explicación para estudio

El phishing se basa en engañar al usuario para que revele sus credenciales.



Se identifica por:



\- mensajes urgentes

\- enlaces falsos

\- dominios parecidos al real



Es importante combinar análisis técnico con comportamiento del usuario.



\---



\## 8. Puntos clave



\- El usuario es el objetivo principal

\- El correo es el vector de ataque

\- El login anómalo es la señal crítica

\- La respuesta debe ser rápida



\---



\## Flujo del ataque



\[Correo phishing] → \[Usuario] → \[Robo de credenciales] → \[Login sospechoso] → \[Detección] → \[Respuesta]

