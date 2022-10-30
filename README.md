# Modelagem BD E-commerce.
- Modelagem de banco de dados relacional para sistema ecommerce com possibilidade de vendedores externos, em sistema de marketplace
- Entidades identificadas com atributos básicos suficientes para sua caracterização.
- Pelas características do sistema de marketplace, o estoque de produtos a ele associados não será persistido.
- A entidade vendedores refere-se aos vendedores parceiros, do sistema de marketplace.

## Cliente
A entidade mais importante é cliente, que poderá ser Pessoa Física (PF) ou Pessoa Jurídica (PJ). Está relacionada à entidade pedido, que possui um ou mais itens (produtos).

## Produto
Estes produtos, quando entregues pela própria ecommerce, tem associados a eles um ou mais fornecedores, além de estarem também associados a um ou mais fornecedores.

## Estoque
O estoque físico dos produtos entregues pela própria ecommerce é representado pela entidade centro de distribuição, a partir dos quais a entrega será realizada a entrega.

## Marketplace
Um produto também poderá ser entregue por vendedor parceiro (marketplace). Nesse caso, o estoque não será persistido, ficando esses dados a cargo de cada vendedor.

## Entrega
Dada a importância estratégica, optou-se por persistir os dados de entrega em uma entidade própria.
