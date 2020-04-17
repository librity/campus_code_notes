# Trello cards

All the cards from our shared Trello Board used in this class.

# [Admin] Validar dados da fabricante

Eu, usuário administrador,
Gostaria que o sistema validasse que uma fabricante só seja cadastrado com um nome válido (não vazio) e que uma fabricante não seja cadastrada duas vezes,
Para evitar cadastros indevidos na base de dados.


## Dicas e Informações

Nessa tarefa vamos resolver nossos primeiros testes unitários. O arquivo `manufacturer_spec.rb` possui 2 testes que garantem que estamos adicionando validações em nosso `model`. O teste segue a mesma lógica dos testes de aceitação/integração, com uma etapa onde criamos os dados, uma etapa onde executamos o código e uma etapa de verificação dos resultados.

A grande diferença aqui é que, ao invés de executar a aplicação, visitar links, preencher formularios etc, nosso teste simplesmente executa o método `valid?` em um objeto do tipo `Manufacturer`. Essa é a principal característica de testes unitários: eles focam na execução de um único método e no retorno desse método dado as condições estabelecidas no começo do teste.

# [Admin] Editar um fabricante

Eu, usuário administrador,
Gostaria de editar um fabricante de carros
Para que eu possa corrigir erros durante o cadastro.

## Dicas e Informações

Para editar um objeto, repare que os testes sempre começam criando um objeto diretamente na base de dados através do método `create!`. Não é necessário criar objetos via formulário pois isso deixaria o teste mais lento - com o método `create` o objeto é salvo no banco de dados em apenas um passo, para utilizar o formulário precisaríamos de passos para abrir o formulário, preencher os campos e clicar no botão 'Enviar'. 

Repare também que existem testes para garantir que todas validações adotadas no processo de cadastro continuem sendo respeitadas aqui.

# [Admin] Apagar um fabricante

Eu, usuário administrador,
Gostaria de apagar um fabricante de carros
Para que que não conste na lista de fabricantes.

# [Admin] Create the appropriate attribute validations for all resources

Customer's Email: unique, and validate format.
Subsidiary's name: unique
CarCategory's name: unique

# [Admin] Finish CRUD for all resources

Create Update and Destroy actions with their corresponding views for all resources created so far: Manufacurers, CarCategories, Subsidiaries and Customers.
