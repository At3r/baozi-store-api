# Baozi Store — API REST

Projeto acadêmico de API REST com Java, Spring Boot, Spring Data JPA e MySQL.

## Configuração
1. Crie o banco `baozi_store` no MySQL (ou mantenha `createDatabaseIfNotExist=true` na URL).
2. Edite `src/main/resources/application.properties` e substitua `COLOQUE_SUA_SENHA_AQUI` pela senha local do MySQL.
3. No Eclipse, clique com o botão direito no projeto > Maven > Update Project.
4. Execute `BaoziStoreApplication.java` como Spring Boot App ou Java Application.

## Endpoints
| Método | Caminho | Ação |
|---|---|---|
| POST | /clientes | Criar cliente |
| GET | /clientes | Listar clientes |
| GET | /clientes/{id} | Consultar cliente |
| DELETE | /clientes/{id} | Excluir cliente |
| POST | /produtos | Criar produto |
| GET | /produtos | Listar produtos |
| GET | /produtos/{id} | Consultar produto |
| DELETE | /produtos/{id} | Excluir produto |
| POST | /pedidos | Criar pedido |
| GET | /pedidos | Listar pedidos |
| GET | /pedidos/{id} | Consultar pedido |
| DELETE | /pedidos/{id} | Excluir pedido |

Base URL local: http://localhost:8080

## Exemplos JSON

Cliente:
{"nome":"SeuNomeSEUR U","clienteDesde":"2026-11-25"}

Produto:
{"nome":"Baozi tradicional","preco":8.50,"estoque":true}

Pedido (use IDs existentes):
{"clienteId":1,"produtoId":1,"quantidade":3}

Observação: substitua o nome de exemplo do cliente pelo seu nome seguido do RU, conforme solicitado na atividade. Faça os testes e capturas reais no Postman; o código não gera esses prints automaticamente.
