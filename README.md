# Guia de estilo HTML

Um guia de estilo simples para HTML

## Formato

 - O nome do arquivo html deve ser todo em minúsculo e em param case. Exemplo: minha-pagina-web.html.
 - Utilize sempre o formato de arquivo .html e com a codificação UTF-8.
 - Para identar o código, utilize soft tabs (2 espaços em branco).
 - Na primeira linha de código, insira o doctype.
 - Caso o arquivo for um html parcial, insira um underline como prefixo. Exemplo: _cabecalho.html.
 - Ponha o idioma da página na tag html. 
   
  ```html
   <html lang="en-us">
  ```
  
 - Não se esqueça da meta tag indicando o charset da página.

 ```html
   <meta charset="UTF-8">
 ```
 
 
## Sintaxe

 - Sempre utilize aspas duplas nos atributos de um elemento. Nunca utilize aspas simples.
  
 ```html
   <!-- Ruim -->
   <a href='http://www.github.com/' title='Clique aqui' class='blue-link'>Link</a>
   
   <!-- Bom -->
   <a href="http://www.github.com/" title="Clique aqui" class="blue-link">Link</a>
 ```

 - Alguns elementos são auto-fecháveis, não há necessidade de fechà-los              ([Especificação](https://dev.w3.org/html5/spec-author-view/syntax.html#syntax-start-tag))
 
 ```html
   <!-- Ruim -->
   <img src="img/loading.png" alt="Carregando..." />
   <input type="text" id="name" name="user[name]" />
   
   <!-- Bom -->
   <img src="img/loading.png" alt="Carregando...">
   <input type="text" id="name" name="user[name]">
 ```
 
 - Algumas tags são de fechamento obrigatório, não devemos omitir
 
 ```html
   <!-- Ruim -->
   <div class="left-container">
     <h4>Lançamentos da semana</h4>
     <ul class="release-list">
       <li>Filme1
       <li>Filme2
       <li>Filme3
     </ul>
   </div>
   
   <!-- Bom -->
   <div class="left-container">
     <h4>Lançamentos da semana</h4>
     <ul class="release-list">
       <li>Filme1</li>
       <li>Filme2</li>
       <li>Filme3</li>
     </ul>
   </div>
  ```
  
  - Os estilos em cascata (CSS) e os scripts devem estar em arquivos separados do HTML
  
 ```html
  <!-- Ruim -->
  <div style="font-size: 18px">Oi</div>
  <style> .pull-left{ float: left; } </style> 
  <script> alert('Hello world!'); </script> 
 
  <!-- Bom -->
  <link rel="stylesheet" href="style.css">
  <script src="scripts.js"></script>
 ```
 
 - Os atributos booleanos devem ser declarados sem valor
 
 ```html
  <!-- Ruim -->
  <input type="text" disabled="true">
  <input type="checkbox" value="1" checked="checked">
 
  <!-- Bom -->
  <input type="text" disabled>
  <input type="checkbox" value="1" checked>
 ```
