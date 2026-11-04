# Langchain Componentes Principales

# LLM Wrappers

- Los "LLM Wrappers" son abstracciones que encapsulan la interacción con modelos de lenguaje de gran escala (LLM), facilitando su integración y manejo dentro de aplicaciones más amplias.
- Para modelos que usan texto plano como entrada y salida

```
from langchain_openai import OpenAI

llm = OpenAI(api_key='')
```

# ChatModels

- Un modelo de chat es un tipo especializado de modelo de lenguaje que procesa y responde a entradas en formato de mensaje de chat, en lugar de texto plano. 
- Para modelos que usan mensajes de chat de entrada y salida 
- Entregaría arrays de strings

```
from langchain_openai import ChatOpenAI

chat = ChatOpenAI(model='gpt-3.5-turbo')
```

# Prompt Templates

- Son recetas predefinidas que facilitan la generación de prompts para modelos de lenguaje
- **Asegura que los prompts puedan ser utilizados de manera flexible y eficiente a través de diferentes modelos de lenguaje, maximizando la reusabilidad y minimizando la necesidad de rediseño constante.**

```
from langchain.prompts import PromptTemplate

promp_template = PromptTemplate.from_template(
	"Tell me an {adjective} joke about {content}"
)

prompt_template.format(adjective='funny', content='chickens')
```

# Retrieval Components

- Los componentes de recuperación en Langchain facilitan la interacción con datos específicos de la aplicación, permitiendo procesar y acceder a la información de manera eficiente y relevante

- Algunos ejemplos:
	- Document loaders - para consultar información de almacenes externos
	- Text splitters 
	- Vector stores
	- ...

