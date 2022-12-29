# Verbo HTTP **GET**

O verbo GET é usado para solicitar a leitura de um recurso. Por exemplo, se você fizer uma chamada GET para /users/123, isso solicitaria a leitura do usuário com o ID 123.

# Existe um padrão?
Não existe um padrão de URL específico para o verbo GET, mas existem algumas convenções comuns que são usadas em APIs RESTful.

Geralmente, o verbo GET é usado para solicitar a leitura de um recurso específico ou de uma lista de recursos. Por exemplo, uma chamada GET para /users solicitaria a leitura de uma lista de usuários, enquanto uma chamada GET para /users/123 solicitaria a leitura do usuário com o ID 123.

Além disso, o verbo GET pode ser usado com parâmetros de consulta na URL para filtrar ou classificar os resultados da solicitação. Por exemplo, você pode usar um parâmetro de consulta como ?sort=name para classificar a lista de usuários por nome ou um parâmetro de consulta como ?category=electronics para filtrar a lista de produtos por categoria.

# Exemplos de aplicação
- Obter uma lista de usuários: Você pode fazer uma chamada GET para /users para obter uma lista de todos os usuários no sistema.

- Obter detalhes de um usuário específico: Você pode fazer uma chamada GET para /users/123 para obter os detalhes do usuário com o ID 123.

- Obter uma lista de produtos de uma determinada categoria: Você pode fazer uma chamada GET para /products?category=electronics para obter uma lista de produtos na categoria de eletrônicos.

- Obter um arquivo de imagem: Você pode fazer uma chamada GET para /images/logo.png para obter o arquivo de imagem logo.png.

- Obter um relatório de vendas: Você pode fazer uma chamada GET para /sales_report?start_date=2022-01-01&end_date=2022-01-31 para obter um relatório de vendas para o mês de janeiro de 2022.

# Exemplos de uso

O formato de uma solicitação HTTP para o verbo GET depende da API que está sendo usada e do formato de dados que ela espera receber. Em geral, uma solicitação GET inclui a URL da API e um conjunto opcional de parâmetros de consulta na URL.

Aqui está um exemplo de uma solicitação GET básica:

```
GET /users HTTP/1.1
Host: example.com
```

Neste exemplo, a solicitação GET está solicitando a leitura de uma lista de usuários na API em example.com.

O verbo GET também pode ser usado com parâmetros de consulta na URL para filtrar ou classificar os resultados da solicitação. Aqui está um exemplo de uma solicitação GET com parâmetros de consulta:

```
GET /users?sort=name&age=30 HTTP/1.1
Host: example.com
```
Neste exemplo, a solicitação GET está solicitando a leitura de uma lista de usuários que tenham 30 anos e que estejam classificados por nome.

Além disso, é possível adicionar cabeçalhos HTTP à solicitação GET para fornecer informações adicionais sobre a solicitação. Por exemplo, você pode adicionar um cabeçalho "Accept" para especificar o formato de dados que você deseja receber na resposta.

Esses são apenas alguns exemplos de como uma solicitação GET pode ser formatada. É importante lembrar que cada API é diferente e pode ter suas próprias convenções de URL e cabeçalhos HTTP.