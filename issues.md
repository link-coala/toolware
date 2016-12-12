---
layout: page
title: Problemas
permalink: /problemas/
---
1.el formulario para crear ordenes solo las crea con el atributo de la direcion hace falta el campo de texto donde
se agregan los productos

1.1. este formulario como involucra dos modelos tiene que habilitar para aceptar nested atributes desde el otro modelo
por que como esta solo se involucra con el modelo order hace falta que este formulario acepte atributos desde line_item y
product 

1.2 como alternativa para aproximarse al wireframe provsionalmente se utilisara el helper collection_select que produce
un campo de seleccion con los registros en la tabla products

1.3 line item tiene tres atributos quantity, product_id, order_id aqui se crean dos mantequillas obteniendo el id de la variable butter

butter = Product.create(name: 'Butter (250 gr)', price: 0.75)

order.line_items.create(product_id: butter.id, quantity: 2)

