# Análisis de ventas — US Superstore

Proyecto de análisis exploratorio de datos (EDA) desarrollado en Python a partir del conjunto de datos **US Superstore**, con registros de pedidos de una tienda minorista de Estados Unidos entre 2014 y 2017.

El propósito es explorar el comportamiento de las ventas y la rentabilidad e identificar patrones relacionados con los productos, los clientes, las regiones, los descuentos y los tiempos de envío.

## Contenido del análisis

El proyecto contempla el análisis de estas dimensiones:

- **Ventas y rentabilidad:** evolución de las ventas y las ganancias a lo largo del tiempo.
- **Productos:** desempeño por categoría y subcategoría.
- **Descuentos:** relación entre los descuentos aplicados y la utilidad.
- **Distribución geográfica:** comportamiento por región y estado.
- **Clientes:** comparación de los segmentos de clientes.
- **Envíos:** análisis de las modalidades y los tiempos de envío.

Los gráficos, resultados y conclusiones específicos se encuentran en el notebook.

## Estructura del proyecto

Coloca los archivos en la misma carpeta, por ejemplo:

```text
US-Superstore/
├── Superstore.ipynb
├── US_Superstore_data.xls
├── requirements.txt
└── README.md
```

**Importante:** el archivo de datos está en la carpeta raíz, junto al notebook. No hace falta crear una carpeta `data/` con esta estructura.

## Requisitos

- Python 3
- Jupyter Notebook
- Las dependencias incluidas en `requirements.txt`

Librerías principales:

| Librería | Uso |
|---|---|
| `pandas` | Lectura, limpieza y manipulación de datos. |
| `numpy` | Operaciones numéricas. |
| `matplotlib` | Creación de gráficos. |
| `seaborn` | Visualización y exploración de datos. |
| `xlrd` | Lectura de archivos Excel `.xls`. |
| `jupyter` | Ejecución del notebook. |

## Instalación y ejecución

1. Abre una terminal en la carpeta del proyecto.
2. (Recomendado) Crea un entorno virtual:

   ```bash
   python -m venv .venv
   ```

   Actívalo en Windows:

   ```bash
   .venv\Scripts\activate
   ```

   O en macOS/Linux:

   ```bash
   source .venv/bin/activate
   ```

3. Instala las dependencias:

   ```bash
   python -m pip install -r requirements.txt
   ```

4. Inicia Jupyter:

   ```bash
   jupyter notebook
   ```

5. Abre `Superstore.ipynb` y ejecuta las celdas en orden.

Asegúrate de ejecutar el notebook desde la carpeta raíz y de mantener allí el archivo `US_Superstore_data.xls`. Si necesitas definir la ruta en el código, utiliza:

```python
file_path = "US_Superstore_data.xls"
```

## Descripción del conjunto de datos

El archivo `US_Superstore_data.xls` contiene **9.994 registros** y **21 columnas**. Cada fila representa una línea de pedido.

| Campo | Descripción |
|---|---|
| `Row ID` | Identificador de la fila. |
| `Order ID` | Identificador del pedido. |
| `Order Date` | Fecha en que se realizó el pedido. |
| `Ship Date` | Fecha de envío. |
| `Ship Mode` | Modalidad de envío. |
| `Customer ID` | Identificador del cliente. |
| `Customer Name` | Nombre del cliente. |
| `Segment` | Segmento del cliente. |
| `Country` | País. |
| `City` | Ciudad. |
| `State` | Estado. |
| `Postal Code` | Código postal. |
| `Region` | Región geográfica. |
| `Product ID` | Identificador del producto. |
| `Category` | Categoría del producto. |
| `Sub-Category` | Subcategoría del producto. |
| `Product Name` | Nombre del producto. |
| `Sales` | Importe de la venta. |
| `Quantity` | Cantidad de unidades. |
| `Discount` | Descuento aplicado. |
| `Profit` | Ganancia o pérdida de la línea de pedido. |

## Notas

- El formato `.xls` requiere `xlrd` para poder leerse con pandas.
- Si cambias el nombre o la ubicación del archivo de datos, actualiza la ruta correspondiente en el notebook.
- Ejecuta las celdas en orden para asegurar que las variables se definan antes de utilizarlas.

---

**Tecnologías:** Python · Jupyter Notebook · pandas · NumPy · Matplotlib · Seaborn
