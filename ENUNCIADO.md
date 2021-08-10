# Desafio - Desenvolvedor Front-end Junior

Este documento apresenta o desafio técnico pelo qual um candidato a desenvolvedor front-end da BRy Tecnologia deve passar durante o processo seletivo.

Os itens em avaliação são divididos em itens fundamentais (cujo não cumprimento implica desqualificação automática) e itens desejáveis (que não são obrigatórios, mas serão observados e pesarão no processo).

Requisitos **fundamentais**:
* Interpretação de texto
* Interpretação de requisitos
* Capacidade de resolução do problema proposto
* Atendimento aos requisitos da aplicação
* Familiaridade com ferramentas de versionamento de código (Git)

Requisitos **desejáveis**:
* Legibilidade de código
* Documentação de código
* Testes unitários
* Familiaridade com ferramentas de desenvolvimento front-end


## Como Realizar o Desafio

1. Se não possuir uma conta no [GitLab](https://gitlab.com), cadastre-se.
2. Informe seu nome de usuário do *GitLab* ao representante da BRy responsável pelo seu processo seletivo, para que sejam dadas permissões para seu usuário.
3. Faça um *fork* do projeto [desafio-frontend-junior](https://gitlab.com/brytecnologia-team/selecao/desafio-frontend-junior) - isso criará um projeto idêntico no seu repositório pessoal.
4. Acesse seu *fork*. Observe que, no diretório raiz do projeto, há um arquivo **ENUNCIADO.md** de conteúdo idêntico a este documento.
5. No seu *fork*, acesse o menu *Settings > Members*.
6. Adicione o usuário **brytecnologia** como membro *Maintainer* do projeto, para que possamos acompanhar seu desenvolvimento.
7. Clone o projeto em sua máquina.
8. Crie uma conta e/ou autentique-se no [Figma](https://www.figma.com/) para acessar o projeto gráfico utilizando este [link](https://www.figma.com/file/yWrBerebGXbyqPnXG5ZKWE/teste-front-end?node-id=0%3A1).
9. Mãos a obra!
10. Havendo quaisquer instruções especiais para execução do projeto, descreva-as num arquivo **README.md** na raiz do projeto.
11. Ao final do desafio, faça um *push* do seu projeto e notifique o representante da BRy responsável pelo seu processo seletivo de que você terminou o desafio.

Observações: 

* Pedimos que trabalhe apenas no branch *master* - não será relevante, para a avaliação, o uso de branches de desenvolvimento.
* Se nenhum aviso de finalização for dado até o fim do prazo para cumprimento do desafio, o conteúdo do branch *master* será considerado como a entrega para a avaliação. 

## Requisitos da aplicação

Requisitos **fundamentais**:
* Será considerado o desenvolvimento com fidelidade ao projeto gráfico. Observe a página Instruções no projeto.
* Desenvolver páginas que são responsivas, ou seja, que adaptam-se para melhor visualização em dispositivos com diferentes resoluções. (Desktop e Mobile)
* Utilizar imagens em SVG.

Requisitos **desejáveis**:
* Capacidade de consumir a API REST para obter os dados dos filmes e personagens de forma paginada. (a documentação da API para consumir pode ser lida [aqui](https://swapi.bry.com.br))
* Utilizar um framework ou biblioteca JavaScript de frontend, orientado a componentes para o desenvolvimento de uma Single Page Application, sendo preferencialmente React ou Angular 7.

Estes são os requisitos de todas as páginas envolvidas no desafio:

*Caso opte por não consumir a API REST, as páginas podem ser estáticas*

* **Página inicial**:
  * A mudança de página dos carrosséis devem possuir animação de rolagem tipicas de carrosséis.
  * Os carrosséis devem possuir [rolagem infinita](https://blackpixel.com/writing/Carousel.gif)
  * Sobre o "carrossel de filmes":
    * Exibe no máximo 3 filmes por página do carrossel.
  * Sobre o "carrossel de personagens":
    * Exibe no máximo 4 personagens por página de carrossel.
  * Ao clicar em um card de um filme, a página de detalhes deve ser exibida.

* **Página de detalhes de um filme**:
  * A lista de personagens deve possuir o mesmo comportamento da pagina inicial, com a diferença que exibe apenas os personagens presentes no filme.

*Caso opte por consumir a API REST, considere também os requisitos abaixo, é importante reforçar que estes são **OPCIONAIS***

* **Página inicial**:
  * Ao acessar o campo de busca e apertar enter com o campo preenchido, o filtro deve ser aplicado em ambos os carrosséis de filmes (título) e personagens (nome).
  * Enquanto os dados dos filmes e/ou personagens estiverem sendo carregados da API, um "content loading" deve ser exibido conforme especificado no projeto gráfico.
  * Sobre o "carrossel de filmes", como são apenas 7 filmes, todos os filmes podem ser carregados de uma vez.
  * Sobre o "carrossel de personagens", os personagens devem ser carregados de 10 em 10 conforme o usuário avança páginas no carrossel, e enquanto mais personagens estão sendo carregados da API, o content loading deve ser exibido.
  * A API não disponibiliza imagens dos filmes e dos personagens, então utilize os ícones e imagens que estão no projeto gráfico.

* **Página de detalhes de um filme**:
  * A lista de personagens deve possuir o mesmo comportamento da pagina inicial, com a diferença que exibe apenas os personagens presentes no filme.
