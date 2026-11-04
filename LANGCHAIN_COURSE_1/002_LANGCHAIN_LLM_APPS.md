# Qué es Langchain

- Framework para construir aplicaciones avanzadas de LLM
- Permite integrar memoria, herramientas y agentes en una estructura modular
- Facilita la creación de asistentes inteligentes personalizados y escalables

# LLM Apps

- Software que utiliza modelos de lenguaje para realizar tareas específicas
- Puede incluir asistentes personales, sistemas de respuesta de cliente y más.
- Combina capacidades de IA con interfaces de usuario y lógica de negocio

## Arquitectura de una aplicación tradicional:

![[Pasted image 20261103165044.png]]

## Arquitectura de LLM app

![[Pasted image 20261103165204.png]]

### Preprocesamiento de los datos

- Un pipeline envía datos a un LLM que ayuda a crear embeddings para guardarlos en una DB vectorial.

![[Pasted image 20261103165326.png]]

### Prompt Construction/Retrieval 

- El usuario hace una pregunta que va al hosting (donde está alojada la aplicación), y luego se va al orquestador que puede ser langchain
- El orquestador puede recuperar la información de algún prompt directo al LLM, o puede recuperar la información por medio de una API/plugin, **o podemos recuperar la informacióñ de nuestra base de datos de vectores**

![[Pasted image 20261103165559.png]]

### Prompt Execution/Inference

- Una simple query de usuario que viaja al LLM y la información se puede recuperar de diversas formas

![[Pasted image 20261103170027.png]]

> [!NOTE]
> Herramientas como Langchain permiten configurar toda esta arquitectura de LLMs dentro de las aplicaciones


