# BotPyAi

Chatbot en Python que responde preguntas sobre **tus propios documentos PDF**, no sobre lo que el modelo haya memorizado.

## Cómo funciona

El problema de preguntarle a un modelo por un documento es que no lo ha leído, y si se le pega entero no cabe. Aquí el PDF se parte en fragmentos, cada fragmento se convierte en un vector que representa su significado, y al llegar una pregunta se buscan los fragmentos más cercanos a ella. Sólo esos van al modelo junto con la pregunta.

El resultado es que la respuesta sale del documento. Si algo no está ahí, el modelo no tiene de dónde inventarlo.

## Stack

Python · embeddings · LLM

## Configuración

Las llaves de API van en variables de entorno, nunca en el código.

> **Nota:** este repositorio es privado y debe seguir así hasta limpiar del historial las llaves que estuvieron versionadas en su momento.
