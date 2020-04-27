# Trello cards

All the cards from our shared Trello Board used in this class.

# [Admin] Vê os modelos de carro

Eu, usuário administrador,
Gostaria de acessar uma lista de todos os modelos de carro,
Para saber quais já foram cadastrados.

Modelo de Carro (CarModel): 

- Nome (name): string
- Ano (year): number
- Fabricante (Manufacturer): object
- Cavalos (motorization): string
- Categoria (CarCategory): object
- Tipo de combustível (fuel_type): string 
- metric_city_milage: integer, 
- metric_highway_milage: integer

# Application-wide I18n

Implement Internationalization and Localization on all views and controllers created so far. 
That means links, labels, resource/model names and any other tag. If it displays text it 
should probably be formatted.

# Test-wide I18n

Implement Internationalization and Localization on all integration tests created so far. 
That means expects to call I18n functions instead of using raw strings. If it displays text 
it should probably be formatted.

# Semantic HTML

Refactor all your views to have a more semantic html (main, section, header, article, etc).

# Advanced capybara

Refactor all your integration tests to use capybara's advanced features *when necessary* 
(`expect(page).to have_css('header h1', text: 'Categoria A')`, etc.)

# Delete modals with tests

Refactor your delete views and tests to have 'are you sure?' modals.

# Format method for CPF & CNPJ

Create a format CPF/CNPJ for Customer & Subsidiary, and integrate it with the views and form inputs

# Use html `<table>` for show views

# Add engine attribute to car model

# Validar preços da categoria de carro

Eu, um usuário da aplicação,
Gostaria que fosse validado que os preços da diária, do seguro do carro e do seguro para terceiros sejam maiores do que zero,
Para evitar cadastros errados na plataforma.

- [x]  use href key on `expect to have link_to('Voltar', href: root_path)`
- [x]  Create a format CPF/CNPJ for Customer & Subsidiary, and integrate it with the views and form inputs
- [x]  Refactor cpf & cnpj validators
- [x]  [CarCategory] Add greater_than 0 validations for daily_rate, insurance & third_party_insurance
- [x]  Use <table> for index views
- [x]  Correct year to integer with migration.
- [x]  Add engine attribute to car model
 