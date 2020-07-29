# \documentclass

A primeira coisa que temos que fazer ao criar um texto, é definir o tipo de documento que será escrito. Para fazer isso, usamos o comando:

``` tex
\documentclass[opções]{classe do documento}
```

### Classe do documento

Por padrão, o LaTeX tem 4 classes de documentos.

- article
- book
- letter
- beamer

Os três primeiros são classes de textos, enquanto o último é utilizado para criação de slides.
Outros formatos também podem ser baixados ou criados, como é o caso da classe abnTeX2, que cria documentos de acordo com as normas da ABNT.

### opções

Além do tipo de documento, podemos definir algumas opções como:

- tamanho da letra
- formato do papel
- número de colunas
- uso de página própria pra título

Para utilizá-las, você precisa colocar as opções entre colchetes e separadas por vírgulas.

Também é importante lembrar que essas opções podem ser omitidas se ela já for pré-definida na classe do documento utilizado.

[lista de opções para o comando documentclass](https://aprendolatex.wordpress.com/2007/03/13/as-classes-e-as-opcoes-de-documentclass/)

### Exemplo

Se eu quiser escrever um artigo em papel a4, fonte 12pt, 2 colunas e sem página de titulo, usarei:

``` tex
\documentclass[a4paper, 12pt, twocolumn, notitlepage]{article}
```