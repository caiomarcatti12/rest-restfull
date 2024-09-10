# Verbo HTTP **DELETE**
O verbo DELETE é usado para excluir um recurso. Por exemplo, se você fizer uma chamada DELETE para /users/123, isso excluiria o usuário com o ID 123 do sistema.

# Exemplos de aplicação
- Excluir um usuário específico: Você pode fazer uma chamada DELETE para /users/123 para excluir o usuário com o ID 123.

- Excluir um produto específico: Você pode fazer uma chamada DELETE para /products/456 para excluir o produto com o ID 456.

- Excluir uma tarefa específica: Você pode fazer uma chamada DELETE para /tasks/789 para excluir a tarefa com o ID 789.

- Excluir um arquivo de imagem: Você pode fazer uma chamada DELETE para /images/logo.png para excluir o arquivo de imagem logo.png.

- Excluir uma conta de usuário: Você pode fazer uma chamada DELETE para /account para excluir a conta do usuário atual.

Esses são apenas alguns exemplos de como o verbo DELETE pode ser usado em uma chamada de API. O verbo DELETE é comumente usado para excluir um recurso específico do sistema. É importante lembrar que uma vez que um recurso é excluído, ele geralmente não pode ser recuperado. Portanto, é importante ter cuidado ao usar o verbo DELETE e garantir que você tenha autorização adequada para excluir o recurso desejado.

# Exemplos de uso
O formato de uma solicitação HTTP para o verbo DELETE depende da API que está sendo usada e do formato de dados que ela espera receber. Em geral, uma solicitação DELETE inclui a URL da API e um conjunto opcional de parâmetros de consulta na URL.

Aqui está um exemplo de uma solicitação DELETE básica:

```
DELETE /users/123 HTTP/1.1
Host: example.com
```
Neste exemplo, a solicitação DELETE está solicitando a exclusão do usuário com o ID 123 na API em example.com.

O verbo DELETE também pode ser usado com parâmetros de consulta na URL para fornecer informações adicionais sobre a solicitação. Aqui está um exemplo de uma solicitação DELETE com parâmetros de consulta:

```
DELETE /users/123?force=true HTTP/1.1
Host: example.com
```

Neste exemplo, a solicitação DELETE está solicitando a exclusão do usuário com o ID 123 na API em example.com e inclui um parâmetro de consulta "force=true" para indicar que o usuário deve ser excluído mesmo se houver dependências.