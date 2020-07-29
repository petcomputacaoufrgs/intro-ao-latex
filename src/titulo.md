# Título

Após criar um documento e importar os seus pacotes, você precisa inserir informações como título, nome da autora ou autor e data.
Para fazer isso, temos três comandos nos documentos padrões do LaTeX para se colocar no preâmbulo:

- `\title{titulo do documento}`
- `\author{autor1 \and autor2}`[^1]
- `\date{data da publicação}`

É importante lembrar que esses comandos são especificos das classes padrões do LaTeX, podendo ser diferente se você usar um modelo importado (ex: abnTeX).

[^1]: O nome de cada autor(a) é dividido usando o comando \and.
Os autores podem fazer agradecimentos especiais como nota de rodapé utilizando o comando
`\thanks{agradecimento}` após o nome de cada um.

### Exemplo

Continuando o nosso documento, se quisermos escrever um artigo chamado "O uso do Lorem Ipsum em exemplos de documentos", escrito por 2 petianos em Julho de 2020, vamos ter o seguinte:

``` tex
\documentclass[a4paper, 12pt, twocolumn, notitlepage]{article}

\usepackage[utf8]{inputenc}
\usepackage[brazil]{babel}
\usepackage{indentfirst}

\title{O uso do Lorem Ipsum em exemplos de documentos}
\author{Jordi Ricarte \and Bruno Zimmermann}}
\date{Julho de 2020}
```