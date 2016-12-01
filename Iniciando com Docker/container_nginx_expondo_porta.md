# Criando Container do Nginx e expondo porta

Na aula passada falamos um pouco sobre alguns comandos básico porém muito importantes para o uso do Docker no dia-a-dia.

Agora, nesta aula, queremos dar um exemplo mais concreto para que consigamos trabalhar com o Docker de uma forma mais produtiva e efetiva. Não queremos utilizar somente uma **imagem** chamada _Hello World_ que não faz nada além de exibir um conteúdo pronto.

### Como saber qual imagem já existe no repositório do Docker para iniciarmos?

Acesse o [Docker Hub](https://hub.docker.com) onde você pode pesquisar pelas mais diversas imagens existentes e também poderá criar uma conta para hospedar suas próprias imagens. Neste site você terá também acesso a todos os detalhes de cada imagem encontrada, mas **atenção** existem imagens **oficiais** e de terceiros.

Leia, com atenção, a especificação de cada imagem antes de rodar no Docker, mas fiquem tranquilos, os tutoriais costumam ser muito bons.

***

# Rodando nosso primeiro Container - Nginx

`$ docker run nginx` Para quem não se lembra este comando irá procurar a imagem **nginx** localmente, se existir ele vai rodar, caso não exista o Docker vai baixar pra gente.

Pra quem está iniciando com Docker vai se deparar com uma situação estranho quando rodar este comando, porque ele vai subir o container e vai **travar** o terminal, mas se abrir um outro terminal e rodar o comando `$ docker ps` irá ver que o nosso container já está funcionando. Outra forma de verificar é digitar `Ctrl + c`para destravar o terminal e ai basta rodar o mesmo comado `$ docker ps` para verificar o funcionamento do nosso container.

Portanto se caso seu terminal travar, não se assuste, isso é normal, porque uma vez que existe uma máquina rodando ele fica exatamente desta forma, como se estivesse travado.

Segue imagem:

![Docker run nginx](./images/docker-run-nginx.png "Docker run nginx")

Verifique que o primeiro terminal ficou travado, mas em um segundo que foi aberto verificamos que o container está rodando normalmente. Esta imagem é só para tranquilizar os iniciantes.

***
Para pararmos o processo de um determinado container basta rodar o comando `$ docker stop ID_DO_CONTAINER` em nosso caso seria `$ docker stop 59c7c4cf06d1`.

![Docker run stop](./images/docker-run-stop.png "Docker run stop")

***

# Rodar container nginx sem travar o terminal

Basta acrescentarmos **-d** ao comando **run**.

**Exemplo:** `$ docker run -d nginx`

Desta forma ele irá rodar nosso container em **background** e eu terei meu terminal livre pra continuar trabalhando. Assim não precisamos abrir outro terminal ou matar o processo no terminal atual.

***

# Acessando Nginx via terminal

O comando `$ docker ps` nos mostra os containers que estão rodando e também as portas disponíveis para acessá-los.

![Docker posts](./images/docker-ports.png "Docker ports")

Se você estiver utilizando o Windows, Mac ou Linux de forma nativa com **HYPER-V**, por exemplo, você não irá precisar descobrir o IP da máquina virtual porque o Docker estará rodando em sua própria máquina então poderá acessar o seu browser diretamente.

Porém como em nosso caso, estamos utilizando uma máquina virtual para rodar o Docker precisaremos descobrir o IP desta máquina virtual para conseguirmos acessar as portas. E existem duas formas para isso:

1. Logo que abrimos o terminal do Docker o IP é mostrado.
2. Podemos rodar o comando `$ docker-machine ls`

![Docker Machine IP](./images/docker-machine-ip.png "Docker Machine IP")









