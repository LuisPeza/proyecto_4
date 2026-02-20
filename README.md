# Proyecto 4: Análisis de Hábitos de Consumo en Instacart
> **Manipulación y Limpieza de Datos a Gran Escala**

---

## 📝 Descripción del Proyecto
[Instacart](https://www.instacart.com) es una plataforma líder en entrega de comestibles que conecta a clientes con tiendas locales. En este proyecto, se analiza un conjunto de datos real para extraer patrones de compra, optimizar el inventario y entender el comportamiento de los usuarios.

### 🎯 Objetivo
Realizar un proceso integral de **Data Wrangling**: desde la carga y limpieza profunda de datos hasta la generación de visualizaciones que comuniquen insights clave sobre los hábitos de compra de los consumidores.

---

## 📂 Diccionario de Datos

El análisis se basa en cinco conjuntos de datos interconectados que describen el ecosistema de pedidos:

### 1. Pedidos (`instacart_orders.csv`)
| Columna | Descripción |
| :--- | :--- |
| `order_id` | ID único del pedido. |
| `user_id` | ID único del cliente. |
| `order_number` | Número secuencial de pedidos realizados por el cliente. |
| `order_dow` | Día de la semana (0 = Domingo). |
| `order_hour_of_day` | Hora de captura del pedido. |
| `days_since_prior_order` | Días transcurridos desde la última compra. |

### 2. Productos y Categorías
Se utilizan tablas de referencia para enriquecer la información de los artículos:
* **Productos:** Contiene `product_id` y `product_name`.
* **Pasillos (`aisles`):** Clasificación por tipo de estante (`aisle_id`, `aisle`).
* **Departamentos:** Segmentación por área de negocio (`department_id`, `department`).

### 3. Detalle de Carrito (`order_products.csv`)
Relaciona los pedidos con los productos, indicando el `add_to_cart_order` (orden de selección) y si el artículo es `reordered` (recompra).

---

## 🛠️ Metodología y Conclusiones



### 🔍 1. Exploración de Datos
Se realizó un diagnóstico inicial de los 5 archivos fuente. Se identificó la estructura de las bases de datos y se detectaron inconsistencias críticas como valores nulos en la columna de días desde el pedido anterior y registros duplicados que podrían sesgar el análisis.

### 🧹 2. Procesamiento y Limpieza
Para garantizar la integridad de los resultados, se ejecutaron las siguientes acciones:
* **Tratamiento de nulos:** Se sustituyeron valores ausentes por datos coherentes o indicadores de "primer pedido".
* **Deduplicación:** Eliminación de filas repetidas tras confirmar que no representaban eventos únicos.
* **Optimización:** Ajuste de tipos de datos para mejorar el rendimiento del procesamiento.

### 📈 3. Análisis de Insights
El análisis final permitió responder preguntas estratégicas de negocio:
* **Picos de Demanda:** Identificación de los días y horas con mayor tráfico de pedidos.
* **Fidelización:** Cálculo de la tasa de recompra y análisis del tiempo promedio entre pedidos.
* **Comportamiento del Carrito:** Determinación del volumen promedio de artículos por pedido y los productos "ancla" (aquellos que se añaden primero al carrito).

---

## 🏁 Conclusión General
El análisis revela oportunidades claras de optimización. Conocer los hábitos de compra permite al negocio:
1.  **Optimizar el Stock:** Asegurar disponibilidad de los productos con mayor rotación.
2.  **Marketing Dirigido:** Crear promociones en los días de baja actividad para nivelar la carga operativa.
3.  **Experiencia de Usuario:** Posicionar productos clave para facilitar el proceso de compra basado en la secuencia de selección detectada.

---

## 🔗 Entregables
* [📂 Ver Jupyter Notebook con el Análisis Completo](https://github.com/LuisPeza/proyecto_4/blob/main/proyecto_4_bien.ipynb)
