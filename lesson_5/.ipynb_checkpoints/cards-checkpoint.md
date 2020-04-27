# Trello cards

All the cards from our shared Trello Board used in this class.

# [Admin] Agendar uma locação

Eu, um administrador do sistema,
Gostaria de agendar uma locação para um cliente
Para que ele possa retirar o veículo na data desejada.

Locaçao (Rental):

  - Start date: date
  - End date: date
  - Client: object
  - CarCategory: object

# [Admin] Ver locações agendadas

Eu, um administrador do sistema,
Gostaria de ver todas locações agendadas,
Para ter uma visão rápida de todas locações previstas para os próximos dias.

Locaçao (Rental):

  - Start date: date
  - End date: date
  - Client: object
  - CarCategory: object

# [Admin] Cadastrar um carro para frota

Eu, usuário administrador, 
Gostaria de cadastrar um novo carro para a frota de uma filial
Para que esse carro possa ser alugado no futuro pelos clientes.

Carro (Car): 

  - Placa (license_plate): string
  - Cor (color): string
  - Car Model: object
  - Quilometragem (mileage): integer
  - Subsidiary: object
