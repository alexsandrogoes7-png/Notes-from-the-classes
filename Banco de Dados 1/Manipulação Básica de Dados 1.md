
# Aula 1 — Criação de Tabelas no PostgreSQL

📌 Nessa aula, o foco foi entender como funcionam tabelas simples no banco de dados, sem relacionamentos. O professor explicou a importância de criar tabelas com estrutura clara, organizada e pensando na futura manutenção do sistema. Também introduziu conceitos como colunas, tipos de dados e boas práticas de modelagem. Ao final, foi mostrado o processo de criação de uma tabela chamada `clientes` no PostgreSQL usando o BKeyper Studio.

📌 Principais pontos

- Tabelas representam entidades do sistema (clientes, produtos, etc.).
- Cada tabela possui colunas com tipos de dados específicos.
- É importante usar nomes padronizados nas tabelas e colunas.
- Boas práticas ajudam na manutenção e expansão do sistema.
- Futuramente as tabelas poderão ter relacionamentos entre si.

📌 Conceitos citados

- Colunas da tabela.
- Tipos de dados (texto, número, data, booleano).
- Restrições (`NOT NULL`, tamanho de campos, etc.).
- Modelagem de banco de dados.
- Chave primária e identificação de registros.

📌 Ferramentas e prática

- Uso do BKeyper Studio.
- Criação de tabela via comando `CREATE TABLE`.
- Exemplo prático com a tabela `clientes`.
  
#  Aula 2 — Estrutura de um Comando CREATE TABLE

📌Nessa aula, foi mostrado como criar tabelas no PostgreSQL usando o BKeyper Studio. O professor explicou o uso do comando `DROP` para excluir tabelas e do `CREATE TABLE` para criar uma nova tabela chamada `clientes`. Também apresentou a ideia de colunas, tipos de dados e algumas restrições básicas usadas na criação das tabelas.

📌 Principais pontos

- Uso do BKeyper Studio para acessar o banco de dados.
- Comando `DROP` remove a tabela e todos os seus dados.
- Comando `CREATE TABLE` cria uma nova tabela.
- Cada tabela possui colunas com tipos de dados específicos.
- A coluna `ID` foi definida como chave primária.

📌 Conceitos citados

- Tipos de dados: `SERIAL`, `VARCHAR`, `DATE`, `NUMERIC`, `BOOLEAN` e `TIMESTAMP`.
- Chave primária (`PRIMARY KEY`) identifica cada registro de forma única.
- `NOT NULL` impede valores vazios.
- `BOOLEAN` trabalha com verdadeiro ou falso.
- `SERIAL` cria valores automáticos em sequência.

📌 Observações importantes

- É importante manter um padrão nos nomes das tabelas e colunas.
- O professor comentou que modelagem e relacionamentos serão vistos mais à frente.
- A aula focou em entender a estrutura básica de uma tabela.


# Aula 3 — Executando O Comando Create Table No Beekeeper

📌Criação e visualização de tabelas no PostgreSQL  
Nessa aula, foi mostrado o processo completo de criação da tabela `clientes` no BKeyper Studio. O professor destacou boas práticas de padronização nos comandos SQL e explicou como visualizar a estrutura e os dados da tabela criada. Também apresentou algumas funcionalidades úteis do BKeyper Studio para gerenciamento das tabelas.

📌 Principais pontos

- Uso de letras maiúsculas para comandos SQL.
- Padronização nos nomes das tabelas e colunas.
- Importância de evitar vírgula na última coluna do `CREATE TABLE`.
- Execução do comando SQL pelo `Run Selection`.
- Visualização da tabela criada no BKeyper Studio.

📌 Conceitos citados

- Estrutura da tabela (`View Structure`).
- Visualização de dados (`View Data`).
- Chave primária (`PRIMARY KEY`).
- Índices e valores únicos (`UNIQUE`).
- Relações e triggers foram mencionadas brevemente.

📌 Funcionalidades do BKeyper Studio

- Atualizar tabelas com `Refresh`.
- Exportar estrutura ou dados.
- Renomear tabelas.
- Excluir tabelas (`DROP`).
- Limpar dados (`TRUNCATE`).

# Aula 4 — Tipos de Dados Numéricos no PostgreSQL

📌 Tipos de Dados Numéricos no PostgreSQL  
Nesta aula, aprendemos os principais tipos de dados do PostgreSQL, focando principalmente nos tipos numéricos. O professor explicou a diferença entre números inteiros e números com casas decimais, além de mostrar quando utilizar cada tipo em situações do dia a dia no desenvolvimento. Também vimos exemplos práticos de uso em tabelas e como definir precisão em valores numéricos.

 📌Pontos principais:

