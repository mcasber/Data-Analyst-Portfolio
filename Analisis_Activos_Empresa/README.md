# 📊 Análisis de Activos "Empresa" - Portafolio de Data Analyst

## 📋 Descripción General del Proyecto

Este proyecto se enfoca en el análisis exploratorio de datos (EDA) y la preparación de datos (ETL) sobre los activos de una empresa (equipos y accesorios). El objetivo principal es consolidar información de diversas fuentes, limpiar y estandarizar los datos, y generar insights clave sobre el inventario de hardware. Este trabajo busca optimizar la gestión de activos y responder preguntas operativas y estratégicas sobre el estado y la distribución de los equipos.

## 🚀 Objetivos del Proyecto

1.  **Limpieza y Consolidación de Datos:** Unificar reportes de activos (.xls encapsulados en HTML) y enriquecerlos con información de un `.csv` adicional.
2.  **Identificación y Gestión de Datos Faltantes/Duplicados:** Abordar valores nulos en campos críticos como `serial`, `ubicación`, `dueño`, `gerencia`, `departamento` y `activo_fijo` (RFID).
3.  **Clasificación de Activos:** Agrupar los activos en categorías lógicas (Gerencias/Grupos) utilizando información de `ubicación`, `gerencia` y `departamento`.
4.  **Análisis de RFID:** Cuantificar y caracterizar los equipos que poseen un identificador RFID.
5.  **Análisis de Hardware Específico:** Identificar tipos de equipos (Workstations, Notebooks) y sus especificaciones de procesador (i3, i5, i7, i9, M1, M2).

## 🛠️ Tecnologías y Herramientas Utilizadas

*   **Python:** Lenguaje de programación principal.
*   **Pandas:** Para manipulación y análisis de datos.
*   **Numpy:** Soporte para operaciones numéricas.
*   **Matplotlib y Seaborn:** Para visualización de datos.
*   **Google Colab:** Entorno de desarrollo para Jupyter Notebooks.
*   **Google Drive:** Almacenamiento de datos de origen.

## 📂 Estructura del Repositorio

*   `Analisis_Activos_Empresa.ipynb`: El cuaderno Jupyter con todo el código del ETL, EDA y análisis.
*   `README.md`: Este archivo, con la descripción del proyecto.

## 🔍 Análisis y Resultados Clave

Durante el desarrollo del proyecto, se lograron los siguientes puntos clave:

*   **Integridad de Datos:** Se consolidó una base de datos única, manejando nulos y eliminando duplicados mediante estrategias como la imputación de `serial` con `id` y la eliminación de registros con `dueño` nulo.
*   **Normalización de RFID:** La columna `activo_fijo` fue estandarizada para crear un indicador binario `rfid` (1 si tiene, 0 si no), facilitando su análisis.
*   **Clasificación por Grupos:** Los activos fueron categorizados en gerencias/grupos como 'SISTEMAS', 'REDACCION', 'COMERCIAL', 'RRHH', etc., utilizando expresiones regulares para unificar criterios.
*   **Identificación de Stock:** Se distinguió entre equipos en uso y equipos en stock, permitiendo un análisis separado del inventario.
*   **Análisis de Procesadores:** Se extrajo y cuantificó la distribución de procesadores (i3, i5, i7, i9, M1, M2) en Workstations y Notebooks.

## 💡 Conclusiones e Insights

*   El proyecto demostró la capacidad de transformar datos brutos y desorganizados en una base de datos limpia y estructurada, lista para el análisis.
*   Se identificó la distribución de activos por gerencia, lo cual es fundamental para la planificación de recursos.
*   El análisis de RFID reveló el número y tipo de equipos que actualmente cuentan con esta tecnología, y se recomendo colocarlo en los faltantes para cumplir con los porcedimientos de seguridad.
*   El detalle sobre los procesadores de Workstations y Notebooks fue un dato que se tomo para evidenciar la falta de información en una gran parte de los equipos.
*   Investigar los activos clasificados como 'OTROS' para intentar asignarles una categoría más específica o entender por qué quedan fuera de las clasificaciones actuales.
*   Realizar un análisis de ciclo de vida de los activos, debido a que no se dispone de datos de fechas de adquisición se recomendo comenzar a incorporar este dato.

## 📧 Contacto

Si tienes preguntas o te interesa mi trabajo, no dudes en contactarme:

*   **Tu Nombre:** Mariano Martin Castelli
*   **LinkedIn:** [(https://www.linkedin.com/in/mariano-castelli-294520182/)]
*   **Email:** [mcastelli2014@gmail.com]

--- 
