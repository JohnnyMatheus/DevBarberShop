<p align="center">
<img src="https://github.com/JohnnyMatheus/DevBarberShop-Trabalho-Final/blob/main/imagens/devbarberLogo.png"/>
</p>

## 🔷Tópicos 
- [Descrição do projeto](#descrição-do-projeto)
- [Levantamento de Requisitos](#Levantamento-de-Requisitos)
- [Prototipagem](#Prototipagem)
- [Ferramentas utilizadas](#ferramentas-utilizadas)
- [Diagrama de caso de uso](#Diagrama-de-atividades)
- [Diagramas de sequência](Diagrama-de-sequência)
- [Diagrama de atividades](#Diagrama-de-atividades)
- [Diagrama de estado](#Diagrama-de-estado)
- [Diagrama de classes](#Diagrama-de-classes)
- [Modelagem](#Modelagem)
- [Script Banco de dados](#Script-Banco-de-Dados)
- [Desenvolvedor](#Desenvolvedor)
- [Professor](#Professor)

## 🔷Descrição do projeto
<p>Projeto desenvolvido envolvendo as diciplinas Banco de Dados II, Engenharia de Software I e Programação II do curso de Ciências da Computação. O projeto tem por objetivo por em prática os conhecimentos adquiridos em aula.</p>
<p>
 O sistema 💈&lt;DevBarberShop/&gt;💈foi desenvolvido para gerenciar as operações de uma barbearia, incluindo o cadastro de clientes, fornecedores, funcionários, serviços, produtos, agendamentos e pagamentos. As tabelas foram estruturadas para fornecer um controle eficiente e organizado, garantindo uma gestão integrada de todos os aspectos da barbearia.
</p>

<h2 align="center">🔷Levantamento de Requisitos</h2>

## 🔹Requisitos Funcionais
<p>Cadastro de Clientes: O sistema deve permitir o cadastro de clientes com informações como nome, telefone, e-mail, endereço, sexo e data de nascimento.</p>
<p>Cadastro de Fornecedores: O sistema deve permitir o cadastro de fornecedores com informações como nome, telefone, e-mail e endereço.</p>
<p>Cadastro de Funcionários: O sistema deve permitir o cadastro de funcionários com informações como nome, telefone, e-mail, cargo e salário.</p>
<p>Cadastro de Serviços: O sistema deve permitir o cadastro de serviços oferecidos pela barbearia, incluindo nome, descrição e preço.</p>
<p>Cadastro de Produtos: O sistema deve permitir o cadastro de produtos, incluindo nome, descrição, quantidade em estoque, preço, e o fornecedor responsável.</p>
<p>Agendamento de Serviços: O sistema deve permitir que os clientes agendem serviços com os funcionários, especificando a data, hora e status do agendamento.</p>
<p>Registro de Pagamentos: O sistema deve permitir o registro de pagamentos realizados pelos clientes para os serviços agendados, incluindo valor, forma de pagamento e data/hora do pagamento.</p>
<p>Histórico de Serviços: O sistema deve registrar o histórico de serviços prestados, com detalhes sobre o serviço realizado, o cliente atendido, e o funcionário responsável.</p>
<p>Relatórios e Consultas: O sistema deve possibilitar a consulta e a geração de relatórios sobre agendamentos, pagamentos e histórico de serviços.</p>

## 🔹Requisitos não Funcionais
<p>Desempenho: O sistema deve ser capaz de processar as transações de agendamento e pagamento rapidamente, sem causar lentidão no sistema.</p>
<p>Segurança: O sistema deve garantir a segurança dos dados, com criptografia das informações sensíveis, como e-mails e números de telefone, além de controle de acesso para diferentes perfis (clientes, funcionários e administradores).</p>
<p>Escalabilidade: O sistema deve ser capaz de se adaptar ao crescimento da barbearia, permitindo a adição de novos funcionários, clientes, serviços e produtos sem impacto significativo no desempenho.</p>
<p>Compatibilidade: O sistema deve ser compatível com diferentes dispositivos e navegadores, garantindo uma experiência fluida para os usuários.</p>
<p>Usabilidade: A interface do sistema deve ser simples, intuitiva e fácil de navegar, com feedback claro para o usuário em cada interação.</p>
<p>Backup e Recuperação de Dados: O sistema deve permitir a criação de backups periódicos dos dados, garantindo que as informações possam ser recuperadas em caso de falha.</p>
<p>Acessibilidade: O sistema deve ser acessível a pessoas com deficiência, seguindo as diretrizes de acessibilidade web, como W3C WCAG.</p>


## 🔹Requisitos de Dominio
<p>🔸Cliente</p>
<p>Cada cliente deve ter um código de identificação único, nome, telefone, e-mail, endereço (bairro, rua, cidade), sexo e data de nascimento.</p>
<p>Os dados do cliente são essenciais para o agendamento de serviços e registro de histórico.</p>

<p>🔸Fornecedor</p>
<p>Cada fornecedor deve ter um código único, nome, telefone, e-mail e endereço, facilitando o controle dos produtos e insumos.</p>

<p>🔸Funcionário</p>
<p>Funcionários devem ter um código único, nome, telefone, e-mail, cargo e salário.</p>
<p>Funcionários são essenciais para o agendamento e execução de serviços.</p>

 <p>🔸Serviço</p>
<p>Cada serviço deve ter um código, nome, descrição e preço.</p>
<p>Os serviços são agendados pelos clientes e registrados no histórico de serviços prestados.</p>

 <p>🔸Produto</p>
<p>Cada produto deve ter um código único, nome, descrição, quantidade em estoque e preço.</p>
<p>Produtos são vinculados a fornecedores e são essenciais para a execução de certos serviços.</p>

 <p>🔸Agendamento</p>
<p>Cada agendamento é identificado por um código e contém a data/hora do serviço, cliente e funcionário responsáveis.</p>
<p>Os agendamentos representam a reserva de um serviço e devem ser gerenciados de acordo com políticas de cancelamento e alteração.</p>

 <p>🔸Pagamento</p>
<p>Pagamentos são identificados por um código e contêm informações de valor, data/hora e forma de pagamento, além do cliente e agendamento vinculados.</p>
<p>O pagamento finaliza a prestação de serviço.</p>

<p>🔸Histórico de Serviços</p>
<p>O histórico de serviços contém registros de todos os serviços realizados, com data/hora, serviço prestado, cliente e funcionário envolvidos.</p>
<p>Este histórico é importante para consultas futuras sobre serviços realizados e pode ser usado para análise do perfil do cliente.</p>

## 🔷Protótipo

## ⚒️Ferramentas utilizadas

| [<img src="https://wiki.postgresql.org/images/3/30/PostgreSQL_logo.3colors.120x120.png" width=115><br><sub>PostgreSQL</sub>](https://www.postgresql.org/download/) | [<img src="https://freesoft.ru/storage/images/221/2207/220636/220636_normal.png" width=115><br><sub>Visual Paradigm 17.1</sub>](https://www.visual-paradigm.com/download/community.jsp) | [<img src="https://dbeaver.io/wp-content/uploads/2015/09/beaver-head.png" width=115><br><sub>DBeaver</sub>](https://dbeaver.io) | [<img src="https://upload.wikimedia.org/wikipedia/commons/4/44/Spring_Framework_Logo_2018.svg" width=115><br><sub>Spring Boot</sub>](https://spring.io/projects/spring-boot) | [<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width=115><br><sub>GitHub</sub>](https://github.com/) | [<img src="https://brandlogos.net/wp-content/uploads/2021/11/java-logo.png" width=115><br><sub>Java</sub>](https://www.oracle.com/java/technologies/javase-downloads.html) | [<img src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Visual_Studio_Code_1.35_icon.svg" width=115><br><sub>VS Code</sub>](https://code.visualstudio.com/) | [<img src="https://th.bing.com/th/id/OIP.J8BxOW4ZXI79Yf2cwu4UOAHaFS?rs=1&pid=ImgDetMain" width=115><br><sub>eclipseide</sub>](https://eclipseide.org/) |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |

## 🔷Diagrama de Caso de uso
<p align="center">
 <img src="https://github.com/JohnnyMatheus/DevBarberShop-Trabalho-Final/blob/main/Diagramas/Diagrama%20de%20caso%20de%20Uso.png"/>
</p>

## 🔷Diagrama de Fluxos
<p align="center">
 <img src="https://github.com/JohnnyMatheus/DevBarberShop-Trabalho-Final/blob/main/Diagramas/DIagrama%20de%20fluxo.drawio.png"/>
</p>

## 🔷Diagrama de sequência
<p align="center">
 <img src="https://github.com/JohnnyMatheus/DevBarberShop-Trabalho-Final/blob/main/Diagramas/diagrama%20de%20sequencia.jpg"/>
</p>

## 🔷Diagrama de atividades
<p align="center">
 <img src="https://github.com/JohnnyMatheus/DevBarberShop-Trabalho-Final/blob/main/Diagramas/diagrama%20de%20atividades.jpg"/>
</p>

## 🔷Diagramas de estado
<p align="center">
 <img src="https://github.com/JohnnyMatheus/DevBarberShop-Trabalho-Final/blob/main/Diagramas/Diagrama%20de%20Estados.png"/>
</p>

## 🔷Diagramas de classes
<p align="center">
 <img src="https://github.com/JohnnyMatheus/DevBarberShop-Trabalho-Final/blob/main/Diagramas/diagrama%20de%20classe.jpg"/>
</p>

## ⚙️Modelagem
Você pode [acessar a modelagem do projeto aqui]()

<p align="center">
<img src="https://github.com/JohnnyMatheus/DevBarberShop-Trabalho-Final/blob/main/imagens/modelagem-atualizada.png">
</p>

## 🎲Script - Criação do Banco do Dados
```sql
--Script - criação do Banco do Dados
create database devbarbershop;

```
## 🎲Script - criação Tabelas
```sql
-- Script de criação de tabelas

create table cliente(
    codcli int generated by default as identity primary key,
    nomcli varchar(150) not null,
    telcli varchar(20) not null,
    emailcli varchar(100) not null,
    bairrocli varchar(100) not null,
    ruaendcli varchar(100) not null,
    sexocli varchar(10) not null,
    cidadecli varchar(50) not null,
    dtnascli date not null
);

comment on table cliente is 'Tabela de clientes da Barbearia';
comment on column cliente.codcli is 'Código do cliente';
comment on column cliente.nomcli is 'Nome do cliente';
comment on column cliente.telcli is 'Telefone do cliente';
comment on column cliente.emailcli is 'E-mail do cliente';
comment on column cliente.bairrocli is 'Bairro do cliente';
comment on column cliente.ruaendcli is 'Rua do endereço do cliente';
comment on column cliente.sexocli is 'Sexo do cliente';
comment on column cliente.cidadecli is 'Cidade do cliente';
comment on column cliente.dtnascli is 'Data de nascimento do cliente';

-----------------------------------------------------------------------------------------------

create table fornecedor(
    codforn int generated by default as identity primary key,
    nomeforn varchar(150) not null,
    telforn varchar(20),
    emailforn varchar(100),
    enderecoforn varchar(100)
);

comment on table fornecedor is 'Tabela de fornecedores';
comment on column fornecedor.codforn is 'Código do fornecedor';
comment on column fornecedor.nomeforn is 'Nome do fornecedor';
comment on column fornecedor.telforn is 'Telefone do fornecedor';
comment on column fornecedor.emailforn is 'E-mail do fornecedor';
comment on column fornecedor.enderecoforn is 'Endereço do fornecedor';

-----------------------------------------------------------------------------------------------

create table funcionario(
    codfun int generated by default as identity primary key,
    nomefun varchar(100) not null,
    telfun varchar(20) not null,
    emailfun varchar(100) not null,
    cargofun varchar(100) not null,
    salariofun numeric(10, 2) not null
);

comment on table funcionario is 'Tabela de funcionários da Barbearia';
comment on column funcionario.codfun is 'Código do funcionário';
comment on column funcionario.nomefun is 'Nome do funcionário';
comment on column funcionario.telfun is 'Telefone do funcionário';
comment on column funcionario.emailfun is 'E-mail do funcionário';
comment on column funcionario.cargofun is 'Cargo do funcionário';
comment on column funcionario.salariofun is 'Salário do funcionário';

-----------------------------------------------------------------------------------------------

create table servico(
    codserv int generated by default as identity primary key,
    nomeserv varchar(100) not null,
    descserv varchar(100),
    precoserv numeric(10, 2) not null
);

comment on table servico is 'Tabela de serviços oferecidos pela Barbearia';
comment on column servico.codserv is 'Código do Serviço';
comment on column servico.nomeserv is 'Nome do serviço';
comment on column servico.descserv is 'Descrição do serviço oferecido pela Barbearia';
comment on column servico.precoserv is 'Preço dos serviços oferecidos pela Barbearia';

-----------------------------------------------------------------------------------------------

create table produto(
    codprod int generated by default as identity primary key,
    nomeprod varchar(100) not null,
    descprod varchar(255),
    qtdprod int not null,
    precoprod numeric(10, 2) not null,
    fornecedorcodforn int references fornecedor(codforn),
    servicocodserv int references servico(codserv)
);

comment on table produto is 'Tabela de produtos';
comment on column produto.codprod is 'Código do produto';
comment on column produto.nomeprod is 'Nome do produto';
comment on column produto.descprod is 'Descrição do produto';
comment on column produto.qtdprod is 'Quantidade do produto em estoque';
comment on column produto.precoprod is 'Preço do produto';
comment on column produto.fornecedorcodforn is 'Código do fornecedor do produto';
comment on column produto.servicocodserv is 'Código do serviço relacionado ao produto';

-----------------------------------------------------------------------------------------------

create table agendamento(
    codagen int generated by default as identity primary key,
    data_hora timestamp not null,
    status varchar(50) not null,
    clientecodcli int references cliente(codcli),
    funcionariocodfun int references funcionario(codfun)
);

comment on table agendamento is 'Tabela de agendamentos';
comment on column agendamento.codagen is 'Código do agendamento';
comment on column agendamento.data_hora is 'Data e hora do agendamento';
comment on column agendamento.status is 'Status do agendamento';
comment on column agendamento.clientecodcli is 'Código do cliente';
comment on column agendamento.funcionariocodfun is 'Código do funcionário';

-----------------------------------------------------------------------------------------------

create table pagamento(
    codpag int generated by default as identity primary key,
    valor numeric(10, 2) not null,
    data_hora_pagamento timestamp not null,
    forma_pagamento varchar(50) not null,
    clientecodcli int references cliente(codcli),
    agendamentocodagen int references agendamento(codagen)
);

comment on table pagamento is 'Tabela de pagamentos';
comment on column pagamento.codpag is 'Código do pagamento';
comment on column pagamento.valor is 'Valor do pagamento';
comment on column pagamento.data_hora_pagamento is 'Data e hora do pagamento';
comment on column pagamento.forma_pagamento is 'Forma de pagamento';
comment on column pagamento.clientecodcli is 'Código do cliente';
comment on column pagamento.agendamentocodagen is 'Código do agendamento';

-----------------------------------------------------------------------------------------------

create table historico_servico(
    codhistorico int generated by default as identity primary key,
    data_hora timestamp not null,
    servicocodserv int references servico(codserv),
    clientecodcli int references cliente(codcli),
    funcionariocodfun int references funcionario(codfun)
);

comment on table historico_servico is 'Tabela de histórico de serviços prestados';
comment on column historico_servico.codhistorico is 'Código do histórico de serviço';
comment on column historico_servico.data_hora is 'Data e hora do serviço';
comment on column historico_servico.servicocodserv is 'Código do serviço';
comment on column historico_servico.clientecodcli is 'Código do cliente';
comment on column historico_servico.funcionariocodfun is 'Código do funcionário';


```
## 🎲Script - Inserir dados na Tabela
```sql
-- Inserts para Clientes
insert into cliente (nomcli, telcli, emailcli, bairrocli, ruaendcli, sexocli, cidadecli, dtnascli) values
    ('Nelson Ramos Rodrigues Junior', '(49) 9999-9999', 'nelson@example.com', 'Centro', 'Rua A', 'Masculino', 'São Miguel do Oeste', '1990-05-15'),
    ('Nathaniel Nicolas Rissi Soares', '(49) 8888-8888', 'nathaniel@example.com', 'Agostini', 'Rua B', 'Masculino', 'Maravilha', '1995-08-20'),
    ('Iraê Ervin Gruber da Silva', '(49) 7777-7777', 'irae@example.com', 'Centro', 'Rua C', 'Masculino', 'Descanso', '1992-03-10'),
    ('Jefferson Alan Schmidt Ludwig', '(49) 6666-6666', 'jefferson@example.com', 'Agostini', 'Rua D', 'Masculino', 'Itapiranga', '1998-11-25'),
    ('Leandro Bertocchi', '(49) 5555-5555', 'leandro@example.com', 'Centro', 'Rua E', 'Masculino', 'Guaraciaba', '1997-04-30'),
    ('Matheus José', '(49) 4444-4444', 'matheus@example.com', 'Centro', 'Rua F', 'Masculino', 'São Miguel do Oeste', '1993-09-05'),
    ('Nícolas Basotti', '(49) 3333-3333', 'nicolas@example.com', 'Agostini', 'Rua G', 'Masculino', 'Maravilha', '1996-06-18'),
    ('Iago Azevedo', '(49) 2222-2222', 'iago@example.com', 'Centro', 'Rua H', 'Masculino', 'Descanso', '1991-02-22'),
    ('Rafael Azevedo', '(49) 1111-1111', 'rafael@example.com', 'Agostini', 'Rua I', 'Masculino', 'Itapiranga', '1994-07-12'),
    ('Luis Paulo', '(49) 0000-0000', 'luis@example.com', 'Centro', 'Rua J', 'Masculino', 'Guaraciaba', '1999-12-31');
   
--------------------------------------------------------------------------------------------------------------------------------------------------

   --Inserts para Funcionários
insert into funcionario (nomefun, telfun, emailfun, cargofun, salariofun) values
    ('NATANI GABRIELA GAYARDO', '(49) 1111-2222', 'natani@example.com', 'Barbeiro', 2500.00),
    ('JOHNNY MATHEUS NOGUEIRA DE MEDEIRO', '(49) 2222-3333', 'johnny@example.com', 'Cabeleireiro', 2800.00),
    ('ROBERSON JUNIOR FERNANDES ALVES', '(49) 3333-4444', 'roberson@example.com', 'Esteticista', 3000.00);
   
--------------------------------------------------------------------------------------------------------------------------------------------------

--Insert para Fornecedor
insert into fornecedor (nomeforn, telforn, emailforn, enderecoforn) values
    ('UNOESC', '(49) 9999-9999', 'unoesc@example.com', 'Rua Universitária, 123');
   
--------------------------------------------------------------------------------------------------------------------------------------------------

--Inserts para Serviços
insert into servico (nomeserv, descserv, precoserv) values
    ('Corte de Cabelo', 'Corte de cabelo masculino', 50.00),
    ('Barba', 'Barba completa', 30.00),
    ('Coloração', 'Coloração de cabelo', 80.00),
    ('Depilação', 'Depilação masculina', 100.00),
    ('Massagem Relaxante', 'Massagem corporal relaxante', 120.00);
   
--------------------------------------------------------------------------------------------------------------------------------------------------
    
--Inserts para Produtos
insert into produto (nomeprod, descprod, qtdprod, precoprod, fornecedorcodforn, servicocodserv) values
    ('Shampoo', 'Shampoo para cabelos masculinos', 100, 25.00, 1, null),
    ('Condicionador', 'Condicionador para cabelos masculinos', 80, 20.00, 1, null),
    ('Pomada Modeladora', 'Pomada modeladora para cabelos', 120, 35.00, 1, null),
    ('Cera Modeladora', 'Cera modeladora para cabelos', 90, 30.00, 1, null);

--------------------------------------------------------------------------------------------------------------------------------------------------

--Inserts para Agendamentos
insert into agendamento (data_hora, status, clientecodcli, funcionariocodfun) values
    ('2024-07-10 09:00:00', 'Agendado', 1, 1),
    ('2024-07-12 15:30:00', 'Agendado', 2, 2),
    ('2024-07-15 11:00:00', 'Agendado', 3, 3),
    ('2024-07-18 14:00:00', 'Agendado', 4, 1),
    ('2024-07-20 10:30:00', 'Agendado', 5, 2),
    ('2024-07-22 13:00:00', 'Agendado', 6, 3),
    ('2024-07-25 16:00:00', 'Agendado', 7, 1),
    ('2024-07-28 12:30:00', 'Agendado', 8, 2),
    ('2024-07-30 10:00:00', 'Agendado', 9, 3),
    ('2024-08-02 14:30:00', 'Agendado', 10, 1);
   
 --------------------------------------------------------------------------------------------------------------------------------------------------
  
 --Inserts para Pagamentos
insert into pagamento (valor, data_hora_pagamento, forma_pagamento, clientecodcli, agendamentocodagen) values
    (50.00, '2024-07-10 10:00:00', 'Dinheiro', 1, 1),
    (30.00, '2024-07-12 16:00:00', 'Cartão de Débito', 2, 2),
    (80.00, '2024-07-15 12:00:00', 'Cartão de Crédito', 3, 3),
    (100.00, '2024-07-18 15:00:00', 'Dinheiro', 4, 4),
    (120.00, '2024-07-20 11:00:00', 'Cartão de Crédito', 5, 5),
    (50.00, '2024-07-22 14:00:00', 'Dinheiro', 6, 6),
    (30.00, '2024-07-25 17:00:00', 'Cartão de Débito', 7, 7),
    (80.00, '2024-07-28 13:00:00', 'Cartão de Crédito', 8, 8),
    (100.00, '2024-07-30 11:00:00', 'Dinheiro', 9, 9),
    (120.00, '2024-08-02 15:00:00', 'Cartão de Crédito', 10, 10);

--------------------------------------------------------------------------------------------------------------------------------------------------
   
--Inserts para Histórico de Serviços
insert into historico_servico (data_hora, servicocodserv, clientecodcli, funcionariocodfun) values
    ('2024-07-10 09:30:00', 1, 1, 1),
    ('2024-07-12 15:45:00', 2, 2, 2),
    ('2024-07-15 11:30:00', 3, 3, 3),
    ('2024-07-18 14:30:00', 4, 4, 1),
    ('2024-07-20 10:45:00', 5, 5, 2),
    ('2024-07-22 13:30:00', 1, 6, 3),
    ('2024-07-25 16:30:00', 2, 7, 1),
    ('2024-07-28 12:45:00', 3, 8, 2),
    ('2024-07-30 10:15:00', 4, 9, 3),
    ('2024-08-02 14:45:00', 5, 10, 1);

```
## 🎲Script - Selects/consultas
```sql
-- Select
SELECT * FROM cliente;
SELECT * FROM fornecedor;
SELECT * FROM funcionario;
SELECT * FROM servico;
SELECT * FROM produto;
SELECT * FROM agendamento;
SELECT * FROM pagamento;
SELECT * FROM historico_servico;

--Consulta: Clientes e Seus Agendamentos
SELECT c.nomcli, a.data_hora, a.status 
FROM cliente c
JOIN agendamento a ON c.codcli = a.clientecodcli;

--------------------------------------------------------------------------------------------
--Consulta: Funcionários e Seus Agendamentos
SELECT f.nomefun, a.data_hora, a.status 
FROM funcionario f
JOIN agendamento a ON f.codfun = a.funcionariocodfun;

--------------------------------------------------------------------------------------------
--Consulta: Produtos e Seus Fornecedores

SELECT p.nomeprod, p.descprod, p.qtdprod, p.precoprod, f.nomeforn
FROM produto p
JOIN fornecedor f ON p.fornecedorcodforn = f.codforn;

--------------------------------------------------------------------------------------------
--Consulta: Serviços Prestados com Detalhes de Clientes e Funcionários

SELECT hs.data_hora, c.nomcli, s.nomeserv, s.descserv, f.nomefun
FROM historico_servico hs
JOIN cliente c ON hs.clientecodcli = c.codcli
JOIN servico s ON hs.servicocodserv = s.codserv
JOIN funcionario f ON hs.funcionariocodfun = f.codfun;

--------------------------------------------------------------------------------------------
--Consulta: Pagamentos Realizados por Cliente

SELECT p.valor, p.data_hora_pagamento, p.forma_pagamento, c.nomcli
FROM pagamento p
JOIN cliente c ON p.clientecodcli = c.codcli;

--------------------------------------------------------------------------------------------
--Consulta: Agendamentos com Detalhes de Clientes e Funcionários
SELECT a.data_hora, a.status, c.nomcli, f.nomefun
FROM agendamento a
JOIN cliente c ON a.clientecodcli = c.codcli
JOIN funcionario f ON a.funcionariocodfun = f.codfun;

--------------------------------------------------------------------------------------------
--Consulta: Total de Pagamentos por Cliente
SELECT c.nomcli, SUM(p.valor) AS total_pago
FROM pagamento p
JOIN cliente c ON p.clientecodcli = c.codcli
GROUP BY c.nomcli;

--------------------------------------------------------------------------------------------
--Consulta: Número de Agendamentos por Funcionário
SELECT f.nomefun, COUNT(a.codagen) AS total_agendamentos
FROM funcionario f
JOIN agendamento a ON f.codfun = a.funcionariocodfun
GROUP BY f.nomefun;

--------------------------------------------------------------------------------------------
--Consulta: Serviços Mais Realizados
SELECT s.nomeserv, COUNT(hs.codhistorico) AS total_servicos
FROM servico s
JOIN historico_servico hs ON s.codserv = hs.servicocodserv
GROUP BY s.nomeserv
ORDER BY total_servicos DESC;
```
## 🎲Script de Consultas solicitadas pelo Professor
```sql
-- Clientes com idade abaixo de 40 anos e sexo masculino, ordenados pelo nome descendente
SELECT nomcli, dtnascli
FROM cliente
WHERE sexocli = 'Masculino' AND date_part('year', age(current_date, dtnascli)) < 40
ORDER BY nomcli DESC;

------------------------------------------------------------------------------------------------------------------------------------------------
--Serviços registrados em meses sem a letra 'o' no final e de clientes nos bairros Centro e Agostini, ordenados pelo nome do cliente descendente
SELECT cli.nomcli, ser.nomeserv, to_char(hs.data_hora, 'Month') AS mes
FROM cliente cli
JOIN agendamento ag ON cli.codcli = ag.clientecodcli
JOIN historico_servico hs ON ag.codagen = hs.codhistorico
JOIN servico ser ON hs.servicocodserv = ser.codserv
WHERE cli.bairrocli IN ('Centro', 'Agostini')
  AND to_char(hs.data_hora, 'Month') !~ 'o$'
ORDER BY cli.nomcli DESC;

------------------------------------------------------------------------------------------------------------------------------------------------
-- Agendamentos de clientes com menos de 20 anos das cidades especificadas, ordenados por número de agendamentos por cidade
SELECT cli.cidadecli, COUNT(*) AS num_agendamentos
FROM cliente cli
JOIN agendamento ag ON cli.codcli = ag.clientecodcli
WHERE date_part('year', age(current_date, cli.dtnascli)) < 20
  AND cli.cidadecli IN ('Maravilha', 'Descanso', 'Itapiranga', 'Guaraciaba')
GROUP BY cli.cidadecli
ORDER BY num_agendamentos DESC;

------------------------------------------------------------------------------------------------------------------------------------------------
-- Total de serviços e valor total realizados por mês em 2024, ordenado do maior valor para o menor valor
SELECT to_char(data_hora, 'Month') AS mes,
       COUNT(*) AS total_servicos,
       SUM(ps.valor) AS valor_total
FROM pagamento ps
JOIN agendamento ag ON ps.agendamentocodagen = ag.codagen
WHERE date_part('year', ag.data_hora) = 2024
GROUP BY mes
ORDER BY valor_total DESC;



```

## 🎲Script de Exclusão das Tabelas
```sql
--Possuem chaves estrangeiras
DROP TABLE IF EXISTS historico_servico CASCADE;
DROP TABLE IF EXISTS pagamento CASCADE;
DROP TABLE IF EXISTS agendamento CASCADE;
DROP TABLE IF EXISTS produto CASCADE;

--tabelas referenciadas pelas anteriores
DROP TABLE IF EXISTS servico CASCADE;
DROP TABLE IF EXISTS funcionario CASCADE;
DROP TABLE IF EXISTS cliente CASCADE;
DROP TABLE IF EXISTS fornecedor CASCADE;
```
## 🎲SQL para Relatórios (com Views e Joins)
```
-- View para visualizar agendamentos com informações do cliente e funcionário
create view view_agendamentos_completos as
select ag.codagen, ag.data_hora, ag.status, cl.nomcli, cl.telcli, fn.nomefun
from agendamento ag
join cliente cl on ag.clientecodcli = cl.codcli
join funcionario fn on ag.funcionariocodfun = fn.codfun;

-- View para visualizar pagamentos com detalhes do cliente e agendamento
create view view_pagamentos as
select pg.codpag, pg.valor, pg.data_hora_pagamento, pg.forma_pagamento, cl.nomcli, ag.data_hora
from pagamento pg
join cliente cl on pg.clientecodcli = cl.codcli
join agendamento ag on pg.agendamentocodagen = ag.codagen;

```

## 🎲Scripts de Criação do Banco de Dados e Índices
```
-- Índices para otimização
create index idx_cliente_nome on cliente(nomcli);
create index idx_fornecedor_nome on fornecedor(nomeforn);
create index idx_funcionario_nome on funcionario(nomefun);
create index idx_servico_nome on servico(nomeserv);

```

## 🎲Políticas de Acesso
```
-- Criação de usuários e grupos
create role gerente with login password 'senha_gerente';
create role atendente with login password 'senha_atendente';

-- Privilégios para gerente
grant all privileges on all tables in schema public to gerente;
grant select, insert, update, delete on all tables in schema public to atendente;

```
## 🎲Gatilhos (Triggers)
```
-- Trigger para garantir que a quantidade de produtos nunca seja negativa
create or replace function verificar_quantidade_produto()
returns trigger as $$
begin
    if new.qtdprod < 0 then
        raise exception 'A quantidade de produto não pode ser negativa.';
    end if;
    return new;
end;
$$ language plpgsql;

create trigger trg_verificar_quantidade_produto
before insert or update on produto
for each row
execute function verificar_quantidade_produto();

-- Trigger de auditoria de agendamentos
create or replace function auditoria_agendamento()
returns trigger as $$
begin
    insert into historico_servico (data_hora, servicocodserv, clientecodcli, funcionariocodfun)
    values (now(), new.servicocodserv, new.clientecodcli, new.funcionariocodfun);
    return new;
end;
$$ language plpgsql;

create trigger trg_auditoria_agendamento
after insert on agendamento
for each row
execute function auditoria_agendamento();

```
## 🎲Políticas e Configuração de Backup e Restore
```
--Backup
pg_dump -U nome_usuario -F c -b -v -f /caminho/do/backup/devbarbershop.bak devbarbershop

--Restaurar Backup
pg_restore -U nome_usuario -d devbarbershop -v /caminho/do/backup/devbarbershop.bak

```

## 🧠Desenvolvedor
| [<img src="https://avatars.githubusercontent.com/u/128015032?v=4" width=115><br><sub>Johnny Matheus Nogueira de Medeiro</sub>](https://github.com/JohnnyMatheus) |
| :---: 

## 🔷Professores
| [<img src="https://avatars.githubusercontent.com/u/20915745?v=4" width=115><br><sub>Otília Donato Barbosa</sub>](https://github.com/otiliadb) | [<img src="https://avatars.githubusercontent.com/u/1161348?v=4" width=115><br><sub>Roberson Alves</sub>](https://github.com/robersonjfa) |
| :---: | :---: |





