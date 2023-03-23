# Como navegar por um documento HTML ou XML

HÃ¡ dois jeitos padrÃµes de navegar por um documento HTML/XML: XPath e CSS Selector.

Exemplo de XML:

```
<?xml version="1.0" encoding="UTF-8"?>

<bookstore>
  <book>
    <title lang="en">Harry Potter</title>
    <author>J. K. Rowling</author>
    <year>2005</year>
    <price>29.99</price>
  </book>
  <book>
    <title lang="pt">O Iluminado</title>
    <author>Stephen King</author>
    <year>1980</year>
    <price>34.99</price>
  </book>
</bookstore>
```

Exemplo HTML:

```
<html>
  <head></head>
</html>
```

## XPath

https://www.w3schools.com/xml/xpath_intro.asp

### Barras

`/xpto` A partir da raiz do documento, pegue o primeiro elemento do tipo _xpto_.

`//xpto` Em qualquer lugar do documento, pegue o primeiro elemento do tipo _xpto_.

Exemplos:

`/bookstore/book` seleciona o primeiro elemento do tipo _book_ dentro de _bookstore_.

`//year` seleciona o primeiro elemento do tipo _year_ em qualquer lugar.

`/bookstore//year` seleciona o primeiro elemento year em qualquer lugar dentro de _bookstore_.

### Sintaxe de elementos e predicados

`tipo-de-elemento[predicado]`

Exemplos:

`//book[1]` seleciona o primeiro _book_.

`//book[2]` seleciona o segundo _book_.

`//author[text()='J. K. Rowling']` seleciona o _author_ cujo texto seja igual a _J. K. Rowling_.

`//author[contains(text(), 'Rowling')]` seleciona o _author_ cujo texto contenha _Rowling_.

`//title[@lang='pt']` seleciona o _title_ cujo atributo _lang_ seja igual a _pt_.

`//title[@lang!='pt']` seleciona o _title_ cujo atributo _lang_ seja diferente de _pt_.

## CSS Selector

https://www.w3schools.com/cssref/css_selectors.php
