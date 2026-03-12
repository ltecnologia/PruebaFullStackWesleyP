### Prueba técnica fullstack

##EJ01

#¿Qué estructura de datos usas para "recordar" los logins pendientes de cada usuario mientras recorres los eventos?

un objeto para guardar los datos de la salida esperada

#¿Qué pasa si el mismo usuario tiene dos logins consecutivos sin logout en medio? ¿Tu código lo detecta o silencia el error?

silencia el error, un segundo login podría remplazar el anterior

#¿Importa el orden en que procesas los eventos? ¿Deberías ordenarlos primero?
 Si, es necesario ordenar los eventos ya que un logout podría ocurrir primero que un login


##EJ03

#¿Por qué el orden de las reglas importa matemáticamente? Si aplicaras el IVA antes del cupón, ¿el resultado sería el mismo?
No seria el mismo resultado, es necesario aplicar descuentos y cupones primero para evitar que el iva sea mas alto

#¿Cómo manejas el caso donde el cupón existe pero el total no alcanza el mínimo? ¿Error o simplemente no aplica?

hay un condicional que permite no aplicarlo en caso de que el total no sea suficiente

#¿Qué pasa si el carrito viene vacío? ¿Y si el mismo SKU aparece dos veces en el array?
el ciclo for recorre el carrito, si viene vacio no va a ocurrir nada

¿Cómo garantizas que la validación de stock sea atómica: o todo pasa o nada se procesa?
un condiconal permite comparar stock con cantidad para verificar si es posible contintinuar, en caso de que no, muestra un error
