# Trello cards

All the cards from our shared Trello Board used in this class.

# [Admin] Administrador vê todas filiais

Eu, usuário administrador,
Gostaria de ver todas as filiais disponíveis,
Para ter certeza de que todas as filiais estão cadastradas.

Filial (Subsidiary): 

- Name: string
- CNPJ: string
- Address: string

# [Admin] Cadastrar uma filial

Eu, usuário administrador,
Gostaria de cadastrar/editar uma nova filial
Para aumentar a frota de carros e expandir área de atendimento.

Filial (Subsidiary): 

- Name: string
- CNPJ: string
- Address: string

# [Admin] Validar dados da filial

Eu, usuário administrador,
Gostaria que o sistema validasse que uma mesma filial não seja cadastrada duas vezes e que uma filial só seja cadastrada com um CNPJ válido,
Para evitar cadastros indevidos na base de dados.

Filial (Subsidiary): 

- Name: string
- CNPJ: string
- Address: string

Informações Adicionais:

Você deve fazer 2 validações obrigatoriamente para o CNPJ ( deve ser obrigatório e único). Outras validações bônus são: garantir a quantidade caracteres (13) e garantir que o CNPJ é válido. 

Você pode validar usando um método próprio (https://guides.rubyonrails.org/active_record_validations.html#custom-methods) ou usando uma gem externa, como a https://github.com/fnando/cpf_cnpj

# [Admin] Administrador vê todas categorias de carro

Eu, usuário administrador,
Gostaria de ver todas categorias de carro cadastradas, 
Para ter certeza de que todas categorias estão cadastradas no sistema e então cadastrar os carros para locação.

Categoria (CarCategory)

- Name: string
- Daily Rate: decimal
- Car insurance: decimal
- Third party insurance: decimal

# [Admin] Cadastrar categorias com preços padrão

Eu, usuário administrador,
Gostaria de cadastrar categorias de carros com valores padrão para diária, seguro do carro e seguro contra terceiros, 
Para que possam ser cadastrados preços de locação por categoria em cada filial

Categoria (CarCategory)

- Name: string
- Daily Rate: float
- Car insurance: float
- Third party insurance: float

# [User] Cadastrar um cliente

Eu, usuário de uma filial, 
Gostaria de cadastrar um cliente
Para que ele possa realizar uma locação.

Cliente (Client):

- Nome (name): string
- CPF (document): string
- Email (email): string
