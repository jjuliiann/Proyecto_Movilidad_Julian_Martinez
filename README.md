# Proyecto: Mi Flujo Profesional de Datos \- Análisis de Movilidad Global (Chile)

## Descripción del proyecto

Este proyecto tiene como objetivo transformar un conjunto de datos "crudo" de movilidad (Google COVID-19) en un dataset limpio, procesado y documentado bajo estándares profesionales de ciencia de datos. El flujo de trabajo integra la carga, limpieza, transformación avanzada y visualización de datos, asegurando la reproducibilidad mediante el uso de Git y GitHub.

## **Integrantes:**

* **Dueño del Repositorio:** Julian Martinez  
* **Colaborador 1:** Lucas Fernandez  
* **Colaborador 2:** Vicente Castro

## **Fases del Flujo de Datos**

### **1\. Entorno de Trabajo y Versionado**

* **Herramientas:** Uso de Git para el control de versiones con al menos 3 commits que evidencian el avance de cada fase.  
* **Colaboración:** Trabajo basado en ramas (*branching*) para separar las tareas de limpieza y transformación de la rama principal (main).

### **2\. Limpieza de Datos (Data Cleaning)**

Se trabajó con el archivo Global Mobility Report.csv, realizando las siguientes acciones:

* **Filtrado:** Selección exclusiva de registros pertenecientes a **Chile** (country region) para optimizar el procesamiento.  
* **Manejo de Nulos:** Identificación de celdas vacías con decisiones justificadas de borrado o imputación.  
* **Duplicados:** Eliminación de registros repetidos por fecha y subregión.  
* **Outliers:** Detección de variaciones de movilidad imposibles para asegurar la calidad de la información.

3\. Transformación Avanzada (Feature Engineering)  
Preparación del dataset para análisis profesional:

* **Tipado:** Conversión de la columna date a formato datetime.  
* **Ingeniería de Atributos:** Creación de la columna movilidad promedio basada en el promedio de las categorías de movilidad.  
* **Escalamiento:** Aplicación de StandardScaler o MinMaxScaler a las columnas numéricas.  
* **Codificación:** Uso de OneHotEncoder para las variables categóricas de las subregiones.

## **Visualización Final**

El proyecto incluye un gráfico de líneas (sns.lineplot) que resume el comportamiento de la movilidad promedio en Chile a través del tiempo, permitiendo visualizar el impacto del preprocesamiento.

## **Reflexión sobre Reproducibilidad**

La reproducibilidad es la capacidad de obtener los mismos resultados siguiendo el mismo flujo de trabajo, sin importar quién lo ejecute. En este proyecto, el uso de Git y la documentación detallada en celdas de Markdown garantizan que cualquier científico de datos pueda replicar nuestro análisis de principio a fin sin pérdida de información.

## **Cómo ejecutar este proyecto**

1. Clonar el repositorio:  
   git clone https://github.com/USUARIO\_DUEÑO/Proyecto\_Movilidad\_NombreApellido.git  
2. Asegurarse de tener instalado Pandas, Seaborn y Scikit-Learn.  
3. Ejecutar el notebook .ipynb de forma secuencial.