- PostgreSQL possui vários tipos de dados: texto, números, booleano, data, arrays e JSON.
- Números inteiros:
    - `SmallInt` → valores pequenos (ex.: idade).
    - `Integer/Int` → valores médios (ex.: quantidade de produtos).
    - `BigInt` → números muito grandes (ex.: população).
- Números decimais:
    - `Numeric` → alta precisão, muito usado para dinheiro.
    - `Decimal` → útil para percentuais.
    - `Real` → valores menos críticos, como temperatura.
    - `Double Precision` → alta precisão para geolocalização e cálculos complexos.
- É possível definir quantidade máxima de dígitos e casas decimais.
- Os tipos são definidos diretamente nas colunas das tabelas.

# Aula 5 —Tipos de Dados Textuais no PostgreSQL

📌 Tipos de Dados Textuais no PostgreSQL  
Nesta aula, aprendemos os principais tipos textuais do PostgreSQL: `char`, `varchar` e `text`. O professor explicou quando utilizar cada um deles e mostrou exemplos práticos de aplicação em tabelas. Também vimos como definir limites de caracteres e a diferença entre textos fixos, variáveis e ilimitados.

📌 Pontos principais:

- `Char` → usado para textos com tamanho fixo.
    - Ex.: CPF, telefone, siglas de estados ou países.
- `Varchar` → tamanho variável com limite de caracteres.
    - Muito usado para nomes, e-mails e descrições curtas.
- `Text` → utilizado para textos longos e sem limite definido.
    - Ex.: artigos, postagens de blog e descrições extensas.
- É possível definir o tamanho máximo no `char` e no `varchar`.
- O `text` não precisa de definição de limite de caracteres.
- Cada tipo textual deve ser escolhido conforme a necessidade da coluna na tabela.

# Aula 6 —Tipos de Dados Booleanos e Datas/Horas no PostgreSQL

📌 Tipo Boolean e Datas no PostgreSQL  
Nesta aula, aprendemos sobre o tipo `Boolean`, usado para armazenar valores lógicos como verdadeiro (`true`) ou falso (`false`). Também vimos os principais tipos de dados relacionados a data e hora no PostgreSQL, entendendo quando utilizar cada um deles em situações práticas dentro de sistemas.

🔹 Pontos principais:

- `Boolean` armazena apenas:
    - `True` → verdadeiro
    - `False` → falso
    - Pode aceitar `Null` se permitido.
- Muito usado para:
    - Usuário ativo/inativo.
    - Contrato ativo.
    - Permissão de administrador.
- O PostgreSQL utiliza o tipo `boolean` para esses campos.

🔹 Tipos de data e hora:

- `Date` → armazena apenas a data.
    - Ex.: data de nascimento.
- `Time` → armazena apenas horário.
    - Ex.: hora de abertura de um processo.
- `Timestamp` → guarda data e hora sem considerar fuso horário.
- `TimestampTZ` → guarda data e hora considerando o fuso horário.

🔹 Aplicação prática:

- Cada tipo deve ser escolhido conforme a necessidade da informação.
- Esses dados são essenciais para controle e organização em sistemas e bancos de dados.

# Aula 7 —Tipos de Dados UUID e Serial no Postgres

📌 Serial, UUID, Array e JSON no PostgreSQL  
Nesta aula, aprendemos alguns tipos de dados muito utilizados no PostgreSQL. O serial é usado para criar IDs automáticos e sequenciais, enquanto o UUID gera identificadores únicos mais seguros e difíceis de adivinhar. Também vimos o array, que permite armazenar listas de valores, e o JSON/JSONB, utilizado para guardar dados estruturados em formato JSON dentro das tabelas. Esses tipos ajudam a tornar o banco mais flexível e organizado.

🔹 Principais pontos:

- `serial` → IDs automáticos sequenciais.
- `UUID` → identificadores únicos mais seguros.
- `array` → armazenamento de listas de valores.
- `JSON/JSONB` → armazenamento de dados em formato JSON.
- Serial continua a sequência mesmo após exclusões.
- UUID usa letras, números e traços para identificação única.

# Aula 8 — Tipos de Dados Array e JSON no Postgres

