# Chatbot Question Simulator

Este proyecto implementa una interfaz gráfica tipo chatbot que se ejecuta localmente en la siguiente URL:

http://127.0.0.1:5001

## Objetivo

Simular un chatbot capaz de registrar, buscar y gestionar preguntas/respuestas, ofreciendo una experiencia visual amigable para la interacción del usuario.

## Funcionalidades principales

### Registro de preguntas
- Permite ingresar una pregunta en lenguaje natural.
- Si no existe respuesta, la pregunta queda registrada con estado `0` (pendiente o `false`).
- Si ya ha sido respondida, se marca con estado `1` (respondida o `true`).

### Búsqueda de preguntas
- Se pueden buscar preguntas completas (coincidencia exacta).
- También permite búsqueda por palabras clave.
- Si existen múltiples coincidencias con las keywords, todas son listadas.

### Escenarios contemplados
1. Pregunta nueva sin respuesta  
   Se registra con estado `0`, y el sistema notifica que la pregunta fue guardada pero aún no tiene respuesta.

2. Pregunta ya registrada con respuesta  
   Se muestra la respuesta correspondiente y el estado es `1`.

3. Pregunta ya registrada sin respuesta  
   Se notifica que la pregunta está registrada pero aún no se ha respondido.

4. Múltiples coincidencias por keywords  
   El sistema lista todas las preguntas similares junto con su estado de respuesta.

