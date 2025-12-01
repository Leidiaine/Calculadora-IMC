# 🌿 Projeto Viver Bem – Banco de Dados Completo  
Mini-mundo | DER | Modelo Lógico | SQL (DML)

Este repositório contém o desenvolvimento completo do projeto de banco de dados do mini-mundo **Viver Bem**, um sistema voltado ao acompanhamento de saúde, bem-estar e hábitos saudáveis dos usuários.

O projeto segue todas as etapas solicitadas pela disciplina:  
✔ Minimundo  
✔ DER (Modelo Conceitual)  
✔ Modelo Lógico  
✔ Normalização até 3FN  
✔ Scripts SQL (Criação, Inserção, Consultas, Atualizações e Remoções)  
✔ Estrutura organizada e versionada

---

## 📌 1. Mini-mundo – “Viver Bem”

O sistema Viver Bem permite que **usuários participem de programas de saúde**, realizem **consultas com profissionais** e registrem **hábitos diários** como peso, hidratação e sono.

Profissionais podem **orientar programas** e realizar acompanhamentos.

---

## 📌 2. Estrutura de Arquivos do ---

## 📌 3. Modelo Conceitual (DER)

O DER representa graficamente:

- Usuário  
- Profissional  
- Programa  
- Participação  
- Consulta  
- Acompanhamento  
- Profissional_Programa

➡ Se quiser, posso incluir aqui a **imagem do DER**.

---

## 📌 4. Modelo Lógico (Tabelas Resultantes)

### Entidades Principais:

- **USUARIO (id_usuario, nome, email, data_nascimento)**
- **PROFISSIONAL (id_profissional, nome, especialidade, telefone)**
- **PROGRAMA (id_programa, nome, objetivo, duracao_semanas)**
- **PARTICIPACAO (id_participacao, id_usuario*, id_programa*, data_inicio)**
- **CONSULTA (id_consulta, data_consulta, id_usuario*, id_profissional*, anotacoes)**
- **ACOMPANHAMENTO (id_acompanhamento, data_registro, peso, horas_sono, agua_ml, id_participacao*)**
- **PROFISSIONAL_PROGRAMA (id_prof_programa, id_profissional*, id_programa*, papel)**

(*) chaves estrangeiras.

---

## 📌 5. Scripts SQL do Projeto

Todos os scripts seguem o padrão MySQL.

### ▶ 01_create_tables.sql  
Criação do banco e das tabelas com chaves primárias e estrangeiras.

### ▶ 02_insert_data.sql  
Inserção de dados reais e coerentes com o mini-mundo.

### ▶ 03_select_queries.sql  
Consultas com:
- WHERE  
- ORDER BY  
- JOIN  
- LIMIT  

### ▶ 04_update.sql  
3 atualizações reais no banco.

### ▶ 05_delete.sql  
3 deleções a partir de condições específicas.

---

## 📌 6. DML – Exemplos presentes nos scripts

### ✔ INSERT  
Registros completos para todas as tabelas.

### ✔ SELECT  
Consultas com JOIN triplo, filtros por data, ordenação e limite.

### ✔ UPDATE  
Atualizações de e-mail, telefone e objetivo de programas.

### ✔ DELETE  
Remoção de registros com integridade preservada.

---

## 📌 7. Normalização (até 3FN)

O modelo foi normalizado até a 3ª Forma Normal:

1. **1FN:** todos os atributos são atômicos.  
2. **2FN:** tabelas de associações criadas para eliminar dependências parciais.  
3. **3FN:** nenhuma dependência transitiva entre atributos não-chave.

---

## 📌 8. Como Executar no Workbench ou PGAdmin

1. Abra o **01_create_tables.sql**  
2. Execute para criar o banco  
3. Rode o **02_insert_data.sql**  
4. Teste consultas com **03_select_queries.sql**  
5. Teste alterações e remoções com **04_update.sql** e **05_delete.sql**

---

## 📌 9. Tecnologias

- MySQL Workbench **ou**  
- PostgreSQL (PGAdmin)  
- GitHub para versionamento  

---

## 📌 10. Autor  
Projeto criado para fins acadêmicos na disciplina de Modelagem e Banco de Dados.

---

## 📌 11. Licença  
Este projeto está sob licença livre para fins ---

## 📌 3. Modelo Conceitual (DER)

O DER representa graficamente:

- Usuário  
- Profissional  
- Programa  
- Participação  
- Consulta  
- Acompanhamento  
- Profissional_Programa

➡ Se quiser, posso incluir aqui a **imagem do DER**.

---

## 📌 4. Modelo Lógico (Tabelas Resultantes)

### Entidades Principais:

- **USUARIO (id_usuario, nome, email, data_nascimento)**
- **PROFISSIONAL (id_profissional, nome, especialidade, telefone)**
- **PROGRAMA (id_programa, nome, objetivo, duracao_semanas)**
- **PARTICIPACAO (id_participacao, id_usuario*, id_programa*, data_inicio)**
- **CONSULTA (id_consulta, data_consulta, id_usuario*, id_profissional*, anotacoes)**
- **ACOMPANHAMENTO (id_acompanhamento, data_registro, peso, horas_sono, agua_ml, id_participacao*)**
- **PROFISSIONAL_PROGRAMA (id_prof_programa, id_profissional*, id_programa*, papel)**

(*) chaves estrangeiras.

---

## 📌 5. Scripts SQL do Projeto

Todos os scripts seguem o padrão MySQL.

### ▶ 01_create_tables.sql  
Criação do banco e das tabelas com chaves primárias e estrangeiras.

### ▶ 02_insert_data.sql  
Inserção de dados reais e coerentes com o mini-mundo.

### ▶ 03_select_queries.sql  
Consultas com:
- WHERE  
- ORDER BY  
- JOIN  
- LIMIT  

### ▶ 04_update.sql  
3 atualizações reais no banco.

### ▶ 05_delete.sql  
3 deleções a partir de condições específicas.

---

## 📌 6. DML – Exemplos presentes nos scripts

### ✔ INSERT  
Registros completos para todas as tabelas.

### ✔ SELECT  
Consultas com JOIN triplo, filtros por data, ordenação e limite.

### ✔ UPDATE  
Atualizações de e-mail, telefone e objetivo de programas.

### ✔ DELETE  
Remoção de registros com integridade preservada.

---

## 📌 7. Normalização (até 3FN)

O modelo foi normalizado até a 3ª Forma Normal:

1. **1FN:** todos os atributos são atômicos.  
2. **2FN:** tabelas de associações criadas para eliminar dependências parciais.  
3. **3FN:** nenhuma dependência transitiva entre atributos não-chave.

---

## 📌 8. Como Executar no Workbench ou PGAdmin

1. Abra o **01_create_tables.sql**  
2. Execute para criar o banco  
3. Rode o **02_insert_data.sql**  
4. Teste consultas com **03_select_queries.sql**  
5. Teste alterações e remoções com **04_update.sql** e **05_delete.sql**

---

## 📌 9. Tecnologias

- MySQL Workbench **ou**  
- PostgreSQL (PGAdmin)  
- GitHub para versionamento  

---

## 📌 10. Autor  
Projeto criado para fins acadêmicos na disciplina de Modelagem e Banco de Dados.

---

## 📌 11. Licença  
Este projeto está sob licença livre para fins educacionais.
