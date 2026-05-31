# Proyecto SOC - Casos prácticos de análisis, detección y respuesta

## Descripción

Este repositorio recopila distintos casos prácticos orientados al análisis de eventos de seguridad en un entorno SOC (Security Operations Center).

El objetivo del proyecto es documentar escenarios habituales de ciberseguridad desde la perspectiva de un analista Blue Team, incluyendo el análisis de los eventos, los mecanismos de detección y las posibles acciones de respuesta.

Además de servir como portfolio técnico, el repositorio está diseñado como material de estudio para reforzar conocimientos relacionados con monitorización, detección de amenazas y respuesta ante incidentes.

---

## Metodología

Todos los casos siguen una estructura común:

1. Contexto
2. Escenario simulado
3. Evidencias
4. Análisis
5. Detección
6. Respuesta
7. Explicación para estudio
8. Puntos clave

Esta metodología permite mantener la consistencia entre los distintos casos y facilitar su consulta posterior.

---

## Casos desarrollados

| Caso                  | Descripción                                              |
| --------------------- | -------------------------------------------------------- |
| SSH Brute Force       | Intentos repetidos de acceso mediante autenticación SSH  |
| Phishing              | Robo de credenciales mediante ingeniería social          |
| Malware Execution     | Ejecución de software malicioso en un sistema            |
| Suspicious PowerShell | Uso sospechoso de PowerShell para actividades maliciosas |
| C2 Connection         | Comunicación con servidores de comando y control         |
| Nmap Reconnaissance   | Actividades de reconocimiento y escaneo de red           |
| Ransomware            | Análisis general de amenazas de tipo ransomware          |

---

## Estructura del proyecto

```text
analisis-logs/
inteligencia-amenazas/
notas-diarias/
```

* **analisis-logs/** → Casos prácticos principales del proyecto.
* **inteligencia-amenazas/** → Información complementaria sobre amenazas relevantes.
* **notas-diarias/** → Registro del progreso y evolución del aprendizaje.

---

## Relación con el Homelab

Este proyecto complementa el laboratorio de seguridad desarrollado en:

https://github.com/Danieldriss/homelab-network-security

Mientras que el Homelab se centra en la infraestructura, la generación de eventos y las evidencias prácticas, este repositorio documenta el análisis técnico, la detección y la respuesta asociada a cada caso.

---

## Estado del proyecto

El proyecto se encuentra finalizado a nivel documental.

En futuras fases se añadirán evidencias prácticas obtenidas directamente del laboratorio para complementar los casos ya desarrollados.

---

## Objetivo final

Desarrollar una base de conocimiento reutilizable orientada a análisis SOC, Blue Team y detección de amenazas, combinando teoría, práctica y documentación técnica.