📌 Arrays e JSON no PostgreSQL  
Nesta aula, aprendemos sobre os tipos de dados `array` e `JSON` no PostgreSQL. O array permite armazenar listas de valores em um único campo, podendo ser de números ou textos. Já o JSON e JSONB servem para armazenar objetos no formato JSON, sendo o JSONB mais otimizado para buscas e grandes volumes de dados. Esses tipos são úteis quando precisamos trabalhar com estruturas mais flexíveis dentro do banco.

🔹 Principais pontos:

- `array` → armazena listas de valores em um único campo.
- Arrays podem ser de números (`integer[]`) ou textos (`text[]`).
- Valores em arrays são separados por vírgula.
- `JSON` → armazenamento simples em formato JSON.
- `JSONB` → versão otimizada para buscas e filtragens.
- JSONB é mais indicado para grandes volumes de dados.

# Aula 9 —  Estrutura do Comando Insert

📌 Inserindo Dados com INSERT INTO  
Nesta aula, aprendemos como inserir dados em tabelas usando o comando `INSERT INTO` no PostgreSQL. Vimos como definir as colunas e adicionar os valores corretamente, respeitando os tipos de dados e a ordem das informações. Também entendemos que colunas do tipo `serial` não precisam ser preenchidas manualmente, pois o banco gera os IDs automaticamente. Além disso, aprendemos a inserir vários registros de uma só vez, deixando o processo mais rápido e prático.

🔹 Principais pontos:

- `INSERT INTO` é usado para inserir registros em tabelas.
- É necessário informar as colunas e os valores correspondentes.
- A ordem dos valores deve seguir a ordem das colunas.
- Textos ficam entre aspas; números não precisam.
- Colunas `serial` geram IDs automaticamente.
- É possível inserir múltiplos registros em um único comando.

# Aula 10 — Estrutura da Tabela no Beekeeper para Realizar o Comando INSERT

Exemplo completo da tabela `clientes` com os principais tipos de dados no PostgreSQL:

```
-- Habilita extensão para gerar UUID automaticamenteCREATE EXTENSION IF NOT EXISTS "uuid-ossp";-- Criação da tabelaCREATE TABLE clientes (    id SERIAL PRIMARY KEY,    codigo_uuid UUID DEFAULT uuid_generate_v4(),    idade SMALLINT,    quantidade_compras INTEGER,    pontos_acumulados BIGINT,    ticket_medio NUMERIC(10,2),    desconto_medio DECIMAL(5,2),    estado CHAR(2),    nome VARCHAR(100),    observacoes TEXT,    ativo BOOLEAN,    data_nascimento DATE,    hora_cadastro TIME,    criado_em TIMESTAMP,    atualizado_em TIMESTAMPTZ,    notas INTEGER[],    tags TEXT[],    dados_extras JSON,    configuracoes JSONB);
```

Exemplo de INSERT com vários tipos de dados:

```
INSERT INTO clientes (    idade,    quantidade_compras,    pontos_acumulados,    ticket_medio,    desconto_medio,    estado,    nome,    observacoes,    ativo,    data_nascimento,    hora_cadastro,    criado_em,    atualizado_em,    notas,    tags,    dados_extras,    configuracoes)VALUES (    25,    120,    450000,    1599.90,    12.50,    'SP',    'João Silva',    'Cliente premium com histórico positivo.',    TRUE,    '2000-05-10',    '14:30:00',    '2026-05-10 14:30:00',    '2026-05-10 14:30:00-03',    ARRAY[10, 20, 30],    ARRAY['vip', 'premium', 'ativo'],    '{"origem":"site","campanha":"black_friday"}',    '{"tema":"dark","notificacoes":true}');
```

Pontos importantes:

- `SERIAL` → gera IDs automáticos sequenciais.
- `UUID` → gera identificadores únicos mais seguros.
- `SMALLINT`, `INTEGER`, `BIGINT` → números inteiros de tamanhos diferentes.
- `NUMERIC(10,2)` → números decimais precisos, ideal para valores monetários.
- `CHAR(2)` → tamanho fixo, ótimo para siglas de estados.
- `VARCHAR(100)` → texto com limite.
- `TEXT` → texto longo sem limite prático.
- `BOOLEAN` → `TRUE` ou `FALSE`.
- `DATE`, `TIME`, `TIMESTAMP` → controle de datas e horários.
- `INTEGER[]` e `TEXT[]` → arrays/listas.
- `JSON` e `JSONB` → armazenamento estruturado em formato JSON.

Exemplo para visualizar os dados:

```
SELECT * FROM clientes;
```

Exemplo para inserir múltiplos registros:

