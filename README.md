✍ Esse é um projeto para o conteúdo de `React Testing Library`.

### Antes de iniciar

- Crie um fork desse projeto. Para isso, siga esse [tutorial de como realizar um fork](https://guides.github.com/activities/forking/).

- Após fazer o fork, clone o repositório criado no seu computador.

- Rode o `npm install`.

- Vá para a branch master do seu projeto e execute o comando`git branch`

- Mude para a branch  digimon-finders com o comando git checkout -b digimon-finders. É nessa branch que você realizará a solução para o exercício.

- Observe o que deve ser feito nas instruções.

- Após a solução dos exercícios, abra um PR no seu repositório forkado e, se quiser, mergeie para a master.

⚠ **Atenção!** Quando for criar o PR você se deparará com a seguinte tela:

![PR do exercício](images/example-pr.png)

- É necessário realizar uma mudança. Clique no *base repository* como na imagem abaixo:

![Mudando a base do repositório](images/change-base.png)

- Mude para o seu repositório. Seu nome estará na frente do nome dele, por exemplo: `antonio/comprehension-exercises`. Depois desse passo a página deve ficar assim:

![Após mudança](images/after-change.png)

- Agora basta criar o PULL REQUEST clicando no botão `Create Pull Request`.

➡ Para cada PR realize esse mesmo processo.


### COMEÇANDO OS EXERCÍCIOS

Este repositório contém uma aplicação funcional, que utiliza a [Digimon API](https://digimon-api.vercel.app/) e pesquisa digimons pelo nome.

Seu objetivo nesse exercício é utilizar todos os aprendizados sobre testes para alcançar 100% de cobertura de testes. 

> 👀 **De olho na dica:** você pode verificar a cobertura de testes utilizando o comando `npm run test-coverage`, que te retornará um relatório parecido com o que é mostrado abaixo:

![Após mudança](images/relatorio.png)

- A seta azul mostra o local que deve estar com o valor de 100, o que indica a finalização do exercício com todas as linhas do código testadas.

- Para implementar os seus testes, edite os arquivos `App.test.js` e `Digimon.test.js`, que se encontram dentro da pasta src na raiz do projeto.

- Ler, entender a aplicação e saber o que testar também é parte do exercício. 

- Atente-se aos logs que são recebidos ao rodar os testes! Logo abaixo há mais instruções de como saber o que está sendo testado ou não.

### INSTRUÇÕES

* Ao rodar o comando `npm run test-coverage`, será gerada uma nova pasta na raiz do seu projeto chamada `coverage`. Após criar a pasta, abra o arquivo `./coverage/lcov-report/index.html` usando a extensão `Live Server` do seu VSCode:

![Resumo Coverage](images/coverage-resume.png)

* Clique no link do arquivo `./coverage/lcov-report/index.html` e veja os detalhes sobre o que está sendo avaliado na cobertura de testes:

![Coverage Detail](images/coverage-detail.png)

* Utilize essa lista como referência para programar seus testes. Cubra todos as linhas destacadas para ter 100% de cobertura!

### TESTANDO OS TESTES

"Testar testes" pode parecer um conceito estranho, mas existem técnicas bastante engenhosas para isso. A técnica que vamos usar aqui no exercício baseia-se em inserir vários bugs nos arquivos do projeto e verificar se os testes que você programou continuam rodando ou apontando as falhas. Caso os testes não percebam os bugs, significa que estão acusando falsos positivos (ou negativos também).

Esses bugs são chamados de "mutantes", e a nossa missão aqui é eliminá-los! Você pode até pensar nisso como um joguinho, e para que possamos fazer tudo de forma controlada, vamos utilizar uma library chamada [Stryker](https://stryker-mutator.io/).

O Stryker vai gerar os mutantes automaticamente de acordo com a configuração passada pra ele, geralmente em um arquivo `JS`, podendo também ser num `JSON`. Se você acessar a raiz do nosso exercício, encontrará o arquivo `stryker.conf.js`. Abra-o e dê uma espiada! Se você tiver curiosidade sobre como funcionam as configurações, poderá acessar seu repositório e ler o [README](https://github.com/stryker-mutator/stryker/tree/master/packages/core#readme).

### Como usar o Stryker?

Usar o Stryker é fácil: basta rodar o comando `npx stryker run` nos projetos que têm ele configurado. Você pode também instalá-lo de forma global usando o comando `npm install -g stryker-cli`.

---

**Divirta-se codando!** 🚀
