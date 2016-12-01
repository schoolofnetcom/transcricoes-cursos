# Hello Word e comando Básicos

Não é nosso objetivo sair criando um módulo só com os mais diversos comandos do Docker, porque ficaria massante e talvez vocês não entendessem ou guardassem o que é mais importante.

Portando vamos apresentando os comandos principais e explicando para que nosso conteúdo seja mais aproveitado e assimilado por todos. Acreditamos ser melhor desta forma porque iremos utilizar dois recursos super importantes durante o curso que são:

1. Docker File
2. Docker Compose

Para entendermos a ideia e o objetivo destes arquivos precisamos entender como funcionam os containers do Docker, como subimos um novo container entre outros comandos.

Portanto durante nosso processo com o Docker, neste curso, vocês irão entender as ideias básicas e os comandos principais que iremos utilizar.

***

# Iniciando com Docker

Após feita a instalação e ter rodado o terminal para iniciar o Docker, já podemos começar com os primeiros comandos.

No terminal digite `$ docker` e já terá uma lista de comandos disponíveis. São tantos os comandos que talvez ninguém saiba todos, mas temos esta facilidade de consultar a hora que quisermos.

Portanto iremos lhe passar o necessário para que possa trabalhar com o Docker no seu dia-a-dia de desenvolvimento tranquilamente.

Próximo comando que sugerimos na sequência seria o `$ docker version` que trará os seguintes dados:

![Docker Version](./images/docker-version-command.png "Docker Version Command")

Se analisarmos a imagem acima veremos que possuem duas informações importantes para `$ docker version`.

1. Client
2. Server

**Client:** São os dados de onde estamos rodando os comandos

**Server:** São os dados de onde o Docker irá acessar a **_Docker Engine_** , os **_containers_** e de onde vai rodar todas as aplicações.

***

Um comando bem comum para iniciarmos também e que serve como teste para ver se o nosso Docker está rodando certinho é o `$ docker run hello-world`.

Este comando solicita que o Docker rode a **imagem hello-world**. Em breve falaremos mais sobre _imagens_, mas já adiantando **imagem** é como se fosse um **snapshot** de uma aplicação, máquina ou configurações. E no caso deste comando será realmente um Hello World somente para testar nosso Docker.

![Docker Hello World](./images/docker-hello-world.png "Hello World")

Quando rodamos este comando o Docker da uma mensagem de que não foi possível encontrar a **imagem** localmente, mas ele faz um **download** e nos mostra a mensagem acima no terminal. Após isso sabemos que está tudo ok com nosso Docker e já fizemos a nossa primeira impressão.

Caso rode novamente o mesmo comando o Docker nos mostrará diretamente a imagem **Hello World** porque já foi baixada anteriormente e agora ele encontra ela localmente.

Caso queira saber quais imagens você já possui localmente basta rodas o comando `$ docker imagens` e terá o seguinte resultado:

![Docker Images](./images/docker-images.png "Docker Imagens")