```
INSERT INTO clientes (    idade,    estado,    nome,    ativo)VALUES    (22, 'SC', 'Maria Souza', TRUE),    (30, 'RS', 'Carlos Lima', FALSE),    (28, 'PR', 'Ana Costa', TRUE);
```

# Aula 11 — Comando Insert No Beekeeper

O comando completo do `INSERT INTO clientes` da aula fica assim:

```
INSERT INTO clientes (    idade,    quantidade_compras,    pontos_acumulados,    ticket_medio,    desconto_medio,    estado,    nome,    observacoes,    ativo,    data_nascimento,    hora_cadastro,    criado_em,    atualizado_em,    notas,    tags,    dados_extras)VALUES (    30,    123,    1500,    250.75,    12.50,    'SP',    'João Silva',    'Cliente premium com histórico positivo.',    TRUE,    '1994-05-10',    '14:30:00',    '2026-05-10 14:30:00',    '2026-05-10 14:30:00-03',    ARRAY[10,20,30],    ARRAY['vip','premium','ativo'],    '{"origem":"site","campanha":"black_friday","ativo":true}');
```

Pontos importantes da aula:

- `id` e `codigo_uuid` NÃO são informados no INSERT:
    - `SERIAL` gera `1,2,3...`
    - `UUID` gera automaticamente códigos únicos.
- Ordem importa:
    - Os valores precisam seguir exatamente a mesma ordem das colunas.
- Tipos numéricos:
    - Inteiros → sem aspas:
        
        ```
        30
        ```
        
    - Decimais → usam ponto:
        
        ```
        250.75
        ```
        
- Textos:
    - Sempre entre aspas simples:
        
        ```
        'João Silva'
        ```
        
- Boolean:
    - Usa `TRUE` ou `FALSE`:
        
        ```
        TRUE
        ```
        
- Datas:
    - Formato:
        
        ```
        'YYYY-MM-DD'
        ```
        
- Hora:
    - Formato:
        
        ```
        'HH:MM:SS'
        ```
        
- Arrays:
    - Inteiros:
        
        ```
        ARRAY[1,2,3]
        ```
        
    - Texto:
        
        ```
        ARRAY['vip','premium']
        ```
        
- JSON:
    - Estrutura com chaves:
        
        ```
        '{"chave":"valor"}'
        ```
        

Comando para visualizar os dados inseridos:

```
SELECT * FROM clientes;
```

Ou no Beekeeper:

- Clique direito na tabela `clientes`
- `View Data`

# Aula 12 — Estrutura do Comando SELECT

O comando `SELECT` é usado para consultar dados armazenados em tabelas SQL.  
Sua estrutura básica é:

```
SELECT coluna1, coluna2FROM nome_tabela;
```

## Estrutura do SELECT

- `SELECT` → define quais colunas serão exibidas.
- `FROM` → informa de qual tabela os dados serão buscados.

Exemplo:

```
SELECT nome, idadeFROM alunos;
```

Nesse caso:

- `nome` e `idade` são as colunas selecionadas.
- `alunos` é a tabela.

---

## Selecionando todas as colunas

Quando queremos trazer todos os dados da tabela, usamos `*`:

```
SELECT *FROM alunos;
```

O `*` significa:

- todas as colunas da tabela.

Isso facilita consultas rápidas, principalmente em testes e estudos.

---

## Cuidados com SELECT *

Apesar de útil, o `SELECT *` deve ser usado com cuidado porque:

- pode trazer dados desnecessários;
- aumenta o processamento;
- consome mais memória;
- pode deixar consultas lentas em tabelas grandes.

Por isso, em sistemas reais, normalmente selecionamos apenas as colunas necessárias.

---

## Exemplo com a tabela clientes

Selecionando apenas algumas colunas:

```
SELECT nome, estado, ativoFROM clientes;
```

Selecionando tudo:

```
SELECT *FROM clientes;
```

---

## Pontos importantes

- Os nomes das colunas devem ser exatamente iguais aos da tabela.
- O SQL respeita a estrutura definida no banco.
- Podemos futuramente adicionar filtros usando `WHERE`.

Exemplo futuro:

```
SELECT nome, idadeFROM alunosWHERE idade >= 18;
```

---

## Resumo

| Comando  | Função                     |
| -------- | -------------------------- |
| `SELECT` | Seleciona dados            |
| `FROM`   | Define a tabela            |
| `*`      | Seleciona todas as colunas |
| `WHERE`  | Filtra registros           |

# Aula 13 — Comando Select No Beekeeper

