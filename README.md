# html-style-guide
A very simple HTML style guide


## Formato

 - O nome do arquivo html deve ser todo em minúsculo e em param case. Exemplo: minha-pagina-web.html
 - Utilize sempre o formato de arquivo .html e com a codificação UTF-8
 - Para identar o código, utilize soft tabs (2 espaços em branco)
 - Na primeira linha de código, insira o doctype
 - Caso o arquivo for um html parcial, insira um underline como prefixo. Exemplo: _cabecalho.html
 
## Sintaxe

 - Sempre utilize aspas duplas nos atributos de um elemento. Nunca utilize aspas simples.
  
 ```html
  <a href="http://www.github.com/" title="Clique aqui" class="blue-link">Link</a>
 ```

 - Alguns elementos são auto-fecháveis, não há necessidade de fechà-los              ([Especificação](https://dev.w3.org/html5/spec-author-view/syntax.html#syntax-start-tag))
 
```html
  <img src="img/loading.png" alt="Carregando...">
  <input type="text" id="name" name="user[name]">
```
 
 
