# Resumo das aulas — Projeto Portal de Notícias (Setup + Style Guide)

## 1. Início do projeto
Foi criada a estrutura inicial do projeto para estudar **CSS Grid** em um cenário real (portal de notícias com várias seções e cards). A organização inclui: pasta do projeto, `index.html`, pasta `styles` e os arquivos `index.css` e `global.css`.

O `index.css` funciona como ponto de entrada dos estilos, importando o arquivo global, enquanto no HTML é necessário linkar apenas ele. Também foi utilizado o plugin **Live Preview** no Visual Studio Code para visualizar alterações em tempo real, facilitando o desenvolvimento.

---

## 2. Organização dos estilos
A estrutura do CSS foi pensada para manter o código organizado e escalável. O `global.css` concentra regras globais (reset, variáveis e estilos reutilizáveis), enquanto o `index.css` serve como agregador dos estilos.

Foi aplicado um reset básico para remover margens e espaçamentos padrões do navegador e garantir previsibilidade no layout usando `box-sizing: border-box`.

---

## 3. Variáveis CSS (Style Guide)
Foi iniciado o style guide com variáveis CSS, geralmente definidas no `:root`, para armazenar cores do projeto como brand, texto e tons neutros.

O objetivo é centralizar o controle visual da aplicação, permitindo mudanças rápidas e consistentes em todo o layout apenas alterando os valores dessas variáveis.

---

## 4. Aplicação das variáveis
As variáveis criadas foram aplicadas no `body` usando `var()`, definindo cor de texto e cor de fundo da página.

Isso garante padronização visual e facilita manutenção futura, já que qualquer alteração de cor pode ser feita diretamente nas variáveis, sem precisar modificar vários pontos do código.