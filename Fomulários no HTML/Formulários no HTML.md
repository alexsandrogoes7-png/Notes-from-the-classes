# 📌 HTML Forms

- Servem para capturar dados do usuário.
- Muito usados em:
    - login
    - cadastro
    - pesquisas
    - uploads
- Permitem comunicação entre usuário, front-end e back-end.

---

# 📌 Estrutura do formulário

```
<form action="/" method="POST">  <input type="text" name="nome">  <button type="submit">Enviar</button></form>
```

---

# 📌 Tag `<form>`

## 🔹 `action`

- Define para onde os dados serão enviados.

## 🔹 `method`

- Define como os dados serão enviados.

### `GET`

- Dados aparecem na URL.
- Muito usado em buscas e filtros.

### `POST`

- Dados enviados ocultos.
- Mais seguro.
- Muito usado para:
    - login
    - senhas
    - uploads

---

# 📌 Botões (`<button>`)

## 🔹 `submit`

- Envia formulário.

## 🔹 `reset`

- Limpa os campos.

## 🔹 `button`

- Botão comum.
- Geralmente usado com JavaScript.

---

# 📌 Input (`<input>`)

- Campo de entrada de dados.
- O comportamento muda conforme o `type`.

---

# 📌 Atributos gerais do Input

## 🔹 `name`

- Nome do dado enviado.

## 🔹 `value`

- Valor padrão do campo.

## 🔹 `placeholder`

- Texto de dica.
- Não envia valor.

## 🔹 `required`

- Campo obrigatório.

## 🔹 `readonly`

- Apenas leitura.

## 🔹 `disabled`

- Campo desabilitado.

## 🔹 `autofocus`

- Campo inicia focado.

## 🔹 `autocomplete`

- Navegador sugere preenchimento.

## 🔹 `form`

- Liga input a formulário externo.

---

# 📌 Input `text`

- Campo de texto simples.

---

# 📌 Input `number`

- Campo numérico.

## 🔹 `min`

- Valor mínimo.

## 🔹 `max`

- Valor máximo.

## 🔹 `step`

- Intervalo entre números.

---

# 📌 Input `email`

- Faz validação básica de e-mail.

## 🔹 `multiple`

- Permite vários e-mails.

## 🔹 `minlength`

- Quantidade mínima de caracteres.

## 🔹 `maxlength`

- Limite máximo.

## 🔹 `pattern`

- Validação com expressão regular.

## 🔹 `title`

- Mensagem explicativa da validação.

---

# 📌 Expressão Regular (`pattern`)

- Define padrões obrigatórios de texto.
- Muito usado para:
    - e-mails
    - senhas
    - formatos específicos

---

# 📌 Input `password`

- Oculta caracteres digitados.

## 🔹 Segurança

- Preferir `POST`.
- Evitar envio via `GET`.

## 🔹 Recursos

- `minlength`
- `maxlength`
- `pattern`
- `inputmode`

---

# 📌 Input `file`

- Upload de arquivos.

## 🔹 Importante

```
enctype="multipart/form-data"
```

## 🔹 Recursos

### `multiple`

- Permite vários arquivos.

### `accept`

- Restringe tipos permitidos.

## 🔹 Exemplos

```
accept="image/*"accept="video/*"accept=".pdf"
```

---

# 📌 Input `range`

- Controle deslizante (_slider_).

## 🔹 Recursos

- `min`
- `max`
- `step`
- `value`

---

# 📌 Input `color`

- Abre seletor de cores.

## 🔹 `value`

- Cor inicial.

## 🔹 `list` + `datalist`

- Permite sugestões de cores pré-definidas.

---

# 📌 Input `checkbox`

- Permite múltiplas seleções.

## 🔹 Comportamento

- Marcado → envia valor.
- Desmarcado → não envia.

## 🔹 Recursos

- `checked`
- `value`

---

# 📌 Input `radio`

- Permite apenas uma seleção por grupo.

## 🔹 Funcionamento

- Inputs com mesmo `name` pertencem ao mesmo grupo.

---

# 📌 Input `hidden`

- Campo invisível.
- Muito usado para:
    - IDs
    - tokens
    - informações internas

---

# 📌 Label (`<label>`)

- Associa descrição ao campo.

## 🔹 Importância

- Fundamental para acessibilidade.
- Leitores de tela utilizam labels.

## 🔹 Associação

### `for`

- Liga label ao `id` do input.

### Alternativa

- Input pode ficar dentro do próprio label.

---

# 📌 Textarea (`<textarea>`)

- Campo para textos longos.

## 🔹 Recursos

- `maxlength`
- `minlength`
- `placeholder`
- `required`
- `wrap="off"`

## 🔹 Observação

- `rows` e `cols` existem, mas CSS costuma ser preferido.

---

# 📌 Select (`<select>`)

- Campo de seleção de opções.

## 🔹 Recursos

### `option`

- Define opções.

### `multiple`

- Permite múltiplas escolhas.

### `size`

- Quantidade visível de opções.

### `optgroup`

- Agrupa opções relacionadas.

---

# 📌 Fieldset (`<fieldset>`)

- Agrupa campos relacionados.

## 🔹 `legend`

- Título do agrupamento.

## 🔹 `disabled`

- Desabilita todos os campos internos.

## 🔹 Observação

- Campos desabilitados não são enviados.

---

# 📌 Compatibilidade e documentação

## 🔹 Documentação

- [MDN Web Docs](https://developer.mozilla.org/?utm_source=chatgpt.com)
- [DevDocs](https://devdocs.io/?utm_source=chatgpt.com)

## 🔹 Compatibilidade entre navegadores

- [Can I Use](https://caniuse.com/?utm_source=chatgpt.com)

---

# 📌 Ideia central

- HTML Forms capturam e enviam dados do usuário.
- Inputs possuem vários tipos e validações nativas.
- HTML resolve validações básicas sem JavaScript.
- CSS melhora aparência.
- JavaScript adiciona comportamentos e validações avançadas.