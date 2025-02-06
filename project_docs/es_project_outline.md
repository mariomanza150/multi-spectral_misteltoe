# **Caja de Herramientas para el Procesamiento de Imágenes Multiespectrales**

## **I. Objeto del Servicio**

**Monitoreo de especies de muérdago en parques urbanos usando imágenes aéreas e inteligencia artificial.**

Se requiere desarrollar una caja de herramientas (*toolbox*) para el co-registro y preprocesamiento de series de imágenes aéreas multiespectrales, que serán colectadas sobre los parques urbanos de la Ciudad de México: **Jardín Ramón López Velarde, Ex Convento Churubusco y Xochimilco**, en diferentes etapas fenológicas.

---

## **II. Descripción del Servicio**

El desarrollo de una base de datos especializada en la detección de diferentes especies de muérdago en parques urbanos de la Ciudad de México requiere la creación e implementación de un *toolbox* de código abierto, desarrollado en **Python**.

Este *toolbox* tendrá como objetivo principal el **co-registro de las imágenes aéreas multiespectrales**, un proceso necesario para garantizar la alineación exacta de las bandas multiespectrales capturadas por el sensor. Además, el *toolbox* incluirá:

- **Organización y renombrado de imágenes** para garantizar un orden consistente en cada uno de los vuelos.
- **Calibración espectral** de los valores de intensidad para derivar valores de reflectancia y corregir sesgos generados por variaciones en la iluminación.
- **Transformaciones geométricas** para asegurar la alineación espacial correcta de las bandas.
- **Extracción de características espectrales y de textura** para la detección de especies de muérdago.

---

## **III. Plan de Desarrollo**

| **Tarea** | **Duración Estimada** |
|-----------|--------------------|
| Desarrollo de un script en Python para organizar y renombrar automáticamente las imágenes. | 1-2 semanas |
| Cálculo de reflectancia de las bandas para corrección de iluminación. | 2-4 semanas |
| Implementación de transformaciones geométricas para co-registro de imágenes. | 4-7 semanas |
| Extracción de características espectrales y de textura para detección de especies. | 7-10 semanas |
| Integración del *toolbox* y validación final. | 10-12 semanas |

---

## **IV. Perfil del Personal Requerido**

Se requiere personal con formación en **Ciencias de Información Geoespacial, Ciencias de la Computación o áreas afines**, con conocimientos avanzados en:

- Procesamiento digital de imágenes.
- Programación en **Python**.
- Desarrollo de herramientas de código abierto.
- Manejo de imágenes multiespectrales.
- Experiencia previa en detección de especies forestales o análisis ambiental.
- Integración de herramientas computacionales con grandes volúmenes de datos geoespaciales.

Este equipo debe ser capaz de desarrollar soluciones escalables y eficientes para el procesamiento de imágenes en entornos de alto rendimiento.

---

## **V. Impacto Esperado**

- **Mejor detección y monitoreo de especies de muérdago** en parques urbanos.
- **Eficiencia en el procesamiento** de grandes volúmenes de imágenes multiespectrales.
- **Un *toolbox* modular y reutilizable** para análisis geoespacial en estudios ambientales.
- **Compatibilidad con estándares de sensores remotos y GIS**, permitiendo la integración con herramientas existentes en la comunidad científica.
