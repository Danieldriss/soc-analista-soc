# Caso 6 - Reconocimiento con Nmap

## 1. Contexto

El reconocimiento es una de las primeras fases de un ataque. Herramientas como Nmap permiten identificar puertos abiertos, servicios activos y posibles vectores de entrada en un sistema.

---

## 2. Escenario simulado

Se detectan múltiples conexiones desde una misma dirección IP hacia diferentes puertos de un servidor dentro del laboratorio.

---

## 3. Evidencias

Actividad detectada:

* IP origen: 192.168.1.60
* Puertos escaneados:

  * 22
  * 80
  * 443
  * 8080

Observaciones:

* Conexiones realizadas en un corto intervalo de tiempo.
* Acceso secuencial a múltiples servicios.

---

## 4. Análisis

El comportamiento observado es consistente con una actividad de reconocimiento automatizada.

Los atacantes utilizan herramientas como Nmap para descubrir servicios expuestos antes de intentar explotar vulnerabilidades.

---

## 5. Detección

Se debe generar una alerta cuando:

* Una misma IP acceda a múltiples puertos en poco tiempo.
* Se detecten patrones de escaneo secuencial.
* Existan intentos de enumeración de servicios.

---

## 6. Respuesta

1. Identificar la IP origen.
2. Revisar los servicios expuestos.
3. Aplicar medidas de hardening.
4. Bloquear la IP si procede.
5. Revisar posibles actividades posteriores.

---

## 7. Explicación para estudio

El reconocimiento es una fase previa al ataque cuyo objetivo es recopilar información sobre los sistemas objetivo.

Detectar esta actividad de forma temprana permite anticiparse a intentos de explotación posteriores.

---

## 8. Puntos clave

* Es una fase inicial del ataque.
* Permite descubrir servicios expuestos.
* Puede detectarse mediante análisis de tráfico y correlación de eventos.
* La detección temprana mejora la capacidad defensiva.

---

## Flujo del ataque

[Atacante] → [Escaneo Nmap] → [Identificación de servicios] → [Detección] → [Respuesta]
