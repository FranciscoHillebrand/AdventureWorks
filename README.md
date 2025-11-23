# 🚲 Adventure Works: Análisis de Rentabilidad y Mercado

![Status](https://img.shields.io/badge/Status-Finalizado-success?style=for-the-badge)
![Tools](https://img.shields.io/badge/Tools-SQL%20Server%20%7C%20Power%20BI-blue?style=for-the-badge)

## 📖 Descripción del Proyecto

Este proyecto consiste en un análisis de Business Intelligence realizado sobre la base de datos de **Adventure Works**, una empresa ficticia de manufactura y venta de bicicletas. El objetivo principal fue evaluar la rentabilidad histórica, el rendimiento de los productos y la eficiencia logística en distintos mercados internacionales.

El flujo de trabajo abarcó desde la **restauración y gestión de la base de datos en SQL Server**, pasando por el diseño de la experiencia de usuario (Mockups), hasta la implementación de un Dashboard interactivo en **Power BI**.

---

## ⚙️ Gestión de Base de Datos (SQL)

Para este análisis, se trabajó con una copia de seguridad real (`.bak`).

> **⚠️ Guía de Restauración:**
> El archivo de respaldo `AdventureWorks.bak` se encuentra disponible en este repositorio.
> Si deseas replicar el entorno, **consulta la sección "Desarrollo del proyecto / Avance N°1" dentro del archivo [`Informe.pdf`](./Informe.pdf)**. Allí explico paso a paso cómo restaurar la base de datos en SQL Server Management Studio (SSMS).

---

## 🎨 Diseño y Planificación

Antes de construir el tablero, se realizó una etapa de diseño y documentación para asegurar la calidad del dato y la usabilidad.

### 📚 Diccionario de Datos
Se documentó cada variable utilizada para garantizar la transparencia del análisis. Puedes consultar el diccionario completo en el archivo `Diccionario de Datos.xlsx`.

### 🖌️ Mockups vs. Resultado Final
Se diseñaron bocetos preliminares para definir la narrativa visual.
*(Aquí puedes subir tus imágenes de los mockups y del dashboard final)*

| Mockup Inicial | Dashboard Final en Power BI |
|:---:|:---:|
| ![Mockup](image_ec3124.png) | ![Dashboard](nombre_de_tu_imagen_dashboard.png) |

---

## 💡 Insights y Hallazgos de Negocio

Tras el procesamiento de los datos, se obtuvieron conclusiones clave para la estrategia de la empresa:

### 💰 Rentabilidad General
* **Negocio Saludable:** La organización es consistentemente rentable. Tanto la utilidad bruta como la neta se han mantenido positivas año tras año.
* **2013, El Año Dorado:** Fue el periodo de mayor éxito, alcanzando una utilidad neta de **$5.048.495**.
* **Estacionalidad:** Se detectó un patrón claro de aumento de utilidades brutas en los meses de **Junio, Octubre, Noviembre y Diciembre**.

### 🏆 Productos
* **Bicicletas (Estrella):** Son el motor de la compañía, generando millones en utilidades, especialmente las **Bicicletas de Carretera**.
* **El Misterio de los Componentes:** La categoría "Componentes" no registra utilidades visibles.
    * *Recomendación:* Auditar el inventario y proceso de ventas. ¿Están en stock pero no se ofertan? ¿Hay un error en el registro de datos?

### 🌎 Mercados Internacionales

| Región | Hallazgo | Análisis / Recomendación |
|:---:|:---|:---|
| **🇺🇸 Estados Unidos** | **Mayor Volumen.** Posee más clientes que toda Europa combinada y duplica a Australia. | La Costa Oeste (California, Washington, Oregon) genera los mayores ingresos, aunque con márgenes ajustados debido a altos costos operativos (COGS). |
| **🇨🇦 Canadá** | **Mejores Márgenes.** A pesar de tener 6,000 clientes menos que EE.UU., es el mercado más eficiente en rentabilidad relativa. | *Acción:* Analizar la estrategia de captación canadiense para intentar replicar su eficiencia en otros mercados. |
| **🇦🇺 Australia** | **Logística Costosa.** Es el 2° país con más clientes, pero sus costos de envío ($226k) son casi iguales a los de EE.UU. ($234k) con la mitad de volumen. | *Acción:* Evaluar la viabilidad de establecer un centro de distribución local o buscar proveedores cercanos para reducir el impacto logístico en la utilidad neta. |

---

## 🛠️ Stack Tecnológico

* **SQL Server:** Restauración de BD, consultas y validación de datos.
* **Power BI:** Modelado de datos (DAX), ETL y Visualización.
* **Presentaciones de Google:** Creación de Mockups y prototipado.

---

## 📁 Estructura del Repositorio

* `AdventureWorksDW2019`: Archivo `.bak` .
* `Informe.pdf`: Informe ejecutivo detallado con hallazgos y narrativa.
* `/Imagenes`: Capturas de los Mockups y el Dashboard final.
* `Dashboard.pbix`: Archivo fuente del tablero.

---
**Autor:** Francisco Javier Hillebrand
