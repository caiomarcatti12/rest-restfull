# If-Match, o que é isso?

O cabeçalho HTTP If-Match é um cabeçalho opcional que pode ser incluído em uma solicitação HTTP para garantir que o recurso só seja modificado se tiver sido modificado desde a última vez que foi lido. Ele é usado principalmente com os verbos HTTP PUT e PATCH para evitar conflitos de atualização entre diferentes clientes que estejam tentando modificar o mesmo recurso ao mesmo tempo.

Quando um cliente faz uma solicitação HTTP que inclui o cabeçalho If-Match, a API verifica se o valor especificado no cabeçalho corresponde ao valor atual do cabeçalho ETag do recurso. Se os valores corresponderem, a API sabe que o recurso não foi modificado desde a última vez que foi lido pelo cliente e, portanto, pode prosseguir com a modificação. Se os valores não corresponderem, a API retorna um erro de condição de correspondência e não aplica a modificação.

O valor do cabeçalho If-Match é geralmente um valor de etiqueta de entidade (ETag) gerado pelo servidor para cada recurso. O ETag é um valor único que representa a versão atual do recurso e é usado para gerenciar a integridade de cache e conflitos de atualização.

Aqui está um exemplo de como o cabeçalho If-Match pode ser usado em uma solicitação PUT:

```
PUT /users/123 HTTP/1.1
Host: example.com
Content-Type: application/json
If-Match: "abc123"

{
  "name": "John Smith",
  "email": "john@example.com",
  "age": 30
}
```

Neste exemplo, a solicitação PUT está enviando os novos dados de um usuário para a API em example.com para substituir o usuário com o ID 123. O cabeçalho If-Match inclui o valor "abc123", que é comparado com o valor atual do cabeçalho ETag do recurso para garantir que o recurso só seja modificado se tiver sido modificado desde a última vez que foi lido.


# Mas de onde vem o ETag?

O valor do cabeçalho If-Match é geralmente gerado pelo servidor como uma etiqueta de entidade (ETag) para cada recurso. O ETag é um valor único que representa a versão atual do recurso e é usado para gerenciar a integridade de cache e conflitos de atualização.

Para gerar um valor de ETag, o servidor pode calcular um resumo criptográfico do conteúdo do recurso (por exemplo, usando um algoritmo como o hash SHA-1). O ETag também pode ser gerado usando outros mecanismos, como o timestamp da última modificação do recurso ou um valor de contador incremental.

O valor do ETag é armazenado pelo servidor e incluído no cabeçalho HTTP ETag da resposta a cada solicitação de leitura do recurso. Quando um cliente faz uma solicitação de atualização do recurso usando o verbo PUT ou PATCH, ele inclui o cabeçalho If-Match com o valor do ETag atualmente armazenado pelo servidor. A API então verifica se os valores correspondem antes de prosseguir com a atualização do recurso.

Aqui está um exemplo de como o cabeçalho ETag pode ser incluído em uma resposta HTTP:

```
HTTP/1.1 200 OK
Content-Type: application/json
ETag: "abc123"

{
  "name": "John Smith",
  "email": "john@example.com",
  "age": 30
}
```
Neste exemplo, a resposta HTTP inclui o cabeçalho ETag com o valor "abc123", que é gerado pelo servidor como uma etiqueta de entidade para o recurso. Quando um cliente faz uma solicitação de atualização do recurso, ele pode incluir o cabeçalho If-Match com o valor "abc123" para garantir que o recurso só seja modificado se tiver sido modificado desde a última vez que foi lido.


# Como gerar

O valor do cabeçalho If-Match é geralmente gerado pelo servidor da API como um valor de etiqueta de entidade (ETag). O ETag é um valor único que representa a versão atual de um recurso e é usado para gerenciar a integridade de cache e conflitos de atualização.

Existem várias maneiras de gerar um valor de ETag para um recurso. Algumas opções comuns incluem:

- Hash de conteúdo: Um valor de ETag pode ser gerado como um hash do conteúdo do recurso. Isso garante que o ETag mudará sempre que o conteúdo do recurso for modificado.

- Data e hora de modificação: Um valor de ETag pode ser gerado como a data e hora da última modificação do recurso. Isso garante que o ETag mudará sempre que o recurso for modificado.

- Valor aleatório: Um valor de ETag pode ser gerado como um valor aleatório único para cada recurso. Isso garante que o ETag será diferente para cada recurso, mesmo que o conteúdo do recurso seja o mesmo.

- Combinação de valores: Um valor de ETag pode ser gerado como uma combinação de vários valores, como o conteúdo do recurso, a data e hora da última modificação e um valor aleatório.

Como o ETag é gerado depende da implementação da API e das necessidades do sistema. É importante escolher um método que garanta que o valor do ETag será único e atualizado sempre que o recurso for modificado.