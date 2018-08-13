# Padrões de Desenvolvimento Front-end

## Práticas Gerais

- Todos os projetos devem ser responsivos.
- Usar o conceito mobile-first.
- Para validar nos diversos dispositivos e resoluções utilize [BrowserStack](https://www.browserstack.com/).
- Sempre utilizar Html5 e CSS3.
- Sempre comprima as imagens [Tinypng](https://tinypng.com/).
- Sempre compacte os arquivos de produção: HTMLM, CSS, JS.
- Caso utilize propriedades CSS modernas garanta que irá funcionar em todos os navegadores. Para isso visite [Can I Use](https://caniuse.com/) e se necessário utilize prefixos **-moz-, -webkit-, -ms-, -o-** .


## HTML

- Utilize somente um **h1** por página.
- Dê preferência em utilizar [Google Fonts](https://fonts.google.com/).
- Use o elemento **p** para parágrafos.
- Para estilização sempre priorize o uso de CSS. Por exemplo, para aplicar bold em algum texto crie um span com font-weight desejado e aplique:

```
utilize <span class="bold">Texto em bold</span>
```
```sh
ao invés de <strong>Texto em bold</strong> ou <b>Texto em bold</b>
```
- Listas devem ser sempre representadas por uma ul ou ol, nunca um conjunto de div.
- Use a tag label para rotular cada campo de um formulário, o atributo for deve associar o rótulo ao campo, para que os usuários possam clicar no rótulo e assim dar foco no campo associado. Utilize cursor: pointer no label.
- Não use o atributo size nos seus campos input e textarea. Ao invés disso, use a propriedade width do CSS.
- Tabelas não devem ser utilizadas para layouts de página.
- Quando utilizar a tag table sempre utilize thead e tbody.
- Nunca use caixa-alta em tags.
- Utilize as tags section, header, footer.
- Não utilize a tag **br** para quebrar linhas.
- Todos os atributos das tags devem utilizar aspas duplas.
- Sempre criar nome de classes e id's em inglês.
- Sempre criar nome de arquivos em inglês.
- Usar hifen quando a classe tiver nome composto, por exemplo: header-menu.
- Priorizar uso de classes no html, só utilize **Id's** caso haja interação com js.

## CSS
- Utilizar pré-processadores, como: Sass, Less, Stylus etc.
- Nunca utilize estilo em linha (inline) na tag HTML.
- Use um CSS reset para equalizar as diferenças entre os navegadores.
- Estruture seu CSS de forma modularizada, pensando em reaproveitamento.
- Evite qualificar seletores de forma explícita, exemplo: – .borda-do-menu.
- Carregue seu CSS através de arquivos externos.
- Use o elemento style, dentro do HTML, nunca @import.
- Validar CSS e corrigir possíveis erros.

## JS
- Insira o path dos scripts sempre antes do fechamento da tag body.
- Comente seu código de forma clara e objetiva.
- Nomes de variáveis, arrays, funções sempre em camelCase.

**Certo:**
```sh
	var newVariable
```
**`Errado:`**
```sh
	var new-variable
	var new_variable
	var newvariable
```

## Lembre-se Sempre

Ao desenvolver, **seu código deve ser comunitário**. Outras pessoas, de diferentes níveis técnicos, precisarão dar manutenção no mesmo código, fazer novas implementações e ajustes. Por isso, preocupe-se em escrever um código legível, de fácil manutenção e com comentários relevantes, onde for necessário.