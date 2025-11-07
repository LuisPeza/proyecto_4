<h1>Proyecto_4 </h1>
Manipulación de datos

<h2>Descripcion del proyecto</h2>

🍕🍟🍤🍝🍲Instacart es una plataforma de entregas de comestibles donde la clientela puede registrar un pedido y hacer que se lo entreguen, similar a Uber Eats y Door Dash.🥮🥧🍱

<h3>Objetivo </h3>

Tu misión es limpiar los datos y preparar un informe que brinde información sobre los hábitos de compra de los clientes de Instacart. Después de responder a cada pregunta, escribe una breve explicación de tus resultados en una celda markdown de tu Jupyter notebook.

Este proyecto requerirá que hagas gráficos que comuniquen tus resultados.

<h3>Descripción de los datos</h3>

Cada fila corresponde a un pedido en la aplicacion instacart

- instacart_orders.csv: cada fila corresponde a un pedido en la aplicación Instacart.
- 'order_id': número de ID que identifica de manera única cada pedido.
- 'user_id': número de ID que identifica de manera única la cuenta de cada cliente.
- 'order_number': el número de veces que este cliente ha hecho un pedido.
- 'order_dow': día de la semana en que se hizo un pedido (0 si es domingo).
- 'order_hour_of_day': hora del día en que se hizo el pedido.
- 'days_since_prior_order': número de días transcurridos desde que este cliente hizo su pedido anterior.

Productos unicos que pueden comprar.

'product_id': número ID que identifica de manera única cada producto.
'product_name': nombre del producto.
'aisle_id': número ID que identifica de manera única cada categoría de pasillo de víveres.
'department_id': número ID que identifica de manera única cada departamento de víveres.

Articulo solicitado en un pedido.

- 'order_id': número de ID que identifica de manera única cada pedido.
- 'product_id': número ID que identifica de manera única cada producto.
- 'add_to_cart_order': el orden secuencial en el que se añadió cada artículo en el carrito.
- 'reordered': 0 si el cliente nunca ha pedido este producto antes, 1 si lo ha pedido.

información del pasillo

- 'aisle_id': número ID que identifica de manera única cada categoría de pasillo de víveres.
- 'aisle': nombre del pasillo.

información del departamento 

- 'department_id': número ID que identifica de manera única cada departamento de víveres.
- 'department': nombre del departamento.
