# 📋 Banco de Dados - Clientes

Este projeto SQL representa um banco de dados básico para gerenciamento de informações de clientes, incluindo dados pessoais e localização.

## 💾 Banco de Dados: `Clientes`

### 🧾 Tabela: `Clientes`

| Campo       | Tipo           | Descrição                       |
|-------------|----------------|----------------------------------|
| id_cliente  | INT (PK)       | Identificador único do cliente  |
| nome        | VARCHAR(100)   | Nome completo                   |
| idade       | INT            | Idade do cliente                |
| email       | VARCHAR(100)   | E-mail                          |
| cidade      | VARCHAR(50)    | Cidade                          |

### 🔽 Dados Iniciais

```sql
insert into Clientes (nome, idade, email, cidade) values
('Maria Silva', 28, 'maria@gmail.com', 'Florianópolis'),
('João Souza', 35, 'joao@hotmail.com', 'São Paulo'),
('Ana Lima', 22, 'ana@gmail.com', 'Rio de Janeiro'),
('Carlos Mendes', 40, 'carlos@yahoo.com', 'São Paulo'),
('Julia Rocha', 30, 'julia@gmail.com', 'Curitiba');

🔍 Consultas SQL
Letra	Consulta
A	select * from Clientes;
B	select nome, idade from Clientes;
C	select * from Clientes where cidade like 'São%';
D	select * from Clientes where idade <= 25;
E	select * from Clientes where idade between 30 and 40;
F	select * from Clientes order by idade asc;
G	select COUNT(*) as total_clientes from Clientes;
H	select cidade, COUNT(*) as total_clientes from Clientes group by cidade;
