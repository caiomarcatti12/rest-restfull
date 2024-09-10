# Códigos de resposta HTTP

Os códigos de resposta HTTP são códigos numéricos que são retornados pelo servidor como parte de uma resposta HTTP para indicar o resultado da solicitação do cliente. Eles são usados para informar ao cliente se a solicitação foi bem-sucedida, se ocorreu algum erro ou se outra ação é necessária.

Os códigos de resposta HTTP são divididos em cinco classes: informativo (1xx), sucesso (2xx), redirecionamento (3xx), erro de cliente (4xx) e erro de servidor (5xx). Cada classe de código de resposta inclui uma série de códigos específicos que fornecem mais informações sobre o resultado da solicitação.

Alguns exemplos comuns de códigos de resposta HTTP incluem:

- 200 OK: indica que a solicitação foi bem-sucedida e que a resposta inclui o conteúdo solicitado.
- 301 Moved Permanently: indica que o recurso solicitado foi movido para um novo endereço permanentemente. O cabeçalho "Location" na resposta fornece o novo endereço do recurso.
- 401 Unauthorized: indica que o cliente precisa se autenticar com o servidor para acessar o recurso solicitado.
- 404 Not Found: indica que o recurso solicitado não foi encontrado no servidor.
- 500 Internal Server Error: indica que o servidor encontrou um erro ao tentar processar a solicitação.

# Tabela de códigos HTTP

<table>
<tr><td>(Status-code)</td><td>Significado do código HTTP</td><td>(Reason-Phrase)	Significado do código HTTP</td></tr>
<tr><td>100</td><td>Continue</td><td>Continuar</td></tr>
<tr><td>101</td><td>Switching Protocols</td><td>Mudando Protocolos</td></tr>
<tr><td>102</td><td>Processing</td><td>Processando</td></tr>
<tr><td>200</td><td>Ok</td><td>Ok</td></tr>
<tr><td>201</td><td>Created</td><td>Criado</td></tr>
<tr><td>202</td><td>Accepted</td><td>Aceito</td></tr>
<tr><td>203</td><td>Non-Authoritative Information</td><td>Não autorizado</td></tr>
<tr><td>204</td><td>No Content</td><td>Nenhum Conteúdo</td></tr>
<tr><td>205</td><td>Reset Content</td><td>Resetar Conteúdo</td></tr>
<tr><td>206</td><td>Partial Content</td><td>Conteúdo Parcial</td></tr>
<tr><td>300</td><td>Multiple Choices</td><td>Múltipla Escolha</td></tr>
<tr><td>301</td><td>Moved Permanently</td><td>Movido Permanentemente</td></tr>
<tr><td>302</td><td>Found</td><td>Encontrado</td></tr>
<tr><td>303</td><td>See Other</td><td>Veja outro</td></tr>
<tr><td>304</td><td>Not Modified</td><td>Não modificado</td></tr>
<tr><td>305</td><td>Use Proxy</td><td>Use Proxy</td></tr>
<tr><td>306</td><td>Proxy Switch</td><td>Proxy Trocado</td></tr>
<tr><td>400</td><td>Bad Request</td><td>Solicitação Inválida</td></tr>
<tr><td>401</td><td>Unauthorized</td><td>Não autorizado</td></tr>
<tr><td>402</td><td>Payment Required</td><td>Pagamento necessário</td></tr>
<tr><td>403</td><td>Forbidden</td><td>Proibido</td></tr>
<tr><td>404</td><td>Not Found</td><td>Não encontrado</td></tr>
<tr><td>405</td><td>Method Not Allowed</td><td>Método não permitido</td></tr>
<tr><td>406</td><td>Not Acceptable</td><td>Não aceito</td></tr>
<tr><td>407</td><td>Proxy Authentication Required</td><td>Autenticação de Proxy Necessária</td></tr>
<tr><td>408</td><td>Request Time-out</td><td>Tempo de solicitação esgotado</td></tr>
<tr><td>409</td><td>Conflict</td><td>Conflito</td></tr>
<tr><td>410</td><td>Gone</td><td>Perdido</td></tr>
<tr><td>411</td><td>Length Required</td><td>Duração necessária</td></tr>
<tr><td>412</td><td>Precondition Failed</td><td>Falha de pré-condição</td></tr>
<tr><td>413</td><td>Request Entity Too Large</td><td>Solicitação da entidade muito extensa</td></tr>
<tr><td>414</td><td>Request-URL Too Large</td><td>Solicitação de URL muito Longa</td></tr>
<tr><td>415</td><td>Unsupported Media Type</td><td>Tipo de mídia não suportado</td></tr>
<tr><td>416</td><td>Request Range Not Satisfiable</td><td>Solicitação de faixa não satisfatória</td></tr>
<tr><td>417</td><td>Expectation Failed</td><td>Falha na expectativa</td></tr>
<tr><td>500</td><td>Internal Server Error</td><td>Erro do Servidor Interno</td></tr>
<tr><td>501</td><td>Not Implemented</td><td>Não implementado</td></tr>
<tr><td>502</td><td>Bad Gateway</td><td>Porta de entrada ruim</td></tr>
<tr><td>503</td><td>Service Unavailable</td><td>Serviço Indisponível</td></tr>
<tr><td>504</td><td>Gateway Time-out</td><td>Tempo limite da Porta de Entrada</td></tr>
<tr><td>505</td><td>HTTP Version Not Supported</td><td>Versão HTTP não suportada</td></tr>
</table>