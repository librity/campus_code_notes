# Trello cards

All the cards from our shared Trello Board used in this class.

# Criar o projeto

Tudo começa com a criação de um novo projeto Rails. Vamos usar a versão 6 do framework e para isso você vai precisar de uma versão de Ruby atualizada (recomendamos qualquer versão a partir da 2.5.0).

Além do Ruby você vai precisar ter instalado outros pré-requisitos:

- Git (https://git-scm.com/book/pt-br/v2/Começando-Instalando-o-Git)
- NodeJS (https://nodejs.org/pt-br/download/package-manager/)
- yarn (https://classic.yarnpkg.com/pt-BR/docs/install/)

Recomendamos também que você crie uma pasta em seu computador para manter todos os seus projetos. Essa é uma prática comum entre devs e os nomes mais populares são `projects` ou `workspace`. 

Pelo terminal, navegue até sua pasta de projetos e execute o comando `rails new rental-cars -T`.  A opção `-T` vai impedir o Rails de adicionar o framework padrão de testes (minitest) que não é o mais utilizado em projetos comerciais.

Vamos utilizar o `rspec-rails` com `Capybara` em nosso projeto. Para isso atualize seu `Gemfile` de acordo com a **documentação** dessas duas gems e não esqueça de executar o comando `rails generate rspec:install` ao final.


Documentações:

Rails: http://guides.rubyonrails.org/
rspec: https://github.com/rspec/rspec-rails
capybara: https://github.com/teamcapybara/capybara

# Fluxo de Trabalho

Agora que você já tem o projeto configurado, vamos começar a codificar as funcionalidades planejadas. 

Cada funcionalidade vai ser descrita como um card/cartão aqui no Trello. O título do card serve como resumo do que deve ser feito e também como referência para nossa comunicação no Slack. Então, ao tirar dúvidas você pode sempre postar algo como: 'No card onde o Visitante deve abrir o site...' 

Ainda no título de cada card temos o escopo entre colchetes. Por exemplo: [Admin] Administrador cadastra clientes. O escopo [Admin] vai ser importante em funcionalidades mais avançadas. Então por enquanto apenas vá se acostumando com essa sintaxe  e não se preocupe :) 

Em cada card teremos também uma descrição no formate de uma User Story. Esse formato conta em uma pequena quantidade linhas:
- QUEM irá fazer alguma ação no sistema (visitante, usuário autenticado, admin etc)
- O QUÊ deve ser feito (um cadastro, acessar uma página, um botão para remover itens do banco de dados)
- PARA QUÊ essa ação será executada, ajudando você dev a entender o propósito do código criado

Ao longo do nosso trbalho vamos discutir mais esse formato, ele não é o único mas é bastante popular para documentar de forma rápida uma tarefa.

Também nos cards, você vai encontrar arquivos em anexo que são os testes daquela tarefa. Todo processo de criação de código do treinamento será orientado a testes. Os testes vão estabelecer o que você precisa fazer para concluir uma tarefa. Quando todos os testes estiverem passando (verdes) você está pronto para a próxima tarefa.

Os arquivos de testes devem ser movidos para a pasta `spec` do seu projeto e sempre (SEMPRE) devem ser substituídos em caso de arquivos duplicados.

Ao final de cada tarefa (card), esperamos que você faça um novo `commit` em seu projeto. Assim, com o passar dos dias, você pode revistar toda a linha do tempo das tarefas realizadas e ver sua evolução :)

# [Visitante] Visitante abre o site

Eu, um visitante ainda não autenticado,
Gostaria de acessar a aplicação,
Para ter certeza de que estou no site da RentalCars e posso começar a utilizar os recursos do sistema.

# [Visitante] Visitante vê os fabricantes

Eu, um visitante não autenticado,
Gostaria de acessar uma lista de todos fabricantes de carro,
Para saber quais fabricantes já foram cadastrados.

## Dicas e Informações

- Um fabricante deve ter um nome, do tipo string. 
- A tela de `index` dos fabricantes deve listar todos fabricantes
- Para cada fabricante deve haver um link para ver sua página de detalhes (`show`)

# [Admin] Cadastrar um fabricante

Eu, usuário administrador,
Gostaria de cadastrar um fabricante de carros
Para que modelos de carros sejam criados utilizando os nomes de fabricantes pré-cadastrados.

