# Verbo HTTP **PATCH**
O verbo PATCH é comumente usado para atualizar parcialmente um recurso existente no sistema, ao invés de substituí-lo completamente como o verbo PUT.

# Existe um padrão?

# Exemplos de aplicação

- Atualizar os detalhes de um usuário específico: Você pode fazer uma chamada PATCH para /users/123 com um corpo de solicitação que contenha os novos detalhes do usuário para atualizar o usuário com o ID 123.

- Atualizar o nome de um produto: Você pode fazer uma chamada PATCH para /products/456 com um corpo de solicitação que contenha o novo nome do produto para atualizar o produto com o ID 456.

- Atualizar o status de uma tarefa: Você pode fazer uma chamada PATCH para /tasks/789 com um corpo de solicitação que contenha o novo status da tarefa para atualizar a tarefa com o ID 789.

- Atualizar a imagem de perfil de um usuário: Você pode fazer uma chamada PATCH para /users/123/profile_image com um corpo de solicitação que contenha a nova imagem de perfil para atualizar a imagem de perfil do usuário com o ID 123.

- Atualizar o preço de um produto: Você pode fazer uma chamada PATCH para /products/456/price com um corpo de solicitação que contenha o novo preço do produto para atualizar o preço do produto com o ID 456.

# Exemplos de uso

O formato de uma solicitação HTTP para o verbo PATCH depende da API que está sendo usada e do formato de dados que ela espera receber. Em geral, uma solicitação PATCH inclui a URL da API, o corpo da solicitação e um conjunto opcional de cabeçalhos HTTP.

Aqui está um exemplo de uma solicitação PATCH básica:

```
PATCH /users/123 HTTP/1.1
Host: example.com
Content-Type: application/json

{
  "name": "John Smith",
  "email": "john@example.com",
  "age": 30
}
```
Neste exemplo, a solicitação PATCH está enviando os novos dados de um usuário para a API em example.com para atualizar o usuário com o ID 123. O corpo da solicitação está no formato JSON e inclui os novos detalhes do usuário.

O verbo PATCH também pode ser usado com parâmetros de consulta na URL para fornecer informações adicionais sobre a solicitação. Aqui está um exemplo de uma solicitação PATCH com parâmetros de consulta:

```
PATCH /users/123?action=update HTTP/1.1
Host: example.com
Content-Type: application/json

{
  "name": "John Smith",
  "email": "john@example.com",
  "age": 30
}
```

Neste exemplo, a solicitação PATCH está enviando os novos dados de um usuário para a API em example.com para atualizar o usuário com o ID 123 e inclui um parâmetro de consulta "action=update" para indicar que a atualização deve ser aplicada.

Além disso, é possível adicionar cabeçalhos HTTP à solicitação PATCH para fornecer informações adicionais sobre a solicitação. Por exemplo, você pode adicionar um cabeçalho "Authorization" para fornecer informações de autenticação ou um cabeçalho "If-Match" para garantir que o recurso só seja atualizado se tiver sido modificado desde a última vez que foi lido.
