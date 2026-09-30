# lab07-tecnicas

Bitacora de tecnicas avanzadas de prompting

# Bitacora de tecnicas avanzadas

Laboratorio 07: Tecnicas Avanzadas de Prompting.
Herramienta de IA usada: (gemini)

## Ejercicio 2: Zero-shot, one-shot y few-shot

| Tipo      | Aciertos (de 5) | Formato de la respuesta                                | Todas con el mismo formato (Si/No) |
| --------- | --------------- | ------------------------------------------------------ | ---------------------------------- |
| Zero-shot | 5               | Párrafo con lista numerada y explicaciones adicionales | No                                 |
| One-shot  | 5               | Lista numerada con comillas y etiquetas                | No                                 |
| Few-shot  | 5               | Línea por línea estricta: `"Texto" -> Etiqueta`        | Sí                                 |

## Ejercicio 3: Chain of Thought

| Pedido      | Respuesta de la IA                                                                                    | Muestra los pasos (Si/No) | Correcta (Si/No) |
| ----------- | ----------------------------------------------------------------------------------------------------- | ------------------------- | ---------------- | --- |
| Directo     | 318.60                                                                                                | No                        | Sí               |
| Paso a paso | Muestra: 1) \(120 \times 0.75 = 90\), 2) \(90 \times 1.18 = 106.20\), 3) \(106.20 \times 3 = 318.60\) | Sí                        | Sí               | }   |

## Ejercicio 4: Role prompting

| Version        | Vocabulario (sencillo/tecnico) | Usa ejemplos o codigo                            | A quien le sirve mas                   |
| -------------- | ------------------------------ | ------------------------------------------------ | -------------------------------------- |
| A. Sin rol     | Técnico intermedio             | No usa código, da definición estándar            | Estudiantes generales de computación   |
| B. Rol docente | Sencillo y cotidiano           | Usa la metáfora de una caja con etiqueta         | Principiantes sin experiencia técnica  |
| C. Rol senior  | Técnico avanzado               | Usa código Java, habla de tipos, memoria y scope | Desarrolladores o compañeros de equipo |

## Ejercicio 5: Descomposicion

- **Paso 1:** Entregó la lista de 5 requisitos clave (Gestión de productos, Stock, Categorías, Alertas de stock bajo, Reporte de ventas).
- **Paso 2:** Entregó el diseño UML/clases (`Producto`, `Categoria`, `Inventario`) con sus atributos y tipos de datos.
- **Paso 3:** Generó el código completo en Java para la clase `Producto` con atributos privados, constructor, getters y setters.
- **Paso 4:** Ofreció 3 mejoras: validación en setters, método `toString()` formateado y manejo de excepciones en cantidades negativas.

## Ejercicio 6: Prompt estructurado y autocritica

| Qué revisar                                      | Cumple (Sí / No) |
| ------------------------------------------------ | ---------------- |
| ¿Tiene las 4 columnas pedidas?                   | Sí               |
| ¿Incluye el bloqueo después de 3 intentos?       | Sí               |
| ¿Incluye casos con campos vacíos?                | Sí               |
| ¿Indica qué casos agregó en la autocrítica?      | Sí               |
| ¿Hay algún caso repetido o que no tenga sentido? | No               |

```text
Actua como analista de pruebas de software.
Login web con correo y contrasena. La cuenta se bloquea despues de 3 intentos fallidos.
Piensa paso a paso que puede fallar y escribe 6 casos de prueba.
Tabla con las columnas: ID, escenario, datos de entrada, resultado esperado.

- [Bitacora de tecnicas avanzadas](prompts/BITACORA.md)
```
