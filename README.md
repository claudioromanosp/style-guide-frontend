# Padrões de Desenvolvimento Front-end

## Práticas Gerais

- Todos os projetos devem ser responsivos.
- Usar o conceito mobile-first.
- Sempre utilizar Html5 e CSS3.
- Sempre comprima as imagens [Tinypng](https://tinypng.com/).
- Compacte os arquivos de produção: HTML, CSS, JS.
- Utilize automatizadores de tarefas como Grunt ou Gulp.
- Dê preferencia em usar ícones como fontes (ex: [Font awesome](http://fontawesome.io)). Caso precise do ícone como imagem utilize as técnicas de Sprite. 
- Caso utilize propriedades CSS modernas garanta que irá funcionar em todos os navegadores. Para isso visite [Can I Use](https://caniuse.com/) e se necessário utilize prefixos **-moz-, -webkit-, -ms-, -o-** .


## HTML

- Utilize somente um **h1** por página (no título principal).
- Utilize h2, h3, h4, h5, h6 em subtítulos de forma estruturada.
- Dê preferência em utilizar [Google Fonts](https://fonts.google.com/).
- Use o elemento **p** para parágrafos.
- Para estilização priorize o uso de CSS. Por exemplo, para aplicar bold em algum texto crie um span com font-weight desejado e aplique:

```html
    // utilize
    <span class="bold">Texto em bold</span>
```
```html
    // ao invés de
    <strong>Texto em bold</strong> ou <b>Texto em bold</b>
```
- Listas devem ser sempre representadas por uma ul ou ol, nunca um conjunto de div.
- Use a tag label para rotular cada campo de um formulário, o atributo for deve associar o rótulo ao campo, para que os usuários possam clicar no rótulo e assim dar foco no campo associado. Utilize cursor: pointer no label.
- Não use o atributo size nos seus campos input e textarea. Ao invés disso, use a propriedade width do CSS.
- Tabelas não devem ser utilizadas para layouts de página.
- Quando utilizar a tag table sempre utilize thead e tbody.
- Nunca use caixa-alta em tags.
- Utilize as tags section, header, footer.
- **Não utilize** a tag **br** para quebrar linhas.
- Todos os atributos das tags devem utilizar aspas duplas.
- Usar hifen quando a classe tiver nome composto, por exemplo: header-menu.
- Priorizar uso de classes no html, só utilize **Id's** caso haja interação com js.
- Na tag **img** inserir o atributo alt.
- Criar nome de arquivos em inglês.
- Ao criar nome de arquivo não deixar espaço vago nem camelCase:
```
    // bom
    nome-do-arquivo
```
```
    // ruim
    nome do arquivo
    NomeDoArquivo
    Nome Do Arquivo
```

## CSS

- Utilizar pré-processadores, como: Sass, Less, Stylus etc. Leia a documentação do pré-processador.
- Nunca utilize estilo inline na tag HTML.
- Use CSS reset para equalizar as diferenças entre os navegadores.
- Estruture seu CSS de forma modularizada, ex:
```
    variables.css
    color-variables.css 
    mixins.css
    forms.css
    footer.css
    header.css
    content.css
    sprites.css
    modal.css
```
- Evite qualificar seletores de forma explícita, exemplo: .borda-do-menu.
- Carregue seu CSS através de arquivos externos.

## JS

- Insira o path dos scripts antes do fechamento da tag body.
- Comente seu código de forma clara e objetiva.
- Nomes de variáveis, arrays, funções em camelCase ou underline.

```javascript
    // bom
    let newVariable
    let new_variable
```
```javascript
    // ruim
    let new-variable
    let newvariable
```
Outras práticas **JS** podem ser adotadas neste excelente guia [Airbnb](https://github.com/claudioromanosp/javascript-style-guide).

## Lembre-se

Ao desenvolver, **seu código deve ser comunitário**. Outras pessoas, de diferentes níveis técnicos, precisarão dar manutenção no mesmo código, fazer novas implementações e ajustes. Por isso, preocupe-se em escrever um código legível, indentado, de fácil manutenção e com comentários relevantes, onde for necessário.

