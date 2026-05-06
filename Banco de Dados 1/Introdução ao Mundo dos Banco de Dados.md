


### 📌 Introdução e professor

- Professor com experiência prática (desenvolvedor há +5 anos) e acadêmica (graduação, mestrado e doutorado).
- Curso vai do **básico ao avançado** em banco de dados, com foco prático.

---

### 📌 O que é banco de dados

- É uma **coleção organizada de informações**.
- Permite **armazenar, acessar, atualizar e gerenciar dados** facilmente.
- Exemplo: agenda de contatos ou planilha.

---

### 📌 Conceitos básicos

- **Dados:** informações brutas (números, textos).
- **Informação:** dados organizados com sentido.
- **Tabela:** estrutura do banco.
- **Registro (linha):** um item (ex: um usuário).
- **Campo (coluna):** atributo (nome, email, etc.).

---

### 📌 SGBD (Sistema Gerenciador de Banco de Dados)

- Software que gerencia o banco.
- Exemplos: PostgreSQL, MySQL, MongoDB.
- Permite **criar, acessar e manipular dados**.

---

### 📌 Como funciona (estrutura)

- Banco fica em um **servidor (hardware)**.
- Acesso é feito via **software** (apps ou código).
- Usuário interage com o sistema que consulta o banco.

---

### 📌 Importância dos bancos de dados

- **Rapidez:** acesso em milissegundos.
- **Segurança:** dados protegidos e consistentes.
- **Escalabilidade:** suporta sistemas grandes.

---

### 📌 Exemplos do dia a dia

- Spotify → músicas e recomendações
- Netflix → histórico e sugestões
- Instagram → fotos, curtidas, comentários
- Apps bancários e delivery também usam bancos de dados

---

### 📌 Tipos de banco de dados

#### 🔹 Relacional (SQL)

- Usa **tabelas (linhas e colunas)**.
- Estrutura fixa e organizada.
- Linguagem: SQL.
- Possui **relacionamentos entre tabelas** (chaves).

#### 🔹 Não relacional (NoSQL)

- Estrutura **flexível**.
- Pode usar JSON, chave-valor, grafos.
- Ex: MongoDB, Firebase.

---

### 📌 Diferença principal

- **Relacional:** organizado e estruturado (tipo planilha).
- **Não relacional:** flexível e menos rígido.

---

### 📌 Ideia central

- Bancos de dados estão **em tudo no mundo digital**.
- São essenciais para **organizar, armazenar e recuperar informações com eficiência**.
  
  ### 📌 SQL e PostgreSQL

- SQL é a linguagem usada para **interagir com bancos de dados relacionais**.
- PostgreSQL é um dos SGBDs mais usados no mercado.

---

### 📌 O que é SQL

- **Structured Query Language** (linguagem de consulta estruturada).
- Serve para:
    - Consultar dados
    - Criar estruturas
    - Manipular informações

👉 É a “linguagem de comunicação” com o banco de dados.

---

### 📌 O que dá pra fazer com SQL

- Criar tabelas
- Inserir dados
- Consultar dados
- Atualizar dados
- Deletar dados

---

### 📌 Principais comandos

- **CREATE TABLE** → cria tabela
- **INSERT INTO** → insere dados
- **SELECT** → consulta dados
- **UPDATE** → atualiza dados
- **DELETE** → remove dados

---

### 📌 Exemplos (ideia geral)

- Criar tabela:

```
CREATE TABLE usuarios (  id SERIAL PRIMARY KEY,  nome VARCHAR(100),  email VARCHAR(100));
```

- Inserir dados:

```
INSERT INTO usuarios (nome, email)VALUES ('Ana Silva', 'ana@email.com');
```

- Consultar:

```
SELECT * FROM usuarios;
```

---

### 📌 Ideia principal

- SQL é uma linguagem **simples, poderosa e essencial**.
- Permite **criar, acessar e modificar dados** no banco.
- Dá pra aprender **do zero**, sem precisar de outra linguagem antes.

## 📌 O que é PostgreSQL

- SGBD relacional **open source**
- Gratuito, robusto e seguro
- Usa **SQL padrão** (aprendizado reaproveitável)
- Suporta dados complexos (JSON, arrays, geográficos)
- Comunidade grande + ótima documentação

👉 Ideia-chave:  
**“PostgreSQL = banco completo (tipo canivete suíço)”**

---

## 📌 Ferramentas usadas

### 1. pgAdmin (nativo)

- Interface oficial do PostgreSQL
- Usado para:
    - Criar banco
    - Criar tabelas
    - Gerenciar dados

👉 Só funciona com PostgreSQL

---

### 2. Beekeeper Studio (genérico)

- Interface gráfica universal
- Conecta com:
    - PostgreSQL
    - MySQL
    - MongoDB
    - etc.

👉 Ideia-chave:  
**“pgAdmin = específico | Beekeeper = genérico”**

---

## 📌 Configuração da conexão

Dados padrão que SEMPRE caem:

- Host: `localhost`
- Porta: `5432`
- Usuário: `postgres`
- Senha: (definida na instalação)

👉 localhost = sua própria máquina  
👉 5432 = porta padrão do Postgre

---

## 📌 Criar banco de dados (SQL)

Comando essencial:

```
CREATE DATABASE agenda;
```

👉 Quebra mental:

- CREATE = criar
- DATABASE = banco
- agenda = nome

---

## 📌 Criar tabela (SQL)

Exemplo:

```
CREATE TABLE contatos (  id SERIAL PRIMARY KEY,  nome VARCHAR(100),  telefone VARCHAR(20));
```

👉 Ideias importantes:

- `SERIAL` = auto incremento
- `PRIMARY KEY` = identificador único
- `VARCHAR(n)` = texto com limite

---

## 📌 Conceitos que apareceram

- **Query** = comando SQL
- Executar só parte do código → _Run Selection_
- Sempre dar **refresh** pra ver alterações
- Banco não pode ter nomes duplicados

---

## 📌 Fluxo completo (decora isso)

1. Instala PostgreSQL
2. Abre pgAdmin → testa conexão
3. Instala Beekeeper
4. Conecta com:
    - localhost
    - porta 5432
5. Cria banco (`CREATE DATABASE`)
6. Cria tabela (`CREATE TABLE`)