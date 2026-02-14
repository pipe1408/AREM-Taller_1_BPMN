# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
Taller 1 - BPMN

## 👥 Integrantes del equipo
- Felipe Ballesteros
- Andres Beltran
- Tomas Ariza

## 🧠 Descripción general del trabajo
El presente trabajo tuvo como objetivo modelar un proceso de negocio real utilizando la notación BPMN (Business Process Model and Notation), tomando como cliente la aplicación BO-TECH TRACKING, una solución tecnológica enfocada en el rastreo y monitoreo en tiempo real de transporte escolar.

La aplicación permite a padres de familia y coordinadores hacer seguimiento a rutas escolares mediante geolocalización, recibir notificaciones automáticas y garantizar mayor seguridad en el traslado de estudiantes.

El proceso seleccionado para modelar fue el proceso de monitoreo y notificación de ruta escolar en tiempo real, desde que el vehículo inicia su recorrido hasta que el estudiante llega a su destino.


## 2. Proceso de desarrollo

Para la elaboración del modelo BPMN se siguieron los siguientes pasos:

### 2.1 Identificación del alcance del proceso

Se definió que el proceso iniciaría cuando el conductor activa la ruta en el sistema y finalizaría cuando el estudiante llega a su destino y se envía la notificación correspondiente al acudiente.

### 2.2 Identificación de actores y roles

Se identificaron los siguientes participantes:

- Conductor
- Sistema BO-TECH TRACKING
- Padre o acudiente
- Plataforma de notificaciones
- Base de datos

### 2.3 Definición de actividades principales

Se modelaron las siguientes actividades:

- Activación de la ruta por parte del conductor.
- Captura de ubicación GPS en tiempo real.
- Actualización de datos en el sistema.
- Visualización del recorrido por parte del acudiente.
- Generación y envío de notificaciones automáticas.
- Confirmación de llegada del estudiante.

### 2.4 Modelado de decisiones (Gateways)

Se incluyeron compuertas exclusivas para validar:

- ¿El GPS está activo y funcionando correctamente?
- ¿El estudiante abordó el vehículo?
- ¿El vehículo llegó al destino?
- ¿Se debe enviar notificación automática?

Estas decisiones permiten modelar escenarios alternativos como fallos de señal o retrasos en la ruta.

### 2.5 Ajustes y refinamiento del modelo

Durante el modelado se ajustó el flujo para diferenciar claramente tareas manuales (realizadas por conductor o acudiente) y tareas automáticas (ejecutadas por el sistema). Además, se incorporaron eventos intermedios de mensaje para representar el envío de notificaciones en tiempo real.


## 3. Análisis del modelo propuesto

### 3.1 Cómo se estructura el modelo entregado

El modelo se estructuró con un pool principal correspondiente a BO-TECH TRACKING, dividido en lanes que representan los distintos actores del proceso:

- Conductor
- Sistema
- Padre o acudiente

El flujo inicia con un evento de inicio cuando el conductor activa la ruta. Posteriormente, el sistema comienza a registrar la ubicación en tiempo real, generando actualizaciones continuas. Cuando el estudiante aborda el vehículo, el sistema envía una notificación automática al acudiente.

Finalmente, al llegar al destino, se genera una notificación de llegada y el proceso concluye con un evento de fin.

El modelo incluye:

- Evento de inicio
- Tareas manuales y automáticas
- Gateways exclusivos
- Eventos intermedios de mensaje
- Evento de fin

### 3.2 Cómo representa las necesidades del cliente

El modelo representa adecuadamente las necesidades principales de la aplicación:

- Seguridad en el transporte escolar.
- Información en tiempo real.
- Notificaciones automáticas.
- Control y trazabilidad del recorrido.
- Reducción de incertidumbre para los padres.

Además, permite identificar puntos críticos como:

- Fallas en el GPS.
- Problemas de conectividad.
- Retrasos en la ruta.
- Errores en el envío de notificaciones.

Esto facilita el análisis para mejoras futuras del sistema.

### 3.3 Supuestos tomados

Para el modelado del proceso se asumió que:

- El conductor cuenta con conexión a internet.
- El GPS del dispositivo funciona correctamente.
- El acudiente tiene instalada la aplicación.
- Las notificaciones push funcionan sin retrasos.
- La base de datos registra la información en tiempo real.

Estos supuestos permitieron delimitar el alcance del modelo y evitar complejidad excesiva.

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
