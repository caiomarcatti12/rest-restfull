# Verbo HTTP **POST**

O verbo POST é usado para criar um novo recurso. Por exemplo, se você fizer uma chamada POST para /users com um corpo de solicitação que contenha os detalhes do usuário a ser criado, isso criaria um novo usuário no sistema.

# Exemplos de aplicação
- Criar um novo usuário: Você pode fazer uma chamada POST para /users com um corpo de solicitação que contenha os detalhes do usuário a ser criado para criar um novo usuário no sistema.

- Criar um novo produto: Você pode fazer uma chamada POST para /products com um corpo de solicitação que contenha os detalhes do produto a ser criado para criar um novo produto no sistema.

- Enviar dados de formulário: Você pode fazer uma chamada POST para um endpoint de processamento de formulário com um corpo de solicitação que contenha os dados do formulário para enviar os dados para o servidor.

- Fazer login em uma conta: Você pode fazer uma chamada POST para /login com um corpo de solicitação que contenha o nome de usuário e a senha para fazer login em uma conta.

- Realizar uma busca: Você pode fazer uma chamada POST para /search com um corpo de solicitação que contenha os critérios de busca para realizar uma busca no sistema.
  
# Exemplos de uso

O formato de uma solicitação HTTP para o verbo POST depende da API que está sendo usada e do formato de dados que ela espera receber. Em geral, uma solicitação POST inclui a URL da API, o corpo da solicitação e um conjunto opcional de cabeçalhos HTTP.

Aqui está um exemplo de uma solicitação POST básica:

```
POST /users HTTP/1.1
Host: example.com
Content-Type: application/json

{
  "name": "John Smith",
  "email": "john@example.com",
  "age": 30
}
```

Neste exemplo, a solicitação POST está enviando os dados de um novo usuário para a API em example.com para criar um novo usuário no sistema. O corpo da solicitação está no formato JSON e inclui os detalhes do usuário.

O verbo POST também pode ser usado com parâmetros de consulta na URL para fornecer informações adicionais sobre a solicitação. Aqui está um exemplo de uma solicitação POST com parâmetros de consulta:

```
POST /users?action=create HTTP/1.1
Host: example.com
Content-Type: application/json

{
  "name": "John Smith",
  "email": "john@example.com",
  "age": 30
}
```

Neste exemplo, a solicitação POST está enviando os dados de um novo usuário para a API em example.com e inclui um parâmetro de consulta "action=create" para indicar que o usuário deve ser criado.