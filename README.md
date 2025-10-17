# Sistema de Banco de Dados Hospitalar (SQLite)

## 🎯 Visão Geral

Você foi contratado como **Analista de Banco de Dados** para desenvolver o sistema de banco de dados de um hospital, utilizando **SQLite** (por exemplo, via DB Browser). O objetivo é suportar operações clínico-administrativas básicas, como cadastro de pacientes, médicos e agendamento de consultas, além de permitir consultas e relatórios úteis.

---

## 🏥 Estrutura do Banco de Dados

O modelo inicial utiliza **três tabelas principais**:

- **Paciente**: armazena informações dos pacientes.
- **Medico**: armazena informações dos médicos.
- **Consulta**: registra as consultas realizadas, associando pacientes e médicos.

### 📋 Estrutura das Tabelas

| Tabela     | Colunas                                                                 |
|------------|-------------------------------------------------------------------------|
| **Paciente** | `paciente_id` (INTEGER, PK), `nome` (TEXT), `data_nascimento` (TEXT), `sexo` (TEXT), `telefone` (TEXT), `endereco` (TEXT) |
| **Medico**   | `medico_id` (INTEGER, PK), `nome` (TEXT), `especialidade` (TEXT), `telefone` (TEXT), `email` (TEXT) |
| **Consulta** | `consulta_id` (INTEGER, PK), `data_consulta` (TEXT), `horario` (TEXT), `status` (TEXT), `paciente_id` (INTEGER, FK), `medico_id` (INTEGER, FK) |

---

## 📁 Estrutura de Arquivos


/projeto-hospital
│
├── README.md
├── 01_create_tables.sql
├── 02_insert_data.sql
├── 03_select_all_pacientes.sql
├── 04_select_consultas_paciente.sql
├── 05_select_consultas_medico_periodo.sql


- **01_create_tables.sql**: comandos `CREATE TABLE` para criar as tabelas.
- **02_insert_data.sql**: comandos `INSERT` para popular as tabelas com dados de exemplo.
- **03_select_all_pacientes.sql**: consulta para listar todos os pacientes.
- **04_select_consultas_paciente.sql**: consulta para listar todas as consultas de um paciente específico.
- **05_select_consultas_medico_periodo.sql**: consulta para listar todas as consultas de um médico em um determinado período.

---

## 🛠 Instruções de Uso

1. Clone ou baixe este repositório no seu computador.
2. Abra o **DB Browser for SQLite** (ou outra ferramenta compatível).
3. BOA SORTE !!!


