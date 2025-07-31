# Banco de Dados - Rede de Hotéis Fictícia

Esse projeto foi criado para modelar o banco de dados de uma rede de hotéis, atendendo às regras de negócio fornecidas.
O objetivo é organizar dados de hotéis, quartos, funcionários, hóspedes, reservas e pagamentos de forma clara e eficiente.

---

# O que esse modelo cobre

- Cadastro de hotéis com endereço completo
- Vários quartos por hotel
- Funcionários associados a um hotel
- Hóspedes com dados e endereço
- Reservas feitas por hóspedes e agendadas por funcionários
- Pagamento único por reserva
- Relação muitos-para-muitos entre reservas e quartos

---

# Modelo Entidade-Relacionamento (MER)

O diagrama abaixo mostra como as tabelas se relacionam:

<img width="957" height="940" alt="Captura de tela 2025-06-28 114939" src="https://github.com/user-attachments/assets/837c5d76-d70b-4fcf-916b-24f9ba3e3b59" />

Tecnologias: SQL e Draw.io

---

# Pitch Inicial

Uma Rede de Hotéis necessita controlar os dados dos funcionários, das unidades, dos quartos, dos hóspedes, das reservas e dos pagamentos. Para isso, contratou um profissional de Banco de Dados, a fim de modelar o Banco de Dados que armazenará todos os dados.

As regras de negócio são:

- Funcionário – Deverão ser armazenados os seguintes dados: CPF, nome, telefone, e-mail, login e senha;
- Hotel – Deverão ser armazenados os seguintes dados: identificação do hotel, nome, categoria, telefone, e-mail e endereço, sendo o endereço composto por rua, número, complemento, bairro, CEP, cidade e estado;
- Quarto – Deverão ser armazenados os seguintes dados: identificação do quarto, número de leitos, tipo (standard, luxo ou suíte), preço da diária e status (disponível, ocupado ou manutenção);
- Hóspede – Deverão ser armazenados os seguintes dados: CPF, nome, telefone, email e endereço, sendo o endereço composto por rua, número, complemento, bairro, CEP, cidade e estado;
- Reserva – Deverão ser armazenados os seguintes dados: identificação da reserva, data de entrada, data de saída e status (ativa, cancelada ou concluída);
- Pagamento – Deverão ser armazenados os seguintes dados: identificação do pagamento, forma de pagamento (cartão, pix ou dinheiro), data do pagamento, valor total e status (pago ou pendente);
- Um hotel possui um ou vários quartos;
- Um ou vários funcionários trabalham em um hotel;
- Um funcionário realiza uma ou várias reservas;
- Um ou vários quartos fazem parte de uma ou várias reservas;
- Um hóspede pode fazer uma ou várias reservas;
- Uma reserva gera um pagamento.
