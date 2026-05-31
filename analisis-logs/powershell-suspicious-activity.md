# Caso 4 - Actividad sospechosa mediante PowerShell

## 1. Contexto

PowerShell es una herramienta legítima de administración utilizada ampliamente en sistemas Windows.

Sin embargo, también es utilizada frecuentemente por atacantes para ejecutar comandos maliciosos sin necesidad de instalar software adicional.

---

## 2. Escenario simulado

Se detecta la ejecución de comandos PowerShell que realizan acciones inusuales dentro del sistema.

La actividad genera eventos registrados por las herramientas de monitorización.

---

## 3. Evidencias

Actividad detectada:

* Ejecución de comandos PowerShell.
* Uso de parámetros poco habituales.
* Actividad fuera del comportamiento normal del usuario.

Observaciones:

* Posible intento de evasión.
* Actividad potencialmente maliciosa.

---

## 4. Análisis

El uso de PowerShell es habitual en tareas administrativas, por lo que resulta necesario analizar el contexto de ejecución.

La presencia de comandos inusuales puede indicar intentos de descarga de contenido, ejecución remota o movimientos posteriores dentro del sistema.

---

## 5. Detección

Se debe generar una alerta cuando:

* Se ejecuten comandos PowerShell sospechosos.
* Existan conexiones externas asociadas.
* Se detecten parámetros anómalos.

---

## 6. Respuesta

1. Identificar el usuario responsable.
2. Analizar los comandos ejecutados.
3. Revisar conexiones asociadas.
4. Determinar el alcance de la actividad.
5. Aplicar medidas correctivas.

---

## 7. Explicación para estudio

PowerShell es una herramienta legítima que puede ser utilizada tanto para administración como para actividades maliciosas.

Por este motivo, resulta especialmente importante analizar el comportamiento asociado y no únicamente la ejecución del proceso.

---

## 8. Puntos clave

* PowerShell es una herramienta legítima.
* El contexto determina si la actividad es sospechosa.
* Es una técnica habitual en ataques modernos.
* Requiere monitorización específica.

---

## Flujo del ataque

[Usuario o atacante] → [PowerShell] → [Actividad sospechosa] → [Detección] → [Análisis] → [Respuesta]
