# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller 1 - BPMN

## 👥 Integrantes del equipo
- Felipe Ballesteros
- Andres Beltran
- Tomas Ariza

## 🧠 Descripción general del trabajo
El objetivo del presente taller fue modelar un proceso de negocio real utilizando la notación BPMN (Business Process Model and Notation), identificando sus eventos, actividades, decisiones, actores involucrados y puntos críticos del flujo.

Durante la actividad en clase se trabajó con el caso base de la Clínica Salud Viva, específicamente el proceso de agendamiento de citas médicas. El ejercicio permitió comprender la estructura formal de un modelo BPMN y su utilidad para representar procesos organizacionales de manera clara, estandarizada y comprensible para diferentes actores.

El desarrollo del taller se realizó de manera colaborativa, estructurando primero el flujo lógico del proceso y posteriormente representándolo mediante diagramación formal en una herramienta de modelado.

## 🔧 Proceso de desarrollo
Para la elaboración del modelo BPMN se siguieron los siguientes pasos metodológicos:

### 2.1 Identificación del alcance del proceso
Se definió que el proceso iniciaría cuando el paciente requiere agendar una cita médica y finalizaría cuando la cita queda confirmada y el paciente recibe notificación.

### 2.2 Identificación de actores y roles
Se determinaron los siguientes participantes:

- Paciente  
- Sistema de gestión de citas  
- Base de datos  
- Servicio de notificaciones  

### 2.3 Definición de actividades principales
Se modelaron las tareas realizadas por el paciente (selección de especialidad, médico y fecha) y las tareas automáticas del sistema (verificación de disponibilidad, registro en base de datos y envío de notificación).

### 2.4 Modelado de decisiones (Gateways)
Se incluyeron compuertas exclusivas para validar:

- Disponibilidad de médicos  
- Disponibilidad de la fecha seleccionada  

### 2.5 Ajustes y refinamiento del modelo
Inicialmente se planteó un flujo lineal; posteriormente se incorporaron decisiones y eventos alternativos (por ejemplo, cuando no hay disponibilidad), mejorando la precisión del modelo.

La herramienta utilizada para la diagramación fue draw.io (diagrams.net), permitiendo aplicar correctamente los elementos estándar de BPMN 2.0.

## 🧩 Análisis del modelo propuesto
### 3.1 Cómo se estructura el modelo entregado

El modelo se encuentra estructurado mediante un pool principal correspondiente a la Clínica Salud Viva, dividido en lanes que representan los roles del proceso.  

El flujo inicia con un evento de inicio simple, continúa con tareas de usuario y tareas automáticas del sistema, incluye gateways exclusivos para la toma de decisiones y finaliza con un evento de fin que representa la confirmación de la cita.

La estructura respeta los principios básicos de BPMN:

- Un evento de inicio claro  
- Secuencia lógica de tareas  
- Decisiones explícitas  
- Evento de fin definido  

### 3.2 Cómo representa las necesidades del cliente

El modelo refleja adecuadamente el proceso real de agendamiento digital, incluyendo:

- Interacción entre usuario y sistema  
- Validación de disponibilidad en tiempo real  
- Registro persistente en base de datos  
- Notificación automática al paciente  

Además, permite identificar posibles cuellos de botella, como la falta de disponibilidad médica o fallos en la confirmación de la cita.

De esta manera, el modelo no solo representa el flujo actual, sino que también sirve como herramienta para análisis y mejora del proceso.

### 3.3 Supuestos tomados

Para la elaboración del modelo se asumió que:

- El paciente ya se encuentra registrado en el sistema.  
- La plataforma funciona correctamente y no presenta fallas técnicas.  
- La disponibilidad médica se encuentra actualizada en tiempo real.  
- El envío de notificaciones se realiza de manera automática.  
- No se contemplan cancelaciones o reprogramaciones en este modelo base.  

Estos supuestos permitieron delimitar el alcance del proceso y evitar una complejidad excesiva en esta primera aproximación.


## 📈 Diagrama final entregado
> (Inserte aquí una imagen o enlace al modelo-final.drawio / .asta / PDF)

## 📋 Tabla de actores, entidades o componentes (si aplica)

| Nombre del elemento | Tipo | Descripción | Responsable |
|---------------------|------|-------------|-------------|
| Ej: Paciente        | Actor | Usuario que agenda una cita médica | Cliente |

## 🔍 Investigación complementaria
### Tema investigado:
(Ej: Buenas prácticas BPMN, comparación TOGAF vs C4, principios de seguridad STRIDE, etc.)

### Resumen:
Describa en 2–3 párrafos lo investigado, citando fuentes cuando sea necesario. Incluya cómo se relaciona con el taller.

## 📚 Referencias
- [1] Apellido, Nombre. *Título*. Año. URL o DOI.
- [2] Fuente oficial BPMN: https://www.omg.org/spec/BPMN/

---

_Este documento hace parte de la entrega del taller X del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
