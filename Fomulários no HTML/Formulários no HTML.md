### 📌 HTML Forms

- HTML Forms servem para **capturar dados do usuário**.
- Muito usados em:
    - login
    - cadastro
    - pesquisas
    - formulários
    - calculadoras
- Permitem interação entre usuário e página web.

---

### 📌 Input e Output

- **Input:** entrada de dados.
- **Output:** saída/apresentação dos dados.

Exemplo:

- Digitar nome → input
- Mostrar resultado → output

---

### 📌 Estrutura básica do formulário

```
<form action="/" method="GET">  <input type="text" name="nome">  <button type="submit">    Enviar  </button></form>
```

---

### 📌 Tag `<form>`

- Elemento responsável por criar formulários.
- Possui atributos importantes:
    - `action`
    - `method`

---

### 📌 Action

- Define **para onde os dados serão enviados**.

```
<form action="/">
```

- Se não definir:
    - o formulário envia para a própria página.

---

### 📌 Method

- Define **como os dados serão enviados**.
- Usa verbos HTTP.

---

### 📌 GET

```
<form method="GET">
```

- Dados aparecem na URL.
- Método padrão do formulário.

Exemplo:

```
site.com?nome=Mike
```

#### 🔹 Características

- Dados visíveis
- Muito usado em:
    - buscas
    - filtros
    - pesquisas

---

### 📌 POST

```
<form method="POST">
```

#### 🔹 Características

- Dados não aparecem na URL.
- Método mais seguro.
- Muito usado em:
    - login
    - senha
    - cadastro

---

### 📌 HTTP

- HTTP é um protocolo de comunicação da web.
- Possui verbos como:
    - GET
    - POST

---

### 📌 Live Preview no VS Code

- Professor utilizou a extensão Live Preview.
- Ela:
    - cria um servidor local
    - mostra pré-visualização da página
    - facilita testes em tempo real

---

### 📌 Tag `<button>`

- Cria botões interativos no HTML.

```
<button>Enviar</button>
```

- O estilo depende do navegador.

---

### 📌 Tipos de botão

#### 🔹 submit

```
<button type="submit">  Enviar</button>
```

- Envia o formulário.
- É o tipo padrão.

---

#### 🔹 reset

```
<button type="reset">  Limpar</button>
```

- Limpa os campos do formulário.

---

#### 🔹 button

```
<button type="button">  Clique</button>
```

- Botão comum.
- Não envia formulário.
- Geralmente usado com JavaScript.

---

### 📌 autofocus

```
<button autofocus>  Entrar</button>
```

- Coloca foco automático no elemento ao carregar a página.
- Nem todos os navegadores aplicam igual.

---

### 📌 disabled

```
<button disabled>  Bloqueado</button>
```

- Desativa o botão.
- Muito usado para impedir envio antes do preenchimento correto.

---

### 📌 name e value no botão

```
<button  name="botao1"  value="enviar">  Submit</button>
```

Exemplo enviado pela URL:

```
?botao1=enviar
```

#### 🔹 Utilidade

- Identificar qual botão foi clicado.
- Enviar informações extras no formulário.

---

### 📌 Ideia central

- Forms permitem comunicação entre:
    - front-end
    - usuário
    - back-end
- São fundamentais para capturar e enviar dados na web.