O comando `SELECT` é usado para consultar dados em tabelas SQL.

## Selecionando todas as colunas

```
SELECT *FROM clientes;
```

- `*` traz todas as colunas da tabela.
- Deve ser usado com cuidado em tabelas grandes.

---

## Selecionando colunas específicas

```
SELECT nome, idade, estadoFROM clientes;
```

- Traz apenas as colunas informadas.
- A ordem das colunas pode ser alterada.

---

## Atenção à vírgula

ERRADO:

```
SELECT nome, idade,FROM clientes;
```

CORRETO:

```
SELECT nome, idadeFROM clientes;
```

---

## No Beekeeper

- `View Data` faz um `SELECT *` automaticamente.
- `Refresh Table` atualiza os dados exibidos.

---

## Resumo

| Comando              | Função              |
| -------------------- | ------------------- |
| `SELECT *`           | Todas as colunas    |
| `SELECT nome, idade` | Colunas específicas |
| `FROM`               | Define a tabela     |
# Aula 14 — Estrutura do Comando Update

O comando `UPDATE` é usado para atualizar registros em uma tabela SQL.

## Estrutura básica

```
UPDATE tabelaSET coluna = novo_valorWHERE condicao;
```

- `UPDATE` → define a tabela que será alterada.
- `SET` → informa os novos valores.
- `WHERE` → filtra quais linhas serão atualizadas.

---

## Exemplo simples

```
UPDATE alunosSET idade = 23WHERE nome = 'Maria Santos';
```

Nesse caso:

- a coluna `idade` será alterada para `23`;
- apenas onde o nome for `'Maria Santos'`.

---

## Atualizando várias colunas

```
UPDATE alunosSET    idade = 23,    email = 'maria@email.com'WHERE nome = 'Maria Santos';
```

- Cada coluna recebe um novo valor.
- As colunas são separadas por vírgula.

---

## Muito cuidado com WHERE

Sem `WHERE`:

```
UPDATE alunosSET idade = 23;
```

Isso atualiza TODAS as linhas da tabela.

Por isso, na maioria dos casos, usamos `WHERE` para evitar alterações em massa.

---

## Resumo

|Comando|Função|
|---|---|
|`UPDATE`|Atualiza registros|
|`SET`|Define novos valores|
|`WHERE`|Filtra linhas específicas|

O `UPDATE` é um dos comandos mais importantes do SQL para manutenção de dados no PostgreSQL.

# Aula 15 — Comando Update No Beekeeper

## Estrutura

```
UPDATE tabelaSET coluna = valorWHERE condicao;
```

---

## Atualizar uma coluna

```
UPDATE clientesSET estado = 'SP'WHERE id = 3;
```

---

## Atualizar várias colunas

```
UPDATE clientesSET    nome = 'Felipe',    ativo = falseWHERE id = 3;
```

---

## Atualizar vários registros

```
UPDATE clientesSET estado = 'RJ'WHERE nome = 'Felipe';
```

---

## Cuidados

- Sem `WHERE` → atualiza TODAS as linhas
- Prefira filtrar por `id` ou `uuid`
- Não usar vírgula no último campo

---

## Resumo

```
UPDATE → tabelaSET → novos valoresWHERE → quais linhas alterar
```

# Aula 15 — Estrutura do Comando DELETE

## Estrutura

```
DELETE FROM tabelaWHERE condicao;
```

---

## Exemplo

```
DELETE FROM alunosWHERE idade < 18;
```

Remove todos os alunos com idade menor que 18.

---

## Deletar um registro específico

```
DELETE FROM clientesWHERE id = 3;
```

---

## Cuidados

- `DELETE` remove a linha inteira
- Sem `WHERE` → apaga TODOS os registros
- Prefira filtrar por `id` ou `uuid`
- Sem backup, os dados podem ser perdidos

---

## ERRADO

```
DELETE FROM clientes;
```


# Aula 16 — Comando Delete No Beekeeper


## Estrutura

```
DELETE FROM tabelaWHERE condicao;
```

---

## Deletar um registro

```
DELETE FROM clientesWHERE id = 4;
```

---

## Deletar vários registros

```
DELETE FROM clientesWHERE nome = 'Felipe';
```

---

## Cuidados

- `DELETE` remove a linha inteira
- Sem `WHERE` → apaga TODOS os registros
- Prefira `id` ou `uuid`
- IDs apagados não voltam

---

## ERRADO

```
DELETE FROM clientes;
```

Apaga todos os registros da tabela.