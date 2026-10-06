# AI-Assistant
AI ASSISTANT es una plataforma o motor con IA que permite la generación y ejecución de aplicaciones con asistencia directa de un modelo pequeño LLM corriendo en modo local. Funciona combinando un agente local con un agente en la nube para orquestar tareas y brindar soporte en el desarrollo y operación de sistemas inteligentes.

<img width="1365" height="720" alt="AI_assistant_0" src="https://github.com/user-attachments/assets/46b6c53d-3c2a-46fe-bbe9-ce470bd374b7" />
---

## Aplicaciones con o sin asistencia LLM (Ver 1er video) 
[![Demo1 en YouTube](https://img.shields.io/badge/▶_Ver_demo-YouTube-red)](https://www.youtube.com/watch?v=f2EUEjG1ETk)

La plataforma AI ASSISTANT ayuda a crear proyectos que pueden funcionar con distintos niveles de inteligencia artificial.
El enfoque es ofrecer una herramienta flexible para facilitar la creación de aplicaciones para IoT, control o automatización, pudiendo operar con o sin asistencia explícita de un modelo LLM.
Dentro de las herramientas de nuestra aplicacion, tenemos un editor para la generación de dashboards para proyectos pequeños (Ej. ESP8266/ESp32, etc), mostrando una base inicial en la que se pueden incorporar capacidades inteligentes.

---

## Desarrollo colaborativo con modelos de inteligencia artificial pequeños: método hormiga para programación local
En el video detallamos la experiencia de desarrollar software utilizando un modelo de inteligencia artificial local de tamaño reducido, específicamente el Qwen 2.5 Coder con 3 mil millones de parámetros. Dada la limitación computacional de la máquina (un Ryzen 7 con 8 GB de RAM), adoptamos un enfoque metódico y paciente denominado "trabajo hormiga", que consiste en dividir el proyecto en pequeñas tareas y avanzar paso a paso, respetando un plan estructurado. El modelo no puede manejar grandes contextos ni proyectos extensos de una sola vez; por ello, se genera previamente un plan o “árbol” que sintetiza las funciones y responsabilidades de cada archivo para facilitar la comprensión del modelo y evitar sobrecargar su memoria limitada.

Lejos de ser una herramienta infalible, el modelo 3B presenta varios problemas como inventar APIs inexistentes, generar código erróneo, entrar en bucles o desviar sus respuestas espontáneamente. Ante esto, desarrollamos una metodología rigurosa donde nosotros los humanos con o sin la ayuda de el "Agente Local" o el "Agente en la Nube" actuamos como director y validador, el modelo como ejecutor y programador fragmentado, y una tercera entidad -una especie de asistente o agente- se encarga de mantener el plan actualizado, traducir instrucciones y controlar el flujo del trabajo. Además, implementamos varias reglas y filtros backend para forzar formatos y condiciones, asegurando que el código generado respete dependencias, prioridades y estructura, minimizando errores y manteniendo la integridad del proyecto.

Si bien este método, aunque lento y demandante, ofrece una alternativa para desarrollar proyectos de IA local en hardware modesto. Si bien no es un proceso rápido ni perfecto, aporta valiosa experiencia y abre posibilidades para crear soluciones personalizadas sin depender de grandes infraestructuras cloud. 

### Highlights
🐜 Introducción del método “trabajo hormiga” para proyectos con IA en hardware limitado.
💻 Uso del modelo Qen 2.5 Coder 3B con 3 mil millones de parámetros para programación local.
🗂️ Creación de un plan o árbol que sintetiza funciones y dependencias para evitar sobrecarga.
⚠️ Identificación de las limitaciones y "manías" del modelo, como errores y respuestas inconsistentes.
👨‍💻 Definición de roles claros: creador/director, modelo/ejecutor y asistente/agente.
🔧 Implementación de reglas backend para controlar calidad y flujo del código generado.
🤝 Enfoque colaborativo, iterativo y paciente para lograr proyectos funcionales en máquinas modestas.

### Insights clave
🐜 El método “trabajo hormiga” es fundamental para evitar la sobrecarga: Al fragmentar el proyecto en tareas pequeñas y ordenadas, se minimiza la necesidad de que el modelo procese contextos amplios y se mantienen constantes los recursos limitados, lo cual es clave para ejecutar modelos 3B en equipos con poca RAM.

⚙️ La generación previa de un plan sintético es una solución innovadora pero necesaria: Dado que el modelo tiene dificultad para manejar archivos extensos, conceptualizar un plan simplificado que describa las funciones y dependencias es esencial para mantener la coherencia en la creación y modificación de código, evitando así la repetición de lecturas pesadas.

🤖 Los modelos IA pequeños tienen un comportamiento probabilístico e impredecible: La misma pregunta puede arrojar resultados variables, y a menudo inventan detalles como APIs falsas o fallan al interpretar errores reales, lo que obliga a implementar mecanismos externos de validación y corrección de forma sistemática.

👨‍🎓 El rol del humano como director y validador es irremplazable en este esquema: La IA no puede asumir la responsabilidad de la visión global ni la depuración final. La supervisión constante y la toma de decisiones sobre la descomposición del proyecto y validación práctica aseguran que el trabajo avance y se mantenga funcional.

🛠️ Implementar reglas de backend que controlen la estructura y dependencias asegura integridad: Forzar formatos, resolver orden de ejecución y bloquear código que viola reglas permite reducir errores y vueltas atrás, constituyendo una suerte de "correa de transmisión" que corrige y guía al modelo.

⏳ La paciencia y la iteración son insumos críticos para el éxito: Más que velocidad, el creador enfatiza el valor de avanzar paso a paso, validar cada pieza y no pedir demasiado al modelo a la vez para evitar que se “colapse” o brinde malas respuestas, lo que se alinea con la analogía de una hormiga que avanza lentamente hacia la meta.

🌍 Esta metodología abre caminos para usar IA localmente en hardware modesto: Se postula como una opción viable para desarrolladores con máquinas limitadas, que no desean depender de servicios en la nube ni grandes infraestructuras, democratizando el acceso a la inteligencia artificial aplicada al desarrollo de software personalizado.

En resumen, como mostramos en el video, ofrecemos una guía realista y práctica para trabajar con modelos de IA pequeños en entornos con recursos limitados. Nuestro enfoque, basado en la división granular de tareas, la anticipación de limitaciones y una fuerte supervisión humana, permite avanzar en la construcción de proyectos complejos sin requerir hardware extremo, abriendo un espacio para usuarios y desarrolladores conscientes de estas restricciones.

---

## Uso del motor AI ASSISTANT para control aplicado a la Industria (Ver 2do video)
[![Demo2 en YouTube](https://img.shields.io/badge/▶_Ver_demo-YouTube-red)](https://www.youtube.com/watch?v=A7ANInk5d_E)

En este video explicamos cómo utilizar un modelo pequeño de inteligencia artificial (IA) ejecutándose de manera local para desarrollar y controlar un sistema SCADA aplicado al control de baterías petroleras. El proceso comienza con la vectorización y generación de “píldoras” de información contenidas en documentos técnicos, que se usan como contexto para alimentar al modelo IA local. Posteriormente, se configura un plan de trabajo dividido en tareas específicas para construir el programa, que en este caso es un SCADA desarrollado 100 % en Python, descartando otras herramientas orientadas a proyectos IoT pequeños.

Tambien mostramos cómo esta inteligencia artificial puede operar en tres modos: manual, asistido y automático. 
- En modo manual, el operador tiene control total del proceso.
- En modo asistido, la IA alerta y sugiere soluciones cuando detecta irregularidades.
- Y en modo automático, el sistema toma decisiones por sí mismo para solucionar problemas.

A pesar de contar con capas de seguridad, se reconoce que la IA puede cometer errores y el operador puede intervenir para corregirlos.

Finalmente, y creo que es uno de los moemntos mas destacados del video, presentamos una modalidad de entrenamiento con simulaciones de fallas precargadas que permiten evaluar la capacidad del modelo e incluso los operadores, con un puntaje basado en su desempeño. 
para concluir, la clave está en usar estas herramientas adecuadamente para complementar el control humano y mejorar la eficiencia en procesos industriales complejos.

### Puntos Destacados
🤖 Vectorización y creación de “píldoras” con datos técnicos para alimentar modelos IA locales.
🔄 Generación automatizada de planes y tareas para construir aplicaciones específicas.
🐍 Uso de Python para implementar un sistema SCADA adaptado a control industrial.
🕹️ Tres modos operativos: manual, asistido y automático, cada uno con distintos niveles de control.
⚠️ La IA puede detectar anomalías y sugerir soluciones; el operador puede intervenir en modo automático.
🎯 Módulo de entrenamiento y simulación para medir y mejorar el desempeño del modelo IA.
🛠️ Aplicabilidad amplia de la estrategia para integrar IA local en procesos de control industriales.

### Análisis de Insights Clave
🤖 Integración de IA Local y Contextualización Mediante Vectorización: La generación de “píldoras” vectorizadas permite que el modelo IA comprenda y retenga información técnica específica, creando un contexto sólido que facilita respuestas más precisas y adaptadas al dominio industrial, en lugar de depender exclusivamente de modelos generales en la nube. Esto es vital para mantener la privacidad y la velocidad en la ejecución.

🔄 Automatización Eficiente Mediante Planes y Tareas Generados por IA: La capacidad del agente en la nube para transformar documentos vectorizados en un plan estructurado con tareas claras y detalladas destaca una nueva manera de automatizar el desarrollo de aplicaciones industriales, reduciendo significativamente la carga del desarrollo manual y aumentando la coherencia en la arquitectura del software.

🐍 Elección Tecnológica Adaptada a la Escala del Proyecto: La decisión de abandonar la solución rápida y pequeña (Dashw para IoT tipo ESP32) en favor de un SCADA 100 % desarrollado en Python evidencia una adecuada evaluación técnica del proyecto. Python brinda la robustez, escalabilidad y flexibilidad necesarias para procesos industriales complejos y muestra el valor de personalizar herramientas según necesidades reales.

🕹️ Diversidad de Modos de Operación para Ampliar la Seguridad y Flexibilidad: El diseño con tres modos (manual, asistido y automático) refleja una comprensión profunda de las dinámicas del control industrial, ya que permite a los operadores intervenir cuando sea necesario, dar lugar a una asistencia inteligente para corregir problemas y permitir automatización completa cuando se confía en la IA, habilitando así escenarios de operación adaptativos y seguros.

⚠️ Reconocimiento de Riesgos y Necesidad de Supervisión Humana: A pesar del avance en la autonomía de la IA, se reconoce que errores pueden ocurrir, reforzando la importancia de mantener al operador como última instancia de control. Esto es fundamental para evitar fallos catastróficos y lograr un equilibrio adecuado entre automatización y supervisión humana, crucial para entornos industriales donde la seguridad es prioritaria.

🎯 Sistema de Entrenamiento Basado en Simulación de Fallas para Mejorar el Modelo: La implementación de fallas controladas y la posterior evaluación mediante scoring permiten no solo medir la capacidad de respuesta de la IA, sino también entrenarla y mejorarla continuamente. Esta retroalimentación es esencial en sistemas críticos, pues incrementa la confiabilidad y robustez del control automatizado.

🛠️ Versatilidad del Enfoque para Proyectos Industriales con IA Local: El modelo demostrado puede replicarse y adaptarse para distintos procesos y sectores industriales, validando la estrategia de usar modelos de IA pequeños en local para asistir y potenciar proyectos que requieran rapidez, confidencialidad y adaptación específica al contexto operativo, abriendo camino a futuras implementaciones escalables.

Este video refuerza una visión práctica y moderna de la aplicación de inteligencia artificial en la automatización industrial, enfatizando la combinación de tecnología local y en la nube, contextos personalizados y la mirada crítica hacia la supervisión y entrenamiento continuo.

# Ventas y Soporte Técnico:
prof.martintorres@educ.ar

