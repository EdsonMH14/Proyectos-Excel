# 📊 Búsqueda de Empleados en Excel

Este proyecto consiste en una herramienta desarrollada en **Microsoft Excel** que permite **consultar información detallada de empleados** a partir de su **ID de empleado**, facilitando la gestión y búsqueda dentro de una base de datos.

## 🧩 Descripción del proyecto

El archivo está diseñado para **buscar automáticamente los datos de un empleado** al seleccionar su **ID** desde una lista desplegable. Toda la información se muestra de forma organizada y clara en una tabla resumen, incluyendo datos personales, cargo, salario, fechas, y más.

La búsqueda funciona incluso cuando los datos están almacenados en **otras hojas de Excel**, gracias a la implementación de fórmulas y validaciones inteligentes.

## ⚙️ Herramientas y funciones utilizadas

- **Importación de datos** desde:
  - Un archivo **Bloc de notas (.txt)**
  - Un documento **Word (.docx)**
- **Fórmula principal:** `BUSCARV` (VLOOKUP)
  - Utilizada para extraer los datos correspondientes al ID seleccionado.
- **Validación de datos:**
  - La celda del **ID de empleado** solo acepta **números válidos**.
  - Se implementó una **lista desplegable** con todos los IDs disponibles.
- **Formato condicional y diseño:**
  - Se aplicaron colores, bordes y estilos para mejorar la presentación visual y la comprensión de la información.

## 🧠 Funcionamiento

1. El usuario selecciona un **ID de empleado** desde la lista desplegable.
2. Excel realiza automáticamente la búsqueda con `BUSCARV` en las hojas correspondientes.
3. Se rellenan los campos de la tabla con los datos del empleado.
4. La información incluye:
   - Nombre y apellido  
   - Cargo y salario  
   - Facultad y seccional  
   - Fechas de ingreso y nacimiento  
   - Datos de contacto (domicilio, ciudad, teléfono, correo)


## 🚀 Objetivo del proyecto

Este proyecto tiene como propósito **demostrar el uso de funciones avanzadas de Excel** para automatizar tareas de búsqueda y organización de datos, integrando información desde diferentes fuentes y aplicando buenas prácticas en diseño y validación.


## 🧾 Autor

**Edson Martínez Hernández**  
📍 Veracruz, México  
💼 Ingeniería en Sistemas Computacionales, especialidad en Ciencia de Datos Aplicada.  

---

✨ *Este proyecto es un ejemplo práctico del uso de Excel para gestión de datos y automatización de consultas mediante funciones y validaciones.*
