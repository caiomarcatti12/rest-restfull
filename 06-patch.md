Atualização Parcial de Recursos com PATCH

## Introdução

No contexto de uma API RESTful, o método **PATCH** é comumente usado para atualizar parcialmente um recurso existente no sistema, ao invés de substituí-lo completamente como o método **PUT**.

Essa abordagem permite maior eficiência, pois somente os campos necessários são enviados, evitando redundâncias. Nesta documentação, serão apresentados conceitos gerais, exemplos de aplicação e boas práticas para o uso do verbo **PATCH**.

---

## Existe um Padrão?

Sim, o uso do verbo **PATCH** segue as diretrizes do protocolo HTTP. No entanto, a implementação exata pode variar dependendo do design da API. É importante manter consistência e seguir padrões estabelecidos, como o uso de payloads JSON e cabeçalhos adequados.

---

## Exemplos de Aplicação

1. **Atualizar os detalhes de um usuário específico:**

   ```http
   PATCH /users/123 HTTP/1.1
   Host: example.com
   Content-Type: application/json

   {
     "name": "John Smith",
     "email": "john@example.com"
   }
   ```

   Essa requisição atualiza apenas os campos fornecidos no corpo, como nome e email, do usuário com ID 123.

2. **Atualizar o status de uma tarefa:**

   ```http
   PATCH /tasks/789 HTTP/1.1
   Host: example.com
   Content-Type: application/json

   {
     "status": "completed"
   }
   ```

   Apenas o campo `status` é modificado na tarefa identificada pelo ID 789.

3. **Atualizar o preço de um produto:**

   ```http
   PATCH /products/456/price HTTP/1.1
   Host: example.com
   Content-Type: application/json

   {
     "price": 99.99
   }
   ```

   Essa chamada atualiza somente o preço do produto com ID 456.

**Nota: Apenas os campos que precisam de atualização devem ser incluídos no payload.**

---

## Resposta de Sucesso

#### Código de Status:

```
200 OK
```

#### Corpo da Resposta:

Caso a mensagem seja dinâmica:

```json
{
  "message": "Recurso 123atualizado com sucesso"
}
```

Se nenhuma mensagem dinamica for necessária, a resposta pode ser vazia:

```json
{}
```

---

## Diferença entre PUT e PATCH

- **PUT:**

    - Substitui completamente o recurso.
    - Todos os campos precisam ser enviados.
    - Útil para atualizações completas.

- **PATCH:**

    - Atualiza apenas os campos fornecidos.
    - Reduz o tamanho da requisição.
    - Mais eficiente para alterações parciais.

Exemplo com PUT:

```http
PUT /users/123 HTTP/1.1
Host: example.com
Content-Type: application/json

{
  "id": 123,
  "name": "John Smith",
  "email": "john@example.com",
  "age": 30
}
```

Exemplo com PATCH (Mais Eficiente):

```http
PATCH /users/123 HTTP/1.1
Host: example.com
Content-Type: application/json

{
  "name": "John Smith"
}
```

---

## Considerações Finais

- Prefira o uso de **PATCH** para atualizações parciais de recursos.
- Certifique-se de validar as requisições para evitar alterações indevidas ou inconsistentes.
- Utilize respostas claras para indicar o sucesso ou a falha da operação.

Essa abordagem melhora a eficiência e segue as boas práticas de design de APIs RESTful.