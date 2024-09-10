# O que é uma API Rest

Uma API REST (ou API RESTful) é um estilo de arquitetura de API que segue uma série de convenções para criar APIs da web que são compatíveis com o protocolo HTTP. Essas APIs são projetadas para serem flexíveis, escaláveis e independentes de plataforma, o que as torna uma opção popular para a integração de sistemas em aplicativos da web e dispositivos móveis.

Uma API REST é baseada em uma arquitetura de cliente-servidor, onde o cliente faz uma solicitação ao servidor através de uma chamada de API. O servidor, por sua vez, retorna uma resposta ao cliente na forma de um conjunto de dados, geralmente no formato JSON (JavaScript Object Notation). As APIs REST são projetadas para serem fáceis de usar e acessíveis a qualquer dispositivo que possa fazer chamadas HTTP.

Uma API REST segue um conjunto de convenções conhecidas como o "Estilo arquitetural REST", que inclui o uso de recursos HTTP como métodos GET, POST, PUT e DELETE para realizar operações de leitura, criação, atualização e exclusão em um sistema. Além disso, uma API REST deve ser projetada de forma a ser independente da plataforma, o que significa que ela pode ser acessada e consumida por qualquer dispositivo ou aplicativo que possa fazer chamadas HTTP.


# Rest ou RestFull?

A palavra "REST" é a abreviação de "Representational State Transfer", que é um estilo arquitetural para projetar APIs da web. Esse estilo arquitetural foi proposto pelo cientista da computação Roy Fielding em sua tese de doutorado em 2000. Ele define uma série de convenções para criar APIs que são compatíveis com o protocolo HTTP e que seguem uma arquitetura de cliente-servidor.

Já a palavra "RESTful" é um adjetivo que descreve uma API que segue o estilo arquitetural REST. Portanto, uma API RESTful é uma API que segue o estilo arquitetural REST. Em resumo, REST é o estilo arquitetural e RESTful é um adjetivo para descrever uma API que segue esse estilo arquitetural.

Em geral, as APIs RESTful são consideradas uma boa opção para a integração de sistemas, pois são flexíveis, escaláveis e independentes de plataforma. Elas também são fáceis de usar e acessíveis a qualquer dispositivo que possa fazer chamadas HTTP, o que as torna uma opção popular para aplicativos da web e dispositivos móveis.


# Explicando alguns verbos HTTP

- [GET](./01-get.md)
- [POST](./02-post.md) 
- [PUT](./03-put.md) 
- [DELETE](./04-delete.md) 
- [HEAD](./05-head.md) 
- [PATCH](./06-patch.md) 
- [IF-MATCH](./08-if-match.md) 
  
Essas são apenas algumas das convenções comuns para o uso do verbo GET em APIs RESTful. É importante lembrar que cada API é diferente e pode ter suas próprias convenções de URL e parâmetros de consulta.

- [Diferenças entre PATCH, PUT, POST](./07-diference-patch-put-post.md)
  
# Cabeçalhos HTTP
  
Os cabeçalhos HTTP são parte de uma solicitação ou resposta HTTP e fornecem informações adicionais sobre a solicitação ou resposta. Eles são enviados entre o cliente e o servidor como parte da mensagem HTTP e podem ser usados para fornecer informações sobre o cliente, o servidor, o tipo de conteúdo da mensagem e muito mais.

- [Explicando alguns HTTP Headers](./09-headers-http.md) 

# Códigos HTTP
  
Os códigos de resposta HTTP são números que são enviados pelo servidor como parte de uma resposta HTTP para indicar o status da solicitação. Eles informam ao cliente se a solicitação foi bem-sucedida, se houve um erro ou se houve algum outro tipo de resposta.

- [Explicando alguns HTTP Codes](./10-codes-http.md) 