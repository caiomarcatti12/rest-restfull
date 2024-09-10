# Patch, Put, Post... parece tudo igual mas não é!
Aqui estão algumas diferenças entre os verbos HTTP PATCH, PUT e POST:

Objetivo: O verbo PATCH é usado para aplicar modificações parciais a um recurso existente no sistema. O verbo PUT é usado para substituir um recurso inteiro no sistema. O verbo POST é usado para criar um novo recurso no sistema ou enviar uma solicitação que resulte em uma ação no sistema, como enviar um formulário ou iniciar um processo.

Modificação do recurso: O verbo PATCH é usado para fazer modificações parciais em um recurso existente. O verbo PUT é usado para substituir completamente um recurso existente. O verbo POST não modifica um recurso existente, mas cria um novo recurso no sistema.

Idempotência: Os verbos PUT e DELETE são considerados idempotentes, o que significa que se você fizer a mesma chamada várias vezes, o resultado será o mesmo. O verbo PATCH não é idempotente, pois as modificações parciais que ele aplica podem ser acumulativas. O verbo POST também não é idempotente, pois cria um novo recurso a cada vez que é chamado.

Formato de solicitação: O verbo PUT geralmente exige que o corpo da solicitação contenha os novos dados do recurso, enquanto o verbo POST pode enviar dados no corpo da solicitação ou como parâmetros de consulta. O verbo PATCH pode enviar os dados de modificação no corpo da solicitação ou como parâmetros de consulta.

Segurança: O verbo PUT geralmente exige autenticação ou autorização