# 📊 Diagrama de Gantt en Excel

Este proyecto muestra cómo crear un **Diagrama de Gantt dinámico** en Excel, utilizando funciones lógicas, búsqueda de datos y formato condicional para visualizar periodos de trabajo por persona, área o actividad.

## 🧩 Descripción del proyecto

El objetivo fue construir un gráfico tipo Gantt que permita:
- Visualizar el tiempo de trabajo de cada persona.
- Clasificar las tareas por **área o categoría** (Ventas, Mantenimiento, Desarrollo, etc.).
- Cambiar dinámicamente el **intervalo de tiempo** mostrado en el gráfico.
- Identificar visualmente diferentes áreas mediante **colores personalizados**.

## ⚙️ Funcionalidades principales

- **Función `Y()`** → Permite realizar pruebas lógicas múltiples para determinar si una fecha se encuentra dentro de un rango.
- **Función `BUSCARV()`** → Utilizada para obtener la fecha de inicio, fecha de fin y categoría desde una tabla principal.
- **Nombres de rango estáticos** → Facilitan la gestión de referencias en las fórmulas y mejoran la legibilidad del archivo.
- **Formato condicional** → Asigna colores distintos según el área (por ejemplo, Ventas, Mantenimiento, Desarrollo).
- **Intervalo de tiempo modificable** → Se puede ajustar el incremento de fechas (por semanas, quincenas o meses) para modificar el gráfico dinámicamente.

## Estructura del proyecto

- Hoja1 (Diagrama de Gantt): La hoja principal donde se visualiza el gráfico. Contiene las fórmulas y el formato condicional aplicado a la matriz de tiempo.
- Hoja2 (Datos de Origen): Contiene la tabla de datos (tabla2) con los nombres de los recursos, fechas de inicio y fin, el área y un campo auxiliar usado para la categorización en el Gantt.


## 🧮 Fórmula principal

Ejemplo de fórmula usada en el diagrama:

```excel
=SI(
  Y(
    BUSCARV($A2, tabla, 2, FALSO) <= B$1,
    BUSCARV($A2, tabla, 3, FALSO) >= B$1
  ),
  BUSCARV($A2, tabla, 5, FALSO),
  0
)
```

## Autor
Ing. Edson Martínez Hernández
Especialidad: Ciencia de datos aplicada.
📍 Veracruz, México.
💼 Proyecto académico y de práctica en gestión de tiempos con Excel.


