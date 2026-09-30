# Tarea: Mi prompt avanzado

## Tarea elegida

Diseñar y generar las clases en Java para un módulo de gestión de notas estudiantiles con cálculo de promedios y estado de aprobación.

## Version 1: prompt basico

Crea un programa en Java para registrar notas de estudiantes y calcular si aprobaron.

## Version 2

Actua como desarrollador Java Senior.
Diseña un sistema de notas estudiantiles. Muestra el razonamiento paso a paso de las clases requeridas y luego escribe el codigo.

## Version 3: prompt final

Actua como un Arquitecto de Software Java Senior experto en diseño orientado a objetos.
Sistema academico para registrar notas de alumnos (entre 0 y 20). Se requiere calcular el promedio ponderado y determinar si el alumno esta Aprobado (>= 13) o Desaprobado.

1. Diseña la estructura de clases necesarias.
2. Genera el codigo Java limpio de la clase Estudiante aplicando buenas practicas.

// Formato de salida esperado para el calculo:
"Nota final: 14.5 -> Estado: Aprobado"
"Nota final: 10.2 -> Estado: Desaprobado"

Entrega primero la explicacion del diseño y luego el codigo Java dentro de un bloque markdown.

Luego de generar la respuesta, revisa tu propio codigo: ¿Validaste que las notas esten en el rango de 0 a 20? Si no es asi, corrige el codigo agregando la validacion en el constructor.

## Tecnicas usadas en el prompt final

| Técnica             | Parte del prompt final donde se aplica                                         |
| ------------------- | ------------------------------------------------------------------------------ |
| Role Prompting      | `Actua como un Arquitecto de Software Java Senior...`                          |
| Prompt Estructurado | Uso de etiquetas XML (`, `, `, `, ``)                                          |
| Few-Shot            | Sección `` mostrando el formato exacto del mensaje de salida                   |
| Autocrítica         | Instrucción final: `Luego de generar la respuesta, revisa tu propio codigo...` |

## Evaluacion del resultado

| Criterio                                                       | Cumple (Sí / No) |
| -------------------------------------------------------------- | ---------------- |
| ¿Aplica principios de Programación Orientada a Objetos?        | Sí               |
| ¿Valida correctamente que las notas estén entre 0 y 20?        | Sí               |
| ¿Respeta el formato de respuesta especificado en los ejemplos? | Sí               |
| ¿Incluye autocrítica y corrige deficiencias de código?         | Sí               |

## Por que elegi estas tecnicas

Elegí **Role Prompting** para forzar un nivel técnico profesional en el código generado (POO y buenas prácticas); **Prompt Estructurado** para separar con claridad las reglas del negocio de los requerimientos técnicos; **Few-Shot** para garantizar que las salidas de estado tengan el formato exacto necesario; y **Autocrítica** porque el control de límites (como notas menores a 0 o mayores a 20) suele omitirse en la primera generación de código de un LLM.

- [Tarea: mi prompt avanzado](prompts/TAREA.md)
