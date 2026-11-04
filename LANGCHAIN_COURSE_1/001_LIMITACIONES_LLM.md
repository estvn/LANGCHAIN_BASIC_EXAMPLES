# Por qué son necesarias estas herramientas?

# Limitaciones de los LLM

- Conocimiento desactualizado
- Incapacidad para realizar acciones interactivas
- Falta de contexto
- Alucinaciones
- Sesgos y discriminación
- Falta de transparencia - no hay fuente real

# Como podemos mitigar las limitaciones?

## Retrieval Augmentation (Aumento por recuperación)

- Esta técnica accede a bases de conocimiento externas para complementar los datos de entrenamiento desactualizados de un LLM, o bien datos privados, proporcionando contexto externo y reduciendo el riesgo de alucinaciones.

## Chaining 

- Esta técnica integra acciones como búsquedas y cálculos dentro del flujo del LLM para permitir respuestas más dinámicas y basadas en datos reales.
- Los LLM son débiles a la hora de realizar operaciones aritméticas.

## Prompt Engineering

- Involucra la creación cuidadosa de prompts, proporcionando contexto crítico que guía a respuestas apropiadas y relevantes

## Monitoreo, filtrado y revisiones

- Incluye la supervisión continua y efectiva de los problemas emergentes relacionados con los inputs y outputs de la aplicación **para detectar y corregir problemas**
	- Filtros: Lista de bloqueo, clasificadores de sensibilidad y filtros de palabras prohibidas, pueden identificar automáticamente problemas
	- Revisiones humanas: Proporcionan perspectivas sobre el comportamiento del modelo y la calidad de las respuestas

## Memoria 

- Retiene el contexto de la conversación al persistir los datos y el contexto de la interacción a lo largo del tiempo, lo que mejora la coherencia y relevancia de las interacciones sucesivas.

## Fine-tunning 

- Entrenamiento y ajuste de LLM con datos más apropiados para el dominio y principios de la aplicación, adaptando el comportamiento del modelo para su propósito específico.
- 