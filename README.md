# 📚 Sistema de Banco de Dados – Biblioteca

Este projeto implementa um banco de dados completo para uma **biblioteca**, utilizando **SQLite**.  
Inclui criação de tabelas, inserção de dados, consultas, atualizações e exclusões exigidas no projeto.

---

## 🗂️ Tabelas Criadas

### **categoria**
- `id_categoria` (PK)
- `nome`

### **livro**
- `id_livro` (PK)
- `titulo`
- `autor`
- `quantidade`
- `id_categoria` (FK → categoria)

### **leitor**
- `id_leitor` (PK)
- `nome`
- `email`

### **funcionario**
- `id_funcionario` (PK)
- `nome`
- `cargo`

### **emprestimo**
- `id_emprestimo` (PK)
- `data_emprestimo`
- `data_prevista`
- `id_livro` (FK)
- `id_leitor` (FK)
- `id_funcionario` (FK)

### **devolucao**
- `id_devolucao` (PK)
- `data_devolucao`
- `id_emprestimo` (FK)

---

## ▶️ Como Executar o Projeto

1. Abra o **DB Browser for SQLite**.  
2. Crie um banco novo (`.db`) ou abra um existente.  
3. Vá na aba **Execute SQL**.  
4. Execute o script **01_create_tables.sql**.  
5. Execute os demais arquivos na ordem que quiser:
   - `02_insert_data.sql`
   - `03_select_queries.sql`
   - `04_update_commands.sql`
   - `05_delete_commands.sql`

---

## 🧪 O que foi implementado

### ✔️ DDL
- Criação de todas as tabelas com PK, FK e `PRAGMA foreign_keys = ON`.

### ✔️ INSERT
- População das tabelas principais com dados coerentes.

### ✔️ SELECT
Consultas utilizando:
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `JOIN`

### ✔️ UPDATE
- Pelo menos **3 atualizações** com condições.

### ✔️ DELETE
- Pelo menos **3 exclusões** com `WHERE`, respeitando chaves estrangeiras.

---

## 🎯 Objetivo do Projeto

- Praticar criação e manipulação de dados com SQL.  
- Trabalhar com integridade referencial.  
- Executar operações DML completas (INSERT, SELECT, UPDATE, DELETE).  
- Organizar os scripts em um repositório GitHub para avaliação.
