# BDO-pizzaria

## Estrutura do Banco de Dados

- **Tabela Pizzas**: Contém informações sobre as pizzas disponíveis, como nome e preço.
- **Tabela Sabores**: Registra os sabores disponíveis para cada pizza.
- **Tabela Pedidos**: Armazena os pedidos dos clientes, incluindo o status e data de criação.
- **Tabela Status**: Gerencia os diferentes status dos pedidos (Preparando, Em Entrega, Concluído).
- **Tabela Tamanho**: Registra os diferentes tamanhos disponíveis para as pizzas (ex: Pequena, Média, Grande). Essa tabela é usada para associar os tamanhos às pizzas, permitindo uma maior personalização no pedido.

- **Para reiniciar o banco de dados e começar com ID novo**:
SET FOREIGN_KEY_CHECKS = 0;
TRUNCATE TABLE pizzas;
TRUNCATE TABLE pizza_sabor;
TRUNCATE TABLE pedidos;
SET FOREIGN_KEY_CHECKS = 1;
