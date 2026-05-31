# Caso 7 - Ransomware

## 1. Contexto

El ransomware es uno de los tipos de malware más utilizados por los ciberdelincuentes en la actualidad.

Su objetivo principal es cifrar la información de los sistemas afectados para impedir el acceso a los datos y exigir posteriormente un pago económico a cambio de su recuperación.

Este tipo de amenaza puede afectar tanto a usuarios particulares como a organizaciones, provocando importantes pérdidas operativas y económicas.

---

## 2. Escenario simulado

Un usuario recibe un correo electrónico malicioso que contiene un archivo adjunto infectado.

Tras ejecutar el archivo, el sistema comienza a cifrar información y genera actividad sospechosa detectada por las herramientas de monitorización.

---

## 3. Evidencias

Actividad detectada:

* Aparición de archivos cifrados.
* Procesos inusuales ejecutándose en el sistema.
* Incremento de actividad sobre archivos y directorios.
* Conexiones externas sospechosas.

Observaciones:

* Pérdida de acceso a la información.
* Posible compromiso de otros sistemas conectados.

---

## 4. Análisis

El ransomware suele utilizar diferentes vectores de entrada para comprometer los sistemas.

Entre los más habituales se encuentran:

* Campañas de phishing.
* Contraseñas débiles.
* Servicios expuestos a Internet.
* Vulnerabilidades sin parchear.

Una vez ejecutado, el malware intenta cifrar la información disponible y dificultar la recuperación de los datos.

---

## 5. Detección

Se debe generar una alerta cuando:

* Aparezcan procesos relacionados con cifrado masivo de archivos.
* Se detecten accesos anómalos a múltiples directorios.
* Existan conexiones externas sospechosas.
* Se produzcan modificaciones masivas de archivos en un corto periodo de tiempo.

---

## 6. Respuesta

1. Aislar el sistema afectado.
2. Identificar el alcance del incidente.
3. Revisar indicadores de compromiso.
4. Restaurar información desde copias de seguridad.
5. Analizar el origen de la infección.
6. Aplicar medidas correctivas para evitar nuevas infecciones.

---

## 7. Explicación para estudio

El ransomware es una de las amenazas más relevantes dentro de la ciberseguridad actual debido a su impacto operativo y económico.

La prevención, la monitorización continua y la existencia de copias de seguridad actualizadas son elementos fundamentales para minimizar los daños provocados por este tipo de ataques.

---

## 8. Puntos clave

* El phishing es uno de los principales vectores de entrada.
* Las copias de seguridad son esenciales.
* La detección temprana reduce el impacto.
* La segmentación y monitorización mejoran la capacidad defensiva.

---

## Flujo del ataque

[Phishing o vulnerabilidad] → [Infección] → [Cifrado de archivos] → [Detección] → [Respuesta] → [Recuperación]
