# O que é Docker

Podemos utilizar o logo do Docker para fazermos uma analogia e facilitar o entendimento da ferramenta, assim fica mais fácil de descobrir o real objetivo da mesma.

![Image of Docker](/images/docker-logo.jpg "Docker Logo")

### Docker Engine

Análogamente a `baleia` seria uma pré-configuração ou a base de um ambiente de desenvolvimento que você pode levar para qualquer projeto e é conhecido também como `Docker Engine`.

 Isso significar que todos os membros da equipe teriam o mesmo padrão e os mesmos recursos, facilitando assim o desenvolvimento e evitando erros de diferentes sistemas operacionais.

### Containers

As `caixas` ou `container` em cima da `baleia` seriam fragmentos ou instâncias necessários para o desenvolvimento do projeto.

**Exemplos**

1. Mysql
2. Apache/Nginx
3. PHP-FPM
4. Redis
5. ELASTICSEARCH

Estes containers rodam de forma isolada, mas podem ter uma comunicação entre eles.

O mais interessante é que estes containers possuem **somente** o necessário para serem rodados. Em outras palavras somentes pedaços de códigos extremamente necessários para o funcionamento correto dos mesmos.

Vale a pena ressaltar que não existe um limite de containers para serem adicionados em sua `Docker Engine`, pois, como não tem um sistema operacional rodando junto com eles, os containers se tornam muito leves e esta é, sem dúvida, a grande vantagem de utilizar a ferramenta para o desenvolvimento do seu projeto.

**__Veja um exemplo abaixo:__**

![Image of Docker Engine Example](/images/docker-engine-example.jpg "Docker Engine Example")

