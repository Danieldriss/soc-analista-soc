# Caso 5 - Conexión a servidor C2 (Command and Control)

## 1. Contexto

Los servidores de Comando y Control (C2) son utilizados por los atacantes para mantener comunicación con sistemas previamente comprometidos.

A través de estos canales pueden enviar instrucciones, descargar nuevas cargas maliciosas o extraer información del sistema afectado.

---

## 2. Escenario simulado

Se detectan conexiones periódicas desde un equipo interno hacia una dirección IP externa desconocida.

El comportamiento no corresponde con ninguna comunicación habitual del entorno.

---

## 3. Evidencias

Actividad detectada:

* Conexiones repetidas hacia una IP externa.
* Comunicación periódica.
* Tráfico no asociado a servicios legítimos conocidos.

Observaciones:

* Comportamiento persistente.
* Posible compromiso previo del sistema.

---

## 4. Análisis

Las comunicaciones periódicas hacia destinos externos desconocidos constituyen uno de los indicadores más habituales de actividad C2.

Este comportamiento puede indicar la presencia de malware que intenta mantener comunicación con la infraestructura controlada por el atacante.

---

## 5. Detección

Se debe generar una alerta cuando:

* Existan conexiones repetitivas a destinos desconocidos.
* Se detecten patrones de comunicación periódica.
* Aparezcan conexiones externas no habituales.

---

## 6. Respuesta

1. Identificar el sistema afectado.
2. Analizar las conexiones de red.
3. Bloquear la comunicación sospechosa.
4. Revisar posibles indicadores de compromiso.
5. Realizar análisis forense si es necesario.

---

## 7. Explicación para estudio

Los canales C2 permiten a los atacantes mantener el control de sistemas comprometidos de forma remota.

La detección temprana de este tipo de comunicaciones puede evitar fases posteriores del ataque y reducir significativamente su impacto.

---

## 8. Puntos clave

* Las conexiones periódicas son un indicador relevante.
* El tráfico externo debe monitorizarse continuamente.
* Los servidores C2 son habituales en campañas de malware.
* La detección temprana mejora la capacidad de respuesta.

---

## Flujo del ataque

[Compromiso inicial] → [Comunicación C2] → [Control remoto] → [Detección] → [Respuesta]
