
# Resumo das aulas — Tipografia + Assets

## 1. Tipografia e fontes
Foi configurada a tipografia do projeto utilizando a fonte **Arquivo** do Google Fonts, importada no `index.html`. Também foram definidos `preconnects` para melhorar o carregamento da fonte.

No `global.css`, foi criada uma variável principal de fonte (`font-family`) e um conjunto de variáveis tipográficas para títulos e textos (h1, h2, h3, span, text e small), contendo peso, tamanho e line-height. Isso evita ter que consultar o design toda hora e padroniza o uso das fontes no projeto.

Além disso, a fonte foi aplicada no `body`, e os headings (`h1, h2, h3`) foram configurados com `font: inherit`, garantindo que eles herdem estilos do contexto onde estiverem, ao invés de usar o padrão do navegador.

---

## 2. Ajustes básicos de elementos
Foi feito um ajuste nos links (`a`), removendo sublinhado (`text-decoration: none`) e usando `color: inherit` para manter a cor padrão do layout.

Também foi criado um efeito de hover nos links, mudando a cor para a variável de cor principal do projeto. Isso melhora a consistência visual e facilita manutenção futura.

Outro ponto importante foi entender o uso de herança (`inherit`), permitindo que os elementos se adaptem dinamicamente ao contexto (ex: diferentes cards com tamanhos de título diferentes).

---

## 3. Git ignore e versionamento
Foi adicionado um arquivo `.gitignore` para ignorar arquivos desnecessários no repositório (como arquivos do sistema operacional, por exemplo no macOS).

Isso mantém o projeto mais limpo e evita subir arquivos inúteis para o controle de versão.

---

## 4. Exportação e organização de assets
Os assets (imagens, ícones e logo) foram exportados do design (Figma) e organizados dentro do projeto.

A estrutura criada foi:

assets/  
├── images/  
├── icons/  
├── ads/  
└── logo


Os ícones foram exportados em SVG (melhor para escalabilidade) e as imagens em PNG. Também foi criado um padrão para ícones de hover (ex: versão azul), separando estados visuais diferentes.

---

## 5. Organização final
Após exportar e organizar todos os arquivos, foi feito um commit registrando as mudanças.

Essa etapa consolida a base visual do projeto: tipografia padronizada + assets organizados, preparando o terreno para começar a montar o layout com Grid nas próximas aulas.